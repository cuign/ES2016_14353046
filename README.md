README
====================
Description
---------------------
######由所给资料可知：

The distributed operation layer (DOL) is a framework that enables the (semi-) automatic
mapping of applications onto the multiprocessor SHAPES architecture platform. The DOL
consists of basically three parts:

#####DOL Application Programming Interface: 

The DOL defines a set of computation and communication routines that enable the programming of distributed, parallel
applications for the SHAPES platform. Using these routines, application programmers
can write programs without having detailed knowledge about the underlying
architecture. In fact, these routines are subject to further refinement in the
hardware dependent software (HdS) layer.

#####DOL Functional Simulation: 
To provide programmers a possibility to test their applications, a functional simulation framework has been developed. Besides
functional verification of applications, this framework is used to obtain
performance parameters at the application level.

#####DOL Mapping Optimizati on: 
The goal of the DOL mapping optimization is to compute a set of optimal mappings of an application onto the SHAPES architecture platform.
In a first step, XML based specification formats have been defined that allow to
describe the application and the architecture at an abstract level. Still, all the
information necessary to obtain accurate performance estimates is contained.
How to install
---------------------
按照ppt所给

#####1.安装一些必要的环境(ubuntu为例)：

$    sudo apt-get update

$	sudo apt-get install ant

$ 	sudo apt-get install openjdk-7-jdk

$	sudo apt-get install unzip

#####2.解压文件 编译systemc

$    mkdir dol
新建dol的文件夹

$	unzip dol_ethz.zip -d dol
将dolethz.zip解压到 dol文件夹中

$	tar -zxvf systemc-2.3.1.tgz
解压systemc

$    cd systemc-2.3.1
解压后进入systemc-2.3.1的目录下

$	mkdir objdir
新建一个临时文件夹objdir

$	cd objdir
进入该文件夹objdir

$	../configure CXX=g++ --disable-async-updates
运行configure(能根据系统的环境设置一下参数，用于编译)

$    sudo make install

$    pwd 记录下地址

#####3.编译dol

使用2中的地址对dol中build_zip.xml文件的相应语句进行修改

$    ant -f build_zip.xml all
进入dol文件夹进行编译
#####4.完成 进行测试
Experimental experience
---------------------
在安装第二部最后编译的时候出现了错误，根据提示发现是g++没有正常安装
，重新安装g++之后，重新进行编译就解决了问题
