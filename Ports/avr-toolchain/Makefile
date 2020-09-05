PackName=       Rudix-AVR
Prefix=         /usr/local/$(PackName)

define after_install_hook
        mkdir -p $(InstallDir)/etc/paths.d/
        echo "$(Prefix)/bin" > $(InstallDir)/etc/paths.d/$(Name)
endef
