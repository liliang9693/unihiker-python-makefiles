
> 经过测试发现使用pyenv这个工具来管理和切换Python版本最方便。
> 详情：https://gitee.com/liliang9693/unihiker-pyenv-python

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

