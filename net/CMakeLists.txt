SET(net_SRC
        AsyncSocket.cpp)

ADD_LIBRARY(net SHARED ${net_SRC})

SET(CMAKE_CXX_COMPILER "g++")

INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/base)

#LINK_DIRECTORIES(${PROJECT_SOURCE_DIR}/lynetx/lib)

TARGET_LINK_LIBRARIES(net base)

SET(HEADERS
        AsyncSocket.h)
