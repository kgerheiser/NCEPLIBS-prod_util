file(GLOB EXE_C_SRC ${CMAKE_CURRENT_SOURCE_DIR}/*.c)

set(EXENAME fsync_file)
add_executable(${EXENAME} ${EXE_SRC} ${EXE_C_SRC})

install(TARGETS ${EXENAME}
  RUNTIME DESTINATION ${CMAKE_INSTALL_PREFIX}/bin
  LIBRARY DESTINATION ${CMAKE_INSTALL_PREFIX}/lib
  ARCHIVE DESTINATION ${CMAKE_INSTALL_PREFIX}/lib) 

