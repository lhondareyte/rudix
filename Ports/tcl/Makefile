include ../../Library/GNU.mk

Title=		Tcl
Name=		tcl
Version=	8.6.10
Site=		https://www.tcl.tk/
Source=		https://prdownloads.sourceforge.net/$(Name)/$(Name)$(Version)-src.tar.gz
License=	BSD
Description=	Tool Command Language
UncompressedName= $(Name)$(Version)
GnuConfigureExtra += --enable-framework --enable-aqua

BuildDir=$(SourceDir)/macosx
BuildRequires += $(BinDir)/autoreconf
ReadMeFile=     $(SourceDir)/README.md
LicenseFile=    $(SourceDir)/license.terms

