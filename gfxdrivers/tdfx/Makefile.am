## Makefile.am for DirectFB/src/core/gfxcards/tdfx

INCLUDES = \
	-I$(top_builddir)/include	\
	-I$(top_builddir)/lib	\
	-I$(top_srcdir)/include	\
	-I$(top_srcdir)/lib	\
	-I$(top_srcdir)/systems	\
	-I$(top_srcdir)/src

tdfx_LTLIBRARIES = libdirectfb_tdfx.la

if BUILD_STATIC
tdfx_DATA = $(tdfx_LTLIBRARIES:.la=.o)
endif

tdfxdir = $(MODULEDIR)/gfxdrivers

libdirectfb_tdfx_la_SOURCES =	\
	tdfx.c	\
	tdfx.h

libdirectfb_tdfx_la_LDFLAGS = \
	-module			\
	-avoid-version		\
	$(DFB_LDFLAGS)

libdirectfb_tdfx_la_LIBADD = \
	$(top_builddir)/lib/direct/libdirect.la \
	$(top_builddir)/src/libdirectfb.la


include $(top_srcdir)/rules/libobject.make
	
