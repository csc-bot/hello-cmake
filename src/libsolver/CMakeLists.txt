set(target_name solver)

add_library(${target_name} STATIC)

include(CompileOptions)
set_compile_options(${target_name})

target_sources(
  ${target_name}
  PRIVATE
    libsolver/sqrt.hpp
    libsolver/sqrt.cpp
)

target_include_directories(
  ${target_name}
  PUBLIC
    ${CMAKE_CURRENT_LIST_DIR}
)

target_link_libraries(
  ${target_name}
  PRIVATE
    m
)
