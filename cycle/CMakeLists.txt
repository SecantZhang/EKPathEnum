SET(CYCLE_ENUMERATOR_SRC_FILE_LIST main.cpp cycle_enumerator.cpp)
SET(CYCLE_ENUMERATOR_FIXK_SRC_FILE_LIST main.cpp cycle_enumerator_fixk.cpp)

ADD_EXECUTABLE(CycleEnumerator.out ${CYCLE_ENUMERATOR_SRC_FILE_LIST})
ADD_EXECUTABLE(CycleEnumerator_fixk.out ${CYCLE_ENUMERATOR_FIXK_SRC_FILE_LIST})

TARGET_LINK_LIBRARIES(CycleEnumerator.out graph log io)
TARGET_LINK_LIBRARIES(CycleEnumerator_fixk.out graph log io)