BIN_DIR = ../../../Bin

INC_DIRS = \
	../../../../../Include \
	../../../../../Source

SRC_FILES = \
	../../../../../Source/Modules/nimCodecs/*.cpp

LIB_NAME = nimCodecs
USED_LIBS = OpenNI

ifeq ($(shell ld -ljpeg -o /dev/null 1>&2 2> /dev/null; echo $$?), 0)
  USED_LIBS += jpeg
else
  INC_DIRS  += ../../../../../Source/External/LibJPEG
  SRC_FILES += ../../../../../Source/External/LibJPEG/*.c
endif

include ../../Common/CommonCppMakefile



