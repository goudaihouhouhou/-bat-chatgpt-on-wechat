**下载并且解压WechatGPT**

1、双击“python-3.8.0-amd64-webinstall”安装python，记得勾选“Add Python 3.8 to PATH”

2、点开“chatgpt-on-wechat-master”文件夹，复制路径

3、右键“初始配置”，按“编辑”，将cd后面的路径改成刚才复制的路径，保存退出

4、右键“WechatGPT.bat”，按“编辑”，将cd后面的路径改成刚才复制的路径，保存退出

5、双击“初始配置”

6、双击“WechatGPT.bat”，扫码登录即可使用

**新增**

首先第一步学会"WIN+R"打开"运行"，输入"cmd"进入"命令行"

***微信语音（openai)***

语音识别和回复所需依赖如下：

pip3 install pysilk

pip3 install pysilk-mod

pip3 install pydub

pip install SpeechRecognition

解决ffmpeg not found：在cmd里pip install ffmpeg ,网上下载ffmpeg.py后在环境配置里添加该项

解决import pysilk失败：在cmd里pip install pysilk-mod /pip install silk-python

解决no module named 'tiktoken'：在cmd里pip install tiktoken

解决any to wav error, use raw path. name 'any_to_wav' is not defined：

实在不行就接百度/azure/linkai等API，更方便（可能要加钱）


***安装python之后pip无法使用***

大概率是要重装pip，先将原路径下的pip文件删掉（C:\Users\用户名\AppData\Local\Programs\Python\Python38\Lib\site-packages）

1、使用下面的语句确保没有报错了

python -m ensurepip

2、使用pip -V命令查看，依然提示没有，继续输入如下命令测试是否可用

python -m pip install readline

3、怀疑可能是环境没配置好，所以更新一下pip试试

python -m pip install --upgrade pip

再输入pip，现在就正常了

*如果设置了代理，proxy要填写代理地址*

具体请参考大佬的开源项目：https://github.com/zhayujie/chatgpt-on-wechat
