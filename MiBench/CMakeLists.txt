# add benchmark sub-directories

add_subdirectory(telecomm/adpcm)
add_subdirectory(telecomm/CRC32)
# TODO FIXME toast always produces incorrect output (?), untoast does not work with memory delay turned on!
#add_subdirectory(telecomm/gsm)
add_subdirectory(telecomm/FFT)

add_subdirectory(security/blowfish)
add_subdirectory(security/rijndael)
add_subdirectory(security/sha)
#add_subdirectory(security/pgp)

# ispell requires dirent.h and a file system
#add_subdirectory(office/ispell)
# sphinx requires a file system
#add_subdirectory(office/sphinx)
add_subdirectory(office/rsynth)
add_subdirectory(office/stringsearch)
#add_subdirectory(office/ghostscript)

add_subdirectory(network/dijkstra)
add_subdirectory(network/patricia)

add_subdirectory(automotive/basicmath)
add_subdirectory(automotive/bitcount)
add_subdirectory(automotive/qsort)
add_subdirectory(automotive/susan)

add_subdirectory(consumer/jpeg)
# TODO add test
add_subdirectory(consumer/lame)
# TODO add autogenerated headers, fix cmake files, add tests
#add_subdirectory(consumer/mad)
# TODO convert main functions to accept stdin, run tests
add_subdirectory(consumer/tiff-v3.5.4)
# requires file system
#add_subdirectory(consumer/typeset)
