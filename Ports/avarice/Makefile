include ../../Library/GNU.mk

Title=		avarice
Name=		avarice
Version=	2.13
Site=		https://sourceforge.net/projects/avarice
Source=		http://downloads.sourceforge.net/${Name}/$(Name)-$(Version).tar.bz2
License=        GPL
Description=    CLI for programming Atmel AVR CPUs
ReadMeFile=     $(SourceDir)/NEWS
LicenseFile=    $(SourceDir)/COPYING

BuildRequires += $(BinDir)/pkg-config	# pkgconfig
BuildRequires += $(LibDir)/libusb-*.la	# libusb | static-libusb

include ../avr-toolchain/Makefile
