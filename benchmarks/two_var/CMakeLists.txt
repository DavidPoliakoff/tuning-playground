set(EXE_NAME two_var)
set(N_INCLUDE_DIR ${CMAKE_SOURCE_DIR}/benchmarks/two_var)

add_executable(${EXE_NAME}.exe ${EXE_NAME}.cpp)
target_link_libraries(${EXE_NAME}.exe Kokkos::kokkos)
target_include_directories(${EXE_NAME}.exe PRIVATE ${N_INCLUDE_DIR})
install(TARGETS ${EXE_NAME}.exe)
