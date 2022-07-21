cmake_minimum_required(VERSION 3.23)
project("Asteroids" DESCRIPTION "An implementation of the classic Asteroids for the web!" VERSION 1.0.0.0 LANGUAGES CXX HOMEPAGE_URL "https://www.zachariahs.world/asteroids")

add_executable(${PROJECT_NAME})
target_compile_features(${PROJECT_NAME} PRIVATE cxx_std_20)
target_include_directories(${PROJECT_NAME} PRIVATE include)
target_sources(${PROJECT_NAME} PRIVATE
  "src/main.cpp"
)
