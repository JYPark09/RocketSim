set(target RocketSim)

file(GLOB_RECURSE sources
	${CMAKE_CURRENT_SOURCE_DIR}/*.cc)

add_library(${target} ${sources})
target_link_libraries(${target} Eigen3::Eigen)
