if(TRITON_BUILD_PYTHON_MODULE)
  add_triton_plugin(TritonSPIRV ${CMAKE_CURRENT_SOURCE_DIR}/triton_spirv.cc)
  target_link_libraries(TritonSPIRV PUBLIC PRIVATE Python3::Module pybind11::headers)
endif()
