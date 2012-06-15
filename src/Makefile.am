# library
lib_LIBRARIES = libccityhash.a
libccityhash_a_SOURCES = city.c
if SSE42
include_HEADERS = city.h citycrc.h
else
include_HEADERS = city.h
endif

# test
cityhash_unittest_SOURCES = city-test.c
cityhash_unittest_LDADD = libccityhash.a
TESTS = cityhash_unittest
noinst_PROGRAMS = $(TESTS)
