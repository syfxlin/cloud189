<h1 align="center">- cloud189-cli -</h3>
<pre>
#    /$$$$$$  /$$                           /$$   /$$    /$$$$$$   /$$$$$$ 
#   /$$__  $$| $$                          | $$ /$$$$   /$$__  $$ /$$__  $$
#  | $$  \__/| $$  /$$$$$$  /$$   /$$  /$$$$$$$|_  $$  | $$  \ $$| $$  \ $$
#  | $$      | $$ /$$__  $$| $$  | $$ /$$__  $$  | $$  |  $$$$$$/|  $$$$$$$
#  | $$      | $$| $$  \ $$| $$  | $$| $$  | $$  | $$   >$$__  $$ \____  $$
#  | $$    $$| $$| $$  | $$| $$  | $$| $$  | $$  | $$  | $$  \ $$ /$$  \ $$
#  |  $$$$$$/| $$|  $$$$$$/|  $$$$$$/|  $$$$$$$ /$$$$$$|  $$$$$$/|  $$$$$$/
#   \______/ |__/ \______/  \______/  \_______/|______/ \______/  \______/ 
#                                                                          
--------------------------------------------------------------------------
</pre>

# 准备
1. Python 版本 >= 3.8

2. 安装依赖
    ```sh
    pip install -r requirements.txt
    ```

3. 配置
运行 ``python main.py``, 输入用户名与密码，  
账号为自己的天翼云盘手机号，密码不会有回显，  
也可以 直接两次回车后，输入 `clogin` 按提示输入 `cookie` 登录。  
只简单加密 cookie 并保存至 `.config` 文件。

# 功能

|命令                    |描述                   |
|------------------------|-----------------------|
|login                   |用户名+密码 登录       |
|clogin                  |cookie 登录            |
|ls     + `[文件夹]`     |列处文件与目录         |
|cd     + `文件夹名`     |切换工作目录           |
|upload + `文件路径`     |上传文件               |
|down   + `文件名`       |下载文件               |
|mkdir  + `文件夹名`     |创建文件夹             |
|rm     + `文件/文件夹`  |删除文件(夹)           |
|share  + `文件/文件夹`  |分享文件(夹)           |
|jobs   + `[任务id]`     |查看后台上传下载任务   |
|clear                   |清屏                   |
|rename*                 |重命名                 |
|mv*                     |移动文件               |
|bye/exit                |退出                   |

*还未完成，在做了……

# 使用
1. 不加参数则进入交互模式
```sh
# 提示符为 >
python main.py
> cd '文件夹'
...
> ls
...
> bye
```

2. 带上命令与参数  
```sh
python main.py upload '文件路径'
```  

# License

[GPL-3.0](https://github.com/Aruelius/main/blob/master/LICENSE)

# 致谢

> [LanZouCloud-CMD](https://github.com/zaxtyson/LanZouCloud-CMD)
