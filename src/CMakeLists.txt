add_library(asteroid-compass main.cpp resources.qrc)
set_target_properties(asteroid-compass PROPERTIES PREFIX "")

target_link_libraries(asteroid-compass PUBLIC
	AsteroidApp)

install(TARGETS asteroid-compass
	DESTINATION ${CMAKE_INSTALL_LIBDIR})
