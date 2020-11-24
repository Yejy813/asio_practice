# sync timer
ADD_EXECUTABLE(sync_timer sync_timer_test.cpp)
TARGET_LINK_LIBRARIES(sync_timer pthread)

# async timer
ADD_EXECUTABLE(async_timer async_timer_test.cpp)
TARGET_LINK_LIBRARIES(async_timer pthread)

# async timer, bind arg to a handler
ADD_EXECUTABLE(async_timer_bind_arg async_timer_bind_arg.cpp)
TARGET_LINK_LIBRARIES(async_timer_bind_arg pthread)

# async timer, member function
ADD_EXECUTABLE(async_timer_mb_function async_timer_mb_function.cpp)
TARGET_LINK_LIBRARIES(async_timer_mb_function pthread)

# async timer multi thread
ADD_EXECUTABLE(async_timer_in_multi_thread async_timer_in_multi_thread.cpp)
TARGET_LINK_LIBRARIES(async_timer_in_multi_thread pthread)