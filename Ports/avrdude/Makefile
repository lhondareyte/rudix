include ../../Library/GNU.mk

Title=		avrdude
Name=		avrdude
Version=	6.3
Site=		https://www.nongnu.org/avrdude/
Source=         http://download.savannah.gnu.org/releases/$(Name)/$(Name)-$(Version).tar.gz
License=        GPL
Description=    CLI for programming Atmel AVR CPUs
ReadMeFile=     $(SourceDir)/README
LicenseFile=    $(SourceDir)/COPYING

BuildRequires += $(BinDir)/pkg-config	# pkgconfig
BuildRequires += $(LibDir)/libusb-*.la	# libusb | static-libusb

include ../avr-toolchain/Makefile
