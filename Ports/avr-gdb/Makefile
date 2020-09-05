include ../../Library/GNU.mk

Title=		avr-gdb 
Name=		avr-gdb
Version=	7.8
Site=		http://www.gnu.org/software/gdb/
Source=		https://ftpmirror.gnu.org/gdb/gdb-$(Version).tar.xz
License=	GPL
Description=	GNU debugger for AVR cross-development
ReadMeFile=	$(SourceDir)/README
LicenseFile=    $(SourceDir)/COPYING

UncompressedName  =  gdb-$(Version)
GnuConfigureExtra =  --target=avr --prefix=$(Prefix)
GnuConfigureExtra += --program-prefix="avr-" --disable-nls --disable-werror

include ../avr-toolchain/Makefile
