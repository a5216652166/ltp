#
# Read COPYING for licensing details.
#
# Garrett Cooper, June 2010
#

all clean install test:
	@for dir in `ls -d */Makefile 2>/dev/null | sed -e 's,/Makefile$$,,g'`; do \
		$(MAKE) -C $$dir $@;						  \
	done

distclean-makefiles:
	@find */ -name 'Makefile*' | xargs rm -f
