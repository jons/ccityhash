# library
lib_LTLIBRARIES = libccityhash.la
libccityhash_la_SOURCES = city.c
if SSE42
include_HEADERS = city.h citycrc.h
else
include_HEADERS = city.h
endif

libccityhash_la_LDFLAGS = -version-info ${CCITYHASH_LTVER}

# test
cityhash_unittest_SOURCES = city-test.c
cityhash_unittest_LDADD = libccityhash.la
TESTS = cityhash_unittest
noinst_PROGRAMS = $(TESTS)
