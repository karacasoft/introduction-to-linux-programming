cmake_minimum_required(VERSION 3.5.1)

set(CMAKE_CXX_STANDARD 11)

project(03-file-operations)

add_executable(cat 
  src/cat.c
)

add_executable(random 
  src/random.c
)

add_executable(ls 
  src/ls.c
)

add_executable(size 
  src/size.c
)

add_executable(touch
  src/touch.c
)

add_executable(tee
  src/tee.c
)

add_executable(rm
  src/rm.c
)

add_executable(mkdir
  src/mkdir.c
)

configure_file(src/read-this.txt 
  ${CMAKE_BINARY_DIR}/${PROJECT_NAME} COPYONLY
)
