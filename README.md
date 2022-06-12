# DDK_Yocto_Project_Learning
The Yocto Project (YP) is an open source collaboration project that helps developers create custom Linux-based systems regardless of the hardware architecture.

# Let us get started

## What is Poky?
Poky is a distribution of the Yocto Project.</br>
It is simillar to linux that has many distributions, such as Ubuntu, Debian. </br>
Poky uses "OpenEmbedded(oe) Build System" that includes "BitBake" and "OpenEmbedded Core". </br>

## What is BitBake?
make is to makefile what bitbake is to recipe. </br>

## Download Poky
Clone poky from the paths below in https://git.yoctoproject.org/poky/ . </br>

![Screen Shot 2022-06-12 at 8 56 46 PM](https://user-images.githubusercontent.com/67073582/173234328-8912380c-743b-4a31-8814-5de7b844441f.png) </br>

Poky also has different versions, such as Release 4.0 (kirkstone), Release 3.4 (honister) and Release 3.3 (hardknott). </br>
Now, we use "RELEASE YP CORE - KIRKSTONE 4.0.1 - 2022.05.20" . </br>
```git
git clone -b kirkstone git://git.yoctoproject.org/poky.git
```
... </br>

# References
1. https://www.yoctoproject.org/learn/
2. https://www.yoctoproject.org/software-item/poky/
3. https://docs.yoctoproject.org/brief-yoctoprojectqs/index.html
