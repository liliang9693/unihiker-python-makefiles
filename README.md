
> After testing, I found that using the pyenv tool to manage and switch Python versions is the most convenient.  
> Details: https://github.com/liliang9693/unihiker-pyenv-python

# unihiker-python-makefiles
Store multiple Python compiled files suitable for the UNIHIKER system.

This repository contains files made after various versions of Python for UNIHIKER. You can download the package in the [release page](https://github.com/liliang9693/unihiker-python-makefiles/releases) to UNIHIKER, and then install it, to install a higher version of Python on UNIHIKER.



## Python 3.8

```
cd ~
mkdir pythonNew
cd pythonNew
wget https://github.com/liliang9693/unihiker-python-makefiles/releases/download/3.8.5/Python-3.8.5-make-done.tar.gz
tar -xf Python-3.8.5-make-done.tar.gz
cd Python-3.8.5/
#Use altinstall to install Python, which will coexist with the original Python system. The command execution takes about ten minutes.
sudo make altinstall

#The python3.8 command invokes the Python 3.8 version, while the python command invokes the original system Python.
python3.8 --version

#To install libraries for the new 3.8 version, you need to use the pip3.8 command.
pip3.8 list

#Install common dependency libraries.
pip3.8 install pinpong numpy unihiker siot 
pip3.8 list

```



## Python 3.12

```
cd ~
mkdir pythonNew
cd pythonNew
wget https://github.com/liliang9693/unihiker-python-makefiles/releases/download/3.11%263.12/Python-3.12.7-make-done.tar.gz
tar -xf Python-3.12.7-make-done.tar.gz
cd Python-3.12.7/
#Use altinstall to install Python, which will coexist with the original Python system. The command execution takes about ten minutes.
sudo make altinstall

#The python3.12 command invokes the Python 3.12 version, while the python command invokes the original system Python.
python3.12 --version

#To install libraries for the new 3.12 version, you need to use the pip3.12 command.
pip3.12 list

#Install common dependency libraries.
pip3.12 install pinpong numpy unihiker siot 
pip3.12 list

```


- Reference tutorial: https://www.dfrobot.com/forum/topic/322359

- Python package source file download location: https://www.python.org/ftp/python/

- File Description: .tgz is the source file downloaded from python.org, .tar.gz is the compiled file that can be installed on the UNIHIKER,The compiled file is in the release page..

  

---




# 说明
- 本仓库仅适合行空板M10
- 由于直接通过python源码包安装需要很长时间的编译，因此本仓库提供编译好的文件，方便直接安装
- 仅适合有一定动手能力及linux命令行操作经验的用户


# 操作步骤

## 下载文件
下载编译好的适合行空板M10的python环境包，得到.tar.gz文件。
- github releases：https://github.com/liliang9693/unihiker-python-makefiles/releases/
- 百度网盘：https://pan.baidu.com/s/1QztYTRdncrSQv1S6CDKysg?pwd=pylb 

## 上传文件到行空板M10
- 在行空板M10上新建一个pythonNew文件夹
- 将Python-3.12.7-make-done.tar.gz文件上传到pythonNew中

## 安装
命令行操作

```
cd pythonNew
# 解压文件
tar -xf Python-3.12.7-make-done.tar.gz
cd Python-3.12.7/

#安装python3.12，预计需要十几分钟
sudo make altinstall

#安装完成使用python3.12命令操作，原来的python命令操作的是系统自带的python3.7
python3.12 --version

#安装python库到python3.12中要使用pip3.12，原来的pip命令操作的是系统自带的python3.7的库
pip3.12 list


```

- 原始教程: https://www.dfrobot.com/forum/topic/322359

- python源码下载地址: https://www.python.org/ftp/python/

