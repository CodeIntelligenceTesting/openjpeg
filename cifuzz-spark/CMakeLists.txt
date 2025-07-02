#cifuzz:build-template:begin
#add_fuzz_test({{ .FuzzTestName }} {{ .FileName }})
#target_include_directories({{ .FuzzTestName }} PRIVATE ${CMAKE_SOURCE_DIR}/src/lib/openjp2 ${CMAKE_BINARY_DIR}/src/lib/openjp2 ${CMAKE_SOURCE_DIR}/src/bin/common ${CMAKE_BINARY_DIR}/src/bin/common)
#target_link_libraries({{ .FuzzTestName }} PRIVATE "$<LINK_LIBRARY:WHOLE_ARCHIVE,openjp2_static>")
#cifuzz:build-template:end
