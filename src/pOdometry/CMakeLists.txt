#--------------------------------------------------------
# The CMakeLists.txt for:                       pOdometry
# Author(s):                              Manuel Agraz
#--------------------------------------------------------

SET(SRC
  Odometry.cpp
  Odometry_Info.cpp
  main.cpp
)

ADD_EXECUTABLE(pOdometry ${SRC})

TARGET_LINK_LIBRARIES(pOdometry
   ${MOOS_LIBRARIES}
   apputil
   mbutil
   m
   pthread)

