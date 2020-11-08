include_directories(.)

add_executable(timer  timer.cpp)

add_executable(progress_timer progress_timer.cpp)
add_executable(progress_display progress_display.cpp)

add_executable(date1 date1.cpp)
target_link_libraries (date1 ${Boost_LIBRARIES})

add_executable(date2 date2.cpp)
target_link_libraries (date2 ${Boost_LIBRARIES})

add_executable(posix_time posix_time.cpp)
target_link_libraries (posix_time ${Boost_LIBRARIES})

add_executable(datetime datetime.cpp)
target_link_libraries (datetime ${Boost_LIBRARIES})
