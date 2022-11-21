# Yocto BSP for Beagle Bone Black AM335X


## Host build: Ubuntu20.04 LTS

```shell
cd ~

mkdir beagle-bone-black
cd beagle-bone-black

git clone -b dunfell git://git.yoctoproject.org/poky.git
cd poky

git clone -b dunfell https://github.com/openembedded/meta-openembedded.git

git clone git@github.com:tienat/meta-am335x.git

source oe-init-build-env build-am335x
bitbake core-image-minimal
```
