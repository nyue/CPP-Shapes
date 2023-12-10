project(cpp_shapes)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_library(cppshapes
  Circle.cpp
  Circle.h
  IntersectHelper.cpp
  IntersectHelper.h
  Line.cpp
  Line.h
  Printable.cpp
  Printable.h
  Rectangle.cpp
  Rectangle.h
  Vector.cpp
  Vector.h
  Quadtree/QuadtreeItem.h
  Quadtree/QuadtreeArea.cpp
  Quadtree/QuadtreeArea.h
  Quadtree/QuadtreeItem.cpp
  )

add_executable(demo
  main.cpp
  )

target_link_libraries(demo
  cppshapes
  )

