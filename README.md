# RootFS
Petalinux file system (contain development tools, smart package manager and more)

# Smart Install
In order to add new features to Petalinux (Yocto) need to add tags to “EXTRA_IMAGE_FEATURES” field located in “./apu/petalinux_bsp/build/conf/plnxtool.conf”.
For example to use “Smart” package manager use,
	EXTRA_IMAGE_FEATURES += "debug-tweaks package-management"

# Development Tools Install
In order to add development environment add  “packagegroup-self-hosted” in two locations (to be sure)
“./apu/petalinux_bsp/project-spec/meta-plnx-generated/recipes-core/images/petalinux-user-image.bb”
“./apu/petalinux_bsp/project-spec/meta-user/recipes-core/images/petalinux-image.bbappend”

