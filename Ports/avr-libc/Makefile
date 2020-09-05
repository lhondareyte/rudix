include ../../Library/GNU.mk

Title=		avr-libc
Name=		avr-libc
Version=	2.0.0
Site=		https://www.sourceware.org
Source=		https://download.savannah.gnu.org/releases/$(Name)/$(Name)-$(Version).tar.bz2
License=	GPL
Description=	libc for AVR cross-development
ReadMeFile=	$(SourceDir)/README
LicenseFile=    $(SourceDir)/LICENSE

OsVersion=      $(shell uname -v)
CanonicaOSName=  $(Arch)-apple-darmin$(OsVersion)

GnuConfigureExtra =  --host=avr --prefix=/usr/local/CrossPack-AVR
GnuConfigureExtra += --build=$(CanonicalOSName)

include ../avr-toolchain/Makefile
