# 设置 Git
    git config --global user.name "Xiangsu Chen"
    git config --global user.email pgin.oth@gmail.com
* * *
# 安装与配置 VSCode 插件
1. ***Settings Sync***
    * 登陆 GitHub
    * GistID：c8a35873111e13028bbf829f70d5bec6
    * Shift+Alt+D 下载 Gist 配置，Shift+Alt+U 上传 Gist 配置。
2. ***Git Graph***
    * 可视化显示 Git 分支
    * 在这里可以配置 ***<font face="微软雅黑" color=red>user.name</font>*** 和 ***<font color=red>user.email</font>***
***
# Windows 中配置 venv
在终端设置命令执行的路径为当前项目路径，执行以下代码进行部署：

    .venv/Scripts/pip freeze > _requirements_old.txt
    .venv/Scripts/pip uninstall -r requirements.txt -y
    Remove-Item '.venv' -Recurse
    python -m venv .venv
    .venv/Scripts/python -m pip install --upgrade pip
    .venv/Scripts/pip install -r requirements.txt
    .venv/Scripts/pip install auto-py-to-exesd
    .venv/Scripts/Activate.ps1

如果脚本被Windows阻止执行，则需要[设置系统执行策略](https:/go.microsoft.com/fwlink/?LinkID=135170)：

    Set-ExecutionPolicy -ExecutionPolicy AllSigned -Scope CurrentUser
*****
# VSCode 使用技巧
在 VSCode 中按下 **Ctrl+Shift+p** 弹出命令输入栏，输入`Python: Select interpreter`为项目选择 *Python 解释器* 的路径
- - -
# <div align=center><img src="./img/player.png" width="10%" height="10%"> 项目结构</div>

|文件夹路径 | 说明 |
| ---: | :--- |
|./img/ | 存放游戏用到的图像文件 |
|./sound/ | 存放游戏用到的声音文件 |

---------------------------------------
