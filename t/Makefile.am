# INCLUDES                    = @CHECK_CFLAGS@
TESTS                       = check_main
AM_CFLAGS = -ggdb -Wall $(DEPS_CFLAGS) -I$(top_builddir) -I$(top_builddir)/include  @CHECK_CFLAGS@
AM_LDFLAGS = $(DEPS_LIBS) -L$(top_builddir)/src @CHECK_LIBS@

dist_noinst_DATA = \
	$(NULL)

noinst_PROGRAMS             = $(TESTS)

check_main_SOURCES = check_main.c
# check_main_LDADD=$(DEPS_LIBS) -L$(top_builddir)/src @CHECK_LIBS@
# check_main_CFLAGS=$(DEPS_CFLAGS) -I$(top_builddir) -I$(top_builddir)/include @CHECK_CFLAGS@

check_PROGRAMS = $(TESTS)

# AM_CFLAGS=$(DEPS_CFLAGS) -I$(top_builddir)/include
# AM_CFLAGS=$(DEPS_CFLAGS) -I$(top_builddir) -I$(top_builddir)/include
CLEANFILES    += check_main.log
