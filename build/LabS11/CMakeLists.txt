cmake_minimum_required(VERSION 3.10)
project(LabS11)
set(CMAKE_CXX_STANDARD 98)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pthread -static-libgcc -static-libstdc++")
set(CMAKE_C_FLAGS_DEBUG "${CMAKE_CXX_FLAGS_DEBUG}")
set(CMAKE_CXX_FLAGS_DEBUG "${CMAKE_CXX_FLAGS_DEBUG}")
set(CMAKE_C_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE}")
set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE}")
include_directories(
  "D:/TommyT/TechProg/TP2/optick/include"
)
set(SOURCE_FILES
  "D:/TommyT/TechProg/TP2/optick/src/optick.config.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_capi.cpp"
  "D:/TommyT/TechProg/TP2/optick/src/optick_capi.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_common.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_core.cpp"
  "D:/TommyT/TechProg/TP2/optick/src/optick_core.freebsd.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_core.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_core.linux.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_core.macos.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_core.platform.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_core.win.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_gpu.cpp"
  "D:/TommyT/TechProg/TP2/optick/src/optick_gpu.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_memory.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_message.cpp"
  "D:/TommyT/TechProg/TP2/optick/src/optick_message.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_miniz.cpp"
  "D:/TommyT/TechProg/TP2/optick/src/optick_miniz.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_serialization.cpp"
  "D:/TommyT/TechProg/TP2/optick/src/optick_serialization.h"
  "D:/TommyT/TechProg/TP2/optick/src/optick_server.cpp"
  "D:/TommyT/TechProg/TP2/optick/src/optick_server.h"
  "D:/TommyT/TechProg/TP2/Sources/labo.cpp"
  "D:/TommyT/TechProg/TP2/Sources/labo.h"
  "D:/TommyT/TechProg/TP2/Sources/main.cpp"
  "D:/TommyT/TechProg/TP2/Sources/stb_image.h"
  "D:/TommyT/TechProg/TP2/Sources/stb_image_write.h"
)
add_executable(LabS11 ${SOURCE_FILES})
target_link_libraries(LabS11
)
