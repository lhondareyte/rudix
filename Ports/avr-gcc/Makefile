include ../../Library/GNU.mk

LocalLib=     /usr/local/lib
BuildRequires += $(BinDir)/pkg-config	# pkgconfig
BuildRequires += $(LocalLib)/libgmp.la	# gmp
BuildRequires += $(LocalLib)/libmpfr.la	# mpfr
BuildRequires += $(LocalLib)/libmpc.la	# mpc

Title=		avr-gcc 
Name=		avr-gcc
Version=	5.4.0
Site=		https://www.sourceware.org
Source=		https://mirrors.kernel.org/sourceware/gcc/releases/gcc-$(Version)/gcc-$(Version).tar.bz2
License=	GPL
Description=	GNU compiler for AVR cross-development
ReadMeFile=	$(SourceDir)/README
LicenseFile=    $(SourceDir)/COPYING

UncompressedName  =  gcc-$(Version)
GnuConfigureExtra =  --target=avr --prefix=$(Prefix)
GnuConfigureExtra += --disable-libssp --enable-languages="c c++"
GnuConfigureExtra += --with-gmp --with-mpfr --with-mpc
GnuConfigureExtra += --enable-bootstrap=no
GnuConfigureExtra += --disable-dependency-tracking --disable-nls --disable-werror
include ../avr-toolchain/Makefile

define after_prep_hook
	mkdir $(SourceDir)/gcc/include
endef
