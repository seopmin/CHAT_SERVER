cmake_minimum_required(VERSION 3.12)
project(MesTCPChat)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

include_directories(include)


#Boost 라이브러리 설치 확인
find_package(Boost)

if(Boost_FOUND)
    # include 패스 설정
    include_directories(${Boost_INCLUDE_DIRS})
endif()



add_subdirectory(client)
add_subdirectory(server)
