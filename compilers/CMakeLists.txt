FILE(GLOB_RECURSE ALL_LIB_CPP *.h)

ADD_LIBRARY(compilers
  ${ALL_LIB_CPP}
)

SET_TARGET_PROPERTIES(compilers PROPERTIES LINKER_LANGUAGE CXX)

TARGET_LINK_LIBRARIES(compilers
  ${DEPS}
)
