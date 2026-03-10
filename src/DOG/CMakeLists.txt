
set(DOG_SOURCE DOG.cxx
        ../GaussianLPF/GaussianLPF.cxx
        ../GradientAD/GradientAD.cxx
        ../CurvatureAD/CurvatureAD.cxx)
GENERATECLP(DOG_SOURCE DOG.xml)


add_executable(DOG_${MYHAWKID} ${DOG_SOURCE})
target_link_libraries(DOG_${MYHAWKID} ${ITK_LIBRARIES})
