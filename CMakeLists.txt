cmake_minimum_required(VERSION 2.8.4)
project(ffmpeg_helloworld)

set(SOURCE_FILES main.c)

include_directories("/usr/local/include")

link_directories("/usr/local/lib")

add_executable(ffmpeg_helloworld ${SOURCE_FILES})

target_link_libraries(ffmpeg_helloworld "libavformat.a")

target_link_libraries(ffmpeg_helloworld "libavutil.a")

target_link_libraries(ffmpeg_helloworld "libavcodec.a")

target_link_libraries(ffmpeg_helloworld "libavfilter.a")
