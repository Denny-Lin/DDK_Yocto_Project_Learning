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

Below is the original poky folder. </br>
![Screen Shot 2022-06-12 at 9 55 09 PM](https://user-images.githubusercontent.com/67073582/173236667-ab4032fa-6053-4a67-a886-63299ee1aee9.png)

## Enable BitBake
Use the following command to enable the instruction of bitbake. </br>
```sh
source oe-init-build-env
```

![Screen Shot 2022-06-12 at 10 10 38 PM](https://user-images.githubusercontent.com/67073582/173237300-11102460-dcc3-46d5-8154-3d0d85a7ed2e.png)


## Run BitBake
```sh
bitbake core-image-sato
```

```sh
bitbake -s 
bitbake [recipe]
```
... </br>

## What is recipe?
Recipes are denoted by the file extension .bb . </br>
Each recipe implicitly inherits base.bbclass that has many tasks, and each task is similar to a function(). </br>
If we use bitbake to run all the recipes or specified recipe, the running recipe(s) will do all the tasks implemented by the base.bbclass. </br>
Below are the default execution sequence of all the recipes: </br>
1. do_
2. do_

Otherwise, if we do not like the task made by default in base.bbclass, we can override or prohibit this task in our recipe. </br>
Here is an example. </br>

```bb
...
```

... </br>

## What is layer?
... </br>

# References
1. https://www.yoctoproject.org/learn/
2. https://www.yoctoproject.org/software-item/poky/
3. https://docs.yoctoproject.org/brief-yoctoprojectqs/index.html
4. https://www.yoctoproject.org/software-overview/downloads/
5. https://docs.yoctoproject.org/ref-manual/classes.html
6. 
