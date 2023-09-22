include_directories(./include)
aux_source_directory(. DIR_LIB_SRCS)
aux_source_directory(./include DIR_INC_SRCS) 
add_library(Server ${DIR_LIB_SRCS})