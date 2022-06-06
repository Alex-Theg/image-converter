cmake_minimum_required(VERSION 3.14)

project(image-converter LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)


set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)


add_executable(image-converter
  main.cpp
  converter.cpp converter.h
  imageReader.cpp imageReader.h
  presenter.cpp presenter.h
  translator.cpp translator.h
  cellProcessor.cpp cellProcessor.h
  gridWalker.cpp gridWalker.h
  cell.cpp cell.h
)

target_link_libraries(image-converter )
