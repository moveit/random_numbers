cmake_minimum_required(VERSION 3.5)
project(random_numbers)

# Default to C++14
if(NOT CMAKE_CXX_STANDARD)
  set(CMAKE_CXX_STANDARD 14)
endif()

find_package(ament_cmake REQUIRED)
find_package(Boost REQUIRED date_time system thread)

include_directories(
  include
  ${Boost_INCLUDE_DIR}
)

add_library(${PROJECT_NAME} SHARED
  src/random_numbers.cpp
)

target_link_libraries(${PROJECT_NAME} ${Boost_LIBRARIES})

ament_target_dependencies(${PROJECT_NAME})
ament_export_libraries(${PROJECT_NAME})
ament_export_include_directories(include)

install(
	TARGETS ${PROJECT_NAME}
	ARCHIVE DESTINATION lib
	LIBRARY DESTINATION lib
	RUNTIME DESTINATION bin
)

install(DIRECTORY include/
        DESTINATION include)

ament_package()
