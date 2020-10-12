include ../../Library/Unix.mk

Title=		openocd
Name=		openocd
Version=	0.10.0
Site=		https://sourceforge.net/p/stm32flash/wiki/Home/
Repository=	https://git.code.sf.net/p/openocd/code
License=	GPL
Description=	Open On-Chip Debugger
SourceDir=	openocd-code
ReadMeFile=	$(SourceDir)/README
LicenseFile=	$(SourceDir)/COPYING

UncompressedName=stm32flash-code

define retrieve_hook
rm -rf $(SourceDir) && git clone $(Repository) $(SourceDir)
endef

define prep_hook
cd $(SourceDir) && git checkout v$(Version) && \
	git submodule init && git submodule update && cd -
endef

define after_prep_hook
cd $(BuildDir) && autoreconf -fi configure.ac && ./configure && cd -
endef
