CMAKE_MINIMUM_REQUIRED(VERSION 2.8)
PROJECT(CuTest)

IF(MSVC)
	ADD_DEFINITIONS( -D_CRT_SECURE_NO_WARNINGS )
ENDIF(MSVC)
AUX_SOURCE_DIRECTORY(. DIR_SRC_FILES)
ADD_EXECUTABLE(cutesttest ${DIR_SRC_FILES})