# Xshell

[Xshell] 是一款安全壳层客户端。

## 常用操作序列

### 同步文件夹

假定目标：欲将本机 `C:\src` 某目录同步到远程 `/var/dst` 某目录

1.  运行 Xftp；
0.  打开本机和远程会话；
0.  从标准按钮栏或菜单栏“工具”菜单中，点击“同步文件夹”按钮，打开“同步处理”对话框；
0.  对话框左上角，会话选择 `local`，目录路径选择 `C:\src`；
0.  对话框右上角，会话选择 `remote`，目录路径选择 `/var/dst`；
0.  同步方向选择“从左到右”，点击“比较”按钮；
0.  点击“传输”按钮开始同步。

## 注册码

请到官网申领个人版或购买商业版以支持正版。

或可转用自由软件世界的替代方案：[WinSCP](https://winscp.net/) + [PuTTY](https://putty.org/) 。

??? cite "注册机（已失效）"

    !!! warning "声明"

        据《中华人民共和国著作权法（2010年2月26日第二次修正版）》第二十二条，下述行为及其影响仅可用于“为个人学习、研究或者欣赏”，不得用于其他用途。

    1.  访问 [十分钟邮箱](https://10minutemail.com/) 或 [临时邮箱](https://temp-mail.org/) 以获取一个临时邮箱；

    0.  另开标签页，访问 [Xmanager Power Suite 下载页面](https://www.netsarang.com/xmanager-power-suite-download/)，选择“30 天评估”，填入必选信息获取下载地址；

    0.  返回临时邮箱标签页，此时应当会收到一封邮件，内有下载页面地址，形如：

        ``` text
        https://www.netsarang.com/downloading/?token=*
        ```

    0.  访问下载页面，醒目处有“begin downloading”超链接，其链接地址形式如下：
        
        试用版，有时间和标签页限制：

        :   `https://cdn.netsarang.net/????????/XmanagerPowerSuite-?.?.????.exe`
        
        个人版，有标签页限制：

        :   `https://cdn.netsarang.net/????????/XmanagerPowerSuite-?.?.????p.exe`
        
        注册版，需要注册：

        :   `https://cdn.netsarang.net/????????/XmanagerPowerSuite-?.?.????r.exe`
        
        选择需要的版本并下载。

    0.  安装前，若有安装旧版则卸载旧版，并清除注册表：

        ``` doscon
        %USERPROFILE%> REG DELETE HKEY_CURRENT_USER\Software\NetSarang /f
        ```

    0.  若选择的是注册版，则需要注册码。下载 `Xmanager-keygen.py` 并运行，以获取注册码。一些可能有效的下载地址：
        
        *   https://github.com/DoubleLabyrinth/Xmanager-keygen
        *   https://github.com/HeartZhang/Xmanager-keygen

    0.  显然，官方并不认可以此种方式获取到的注册码，所以需要使用一点点额外技术手段来屏蔽联网验证。使用管理员权限启动你喜爱的文本编辑器，比如 `notepad.exe`，打开 `%WINDIR%\System32\drivers\etc\hosts` 并在其中加入以下内容：

        ``` text
        127.0.0.1 sales.netsarang.com
        127.0.0.1 transact.netsarang.com
        127.0.0.1 update.netsarang.com
        127.0.0.1 www.netsarang.com
        127.0.0.1 www.netsarang.co.kr
        ```

    0.  安装；

    0.  上述行为及其影响仅可用于“为个人学习、研究或者欣赏”，不得用于其他用途。

<!----------------------------------------------------------------------------->

[Xshell]: https://www.netsarang.com/free-for-home-school/ "Xshell and Xftp Free Licensing"
