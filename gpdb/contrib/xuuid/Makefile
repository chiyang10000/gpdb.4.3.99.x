MODULES = xuuid 
OBJS = xuuid.o 
DATA_built = xuuid.sql
DATA = uninstall_xuuid.sql

ifdef USE_PGXS
PGXS = $(shell pg_config --pgxs)
include $(PGXS)
else
subdir = contrib/xuuid
top_builddir = ../..
include $(top_builddir)/src/Makefile.global
include $(top_srcdir)/contrib/contrib-global.mk
endif

SHLIB_LINK = -L/$(TOOLCHAIN_DIR)/installed/lib 
