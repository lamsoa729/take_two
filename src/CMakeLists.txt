set (HEADERS ../include/take_two/take_two.hpp)

add_library(TakeTwo STATIC take_two.cpp ${HEADERS})

target_include_directories(TakeTwo PUBLIC ../include)

# Installs to local computer
install (TARGETS TakeTwo DESTINATION lib)
install (FILES ${HEADERS} DESTINATION include/take_two)
