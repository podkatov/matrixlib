project(MatrixLib)

set(HEADER_FILES
        Matrix.h
        )

set(SOURCE_FILES
        Matrix.cpp
        )

add_library(src STATIC ${SOURCE_FILES} ${HEADER_FILES})