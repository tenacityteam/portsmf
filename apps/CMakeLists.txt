add_executable(allegroconvert allegroconvert.cpp)
target_link_libraries(allegroconvert PRIVATE PortSMF)

find_package(PortMidi REQUIRED)
add_executable(allegroplay allegroplay.cpp seq2midi.cpp)
target_link_libraries(allegroplay PRIVATE PortSMF PortMidi::PortMidi)
