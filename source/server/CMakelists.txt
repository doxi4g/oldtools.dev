project("test")

CollectSourceFiles(
 ${CMAKE_CURRENT_SOURCE_DIR} 
  SOURCES)

GroupSources(
 ${CMAKE_CURRENT_SOURCE_DIR})

add_executable(${PROJECT_NAME} ${SOURCES})

target_link_libraries(${PROJECT_NAME}
 PRIVATE 
  
 PUBLIC
   )

set_target_properties(${PROJECT_NAME} 
 PROPERTIES 
  FOLDER 
    server)
