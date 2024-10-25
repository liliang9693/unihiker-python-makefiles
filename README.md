# unihiker-python-makefiles
Store multiple Python compiled files suitable for the UNIHIKER system.

This repository contains files made after various versions of Python for UNIHIKER. You can download the package in the [release page](https://github.com/liliang9693/unihiker-python-makefiles/releases) to UNIHIKER, and then install it, to install a higher version of Python on UNIHIKER.

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

Reference tutorial: https://www.dfrobot.com/forum/topic/322359

