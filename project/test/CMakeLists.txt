add_executable(iterator_tests 
    "TestIterators.cpp"
)
target_link_libraries(iterator_tests PRIVATE Catch2::Catch2WithMain)
add_test(iterator_tests iterator_tests)
