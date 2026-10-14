add_library(minimp3 STATIC minimp3.c)

target_include_directories(minimp3 PUBLIC ${CMAKE_CURRENT_LIST_DIR})
target_compile_definitions(minimp3 PRIVATE MINIMP3_ONLY_MP3 MINIMP3_NO_SIMD)
