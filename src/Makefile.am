lib_LTLIBRARIES = libauto-project.la
libr3_la_SOURCES = main.c
# libr3_la_LDFLAGS = -export-symbols-regex '^r3_|^match_'

libr3_la_LIBADD=$(DEPS_LIBS)
AM_CFLAGS=$(DEPS_CFLAGS) -I$(top_builddir) -I$(top_builddir)/include -Wall -std=c99

if USE_JEMALLOC
AM_CFLAGS += -ljemalloc
endif

if ENABLE_DEBUG
AM_CFLAGS += -ggdb -fprofile-arcs -ftest-coverage
endif

