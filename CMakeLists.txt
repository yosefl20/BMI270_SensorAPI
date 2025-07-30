set(SDK_SOURCES 
       bmi2_ois.c
       bmi2.c
       bmi270_context.c
       bmi270_dsd.c
       bmi270_legacy.c
       bmi270_maximum_fifo.c
       bmi270.c
       )

idf_component_register(SRCS ${SDK_SOURCES}
                       INCLUDE_DIRS
                              "."
                       PRIV_REQUIRES
                            driver
                       REQUIRES ""
                       )
