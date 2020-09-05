include ../../Library/GNU.mk

Title=		avr-binutils
Name=		avr-binutils
Version=	2.32
Site=		https://www.sourceware.org
Source=		https://mirrors.kernel.org/sourceware/binutils/releases/binutils-2.32.tar.bz2
License=	GPL
Description=	GNU binutils for AVR cross-development
ReadMeFile=	$(SourceDir)/README
LicenseFile=    $(SourceDir)/COPYING

UncompressedName=binutils-$(Version)
GnuConfigureExtra= --target=avr --prefix=$(Prefix)

include ../avr-toolchain/Makefile
