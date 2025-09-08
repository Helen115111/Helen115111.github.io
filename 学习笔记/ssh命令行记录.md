
==PS D:\md_files>== git remote -v
github  https://github.com/Helen115111/Helen115111.github.io.git (fetch)
github  https://github.com/Helen115111/Helen115111.github.io.git (push)

---

==PS D:\md_files>== git branch
* main
PS D:\md_files> git branch -r
  github/HEAD -> github/main
  github/main
PS D:\md_files> git branch --set-upstream-to=github/main main
branch 'main' set up to track 'github/main'.
PS D:\md_files>
 *  还原的历史记录 

==PS D:\md_files>== git remote -v
github  https://github.com/Helen115111/Helen115111.github.io.git (fetch)
github  https://github.com/Helen115111/Helen115111.github.io.git (push)
==PS D:\md_files>== git pull origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
==PS D:\md_files>== git remote -v
github  https://github.com/Helen115111/Helen115111.github.io.git (fetch)
github  https://github.com/Helen115111/Helen115111.github.io.git (push)
==PS D:\md_files>== git push -u github main --allow-unrealted-histories
error: unknown option `allow-unrealted-histories'
usage: git push [<options>] [<repository> [<refspec>...]]

    -v, --[no-]verbose    be more verbose
    -q, --[no-]quiet      be more quiet
    --[no-]repo <repository>
                          repository
    --[no-]all            push all branches
    --[no-]branches       alias of --all
    --[no-]mirror         mirror all refs
    -d, --[no-]delete     delete refs
    --[no-]tags           push tags (can't be used with --all or --branches or --mirror)
    -n, --[no-]dry-run    dry run
    --[no-]porcelain      machine-readable output
    -f, --[no-]force      force updates
    --[no-]force-with-lease[=<refname>:<expect>]
                          require old value of ref to be at this value
    --[no-]force-if-includes
                          require remote updates to be integrated locally
    --[no-]recurse-submodules (check|on-demand|no)
                          control recursive pushing of submodules
    --[no-]thin           use thin pack
    --[no-]receive-pack <receive-pack>
                          receive pack program
    --[no-]exec <receive-pack>
                          receive pack program
    -u, --[no-]set-upstream
                          set upstream for git pull/status
    --[no-]progress       force progress reporting
    --[no-]prune          prune locally removed refs
    --no-verify           bypass pre-push hook
    --verify              opposite of --no-verify
    --[no-]follow-tags    push missing but relevant tags
    --[no-]signed[=(yes|no|if-asked)]
                          GPG sign the push
    --[no-]atomic         request atomic transaction on remote side
    -o, --[no-]push-option <server-specific>
                          option to transmit
    -4, --ipv4            use IPv4 addresses only
    -6, --ipv6            use IPv6 addresses only

==PS D:\md_files>== git pull --allow-unrelated-histories github main
From https://github.com/Helen115111/Helen115111.github.io
 * branch            main       -> FETCH_HEAD
fatal: Could not read from '.git/MERGE_MSG': No such file or directory
==PS D:\md_files>== git romote -v
git: 'romote' is not a git command. See 'git --help'.

The most similar command is
        remote
==PS D:\md_files>== git remote -v
github  https://github.com/Helen115111/Helen115111.github.io.git (fetch)
github  https://github.com/Helen115111/Helen115111.github.io.git (push)
PS D:\md_files>
 *  还原的历史记录 

PS D:\md_files> 
 *  还原的历史记录 

PS D:\md_files> 
 *  还原的历史记录 

==PS D:\md_files>== cd D:\my_vscode\notoriginal
==PS D:\my_vscode\notoriginal>== git clone https://github.com/Helen115111/first-contributions.git
Cloning into 'first-contributions'...
remote: Enumerating objects: 27453, done.
remote: Counting objects: 100% (560/560), done.
remote: Compressing objects: 100% (93/93), done.
remote: Total 27453 (delta 546), reused 468 (delta 467), pack-reused 26893 (from 4)
Receiving objects: 100% (27453/27453), 12.24 MiB | 86.00 KiB/s, done.
Resolving deltas: 100% (17739/17739), done.
PS D:\my_vscode\notoriginal> 
 *  还原的历史记录 

==PS D:\md_files>== git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Disable this message with "git config set advice.addEmptyPathspec false"
==PS D:\md_files>== ssh-keygen -p -f ~/.ssh/id_ed25519
~/.ssh/id_ed25519: No such file or directory

#修改密码

---

==PS D:\md_files>== ls -al ~/.ssh
Get-ChildItem : 找不到与参数名称“al”匹配的参数。

**unix风格命令，查看目录下的文件，powershell要用
Get-ChildItem -Force -Path "$env:USERPROFILE\.ssh"
或者
ls -Force ~/.ssh
或者
Get-ChildItem -Path ~/.ssh -Force**

所在位置 行:1 字符: 4
+ ls -al ~/.ssh
+    ~~~
    + CategoryInfo          : InvalidArgument: (:) [Get-ChildItem]，ParameterBindingException
    + FullyQualifiedErrorId : NamedParameterNotFound,Microsoft.PowerShell.Commands.GetChildItemCommand

==PS D:\md_files>== Get-ChildItem -Path ~/.ssh -Force


    目录: C:\Users\yli8i\.ssh

```
Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         2025/8/22     22:09            411 id_ed25519
-a----         2025/8/22     22:09             97 id_ed25519.pub
```

---

==PS D:\md_files>== ssh-keygen -t ed25519 -f ~/.ssh/id_ed25519
Generating public/private ed25519 key pair.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Saving key "~/.ssh/id_ed25519" failed: No such file or directory

**ssh-keygen -t ed25519 -f ~/.ssh/id_ed25519**：生成SSH密钥的命令，*keygen*是key generator的缩写，用于生成ssh密钥对，*-t ed25519*指定密钥类型，ed25519是密钥算法，*-f*代表filename，指定密钥文件的路径和文件名，

运行ssh-keygen，生成可以但是保存会失败，提示无文件或目录。生成密钥是不需要文件基础的，而保存对文件基础有要求，因此生成的操作正常进行了，saving key/保存失败了


---

==PS D:\md_files>== ssh-keygen -p -f $HOME\.ssh\id_ed25519
Key has comment 'yli8i3@163.com'
Enter new passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved with the new passphrase.

小写的p：-p的核心功能是更改密码，通过主参数＋辅助参数可以实现更多功能
-f：也是主参数，指定文件名和保存路径
comment：表示注释信息，等于房门钥匙上标记了门牌号

---


==PS D:\md_files>== git commit -m "关于新建ssh密钥的笔记“
[main c8a2c92] 关于新建ssh密钥的笔记
 3 files changed, 38 insertions(+), 9 deletions(-)
 create mode 100644 1.md
 create mode 100644 tw.md
==PS D:\md_files>== git status
On branch main
Your branch is ahead of 'github/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
==PS D:\md_files>== git push
fatal: unable to access 'https://github.com/Helen115111/Helen115111.github.io.git/': SSL certificate problem: unable to get local issuer certificate
==PS D:\md_files>== git remote set-url origin git@github.com:Helen115111/Helen115111.github.io.git
error: No such remote 'origin'

---

==PS D:\md_files>== git remote -v
github  https://github.com/Helen115111/Helen115111.github.io.git (fetch)
github  https://github.com/Helen115111/Helen115111.github.io.git (push)

git remote -v：显示当前仓库关联的远程仓库，一般双向的关联是能拉取能推送，但有时权限不允许就会出现单向的关联，也就是仅能推送或仅能拉取，因此两个方向上的关联是分开出现的

---

==PS D:\md_files>== git remote set-url github git@github.com:Helen115111/Helen115111.github.io.git       
**remote**：表示远程仓库的管理
**set-url**：表示修改网址
**github**：此处是自定义的仓库别名，并非关键字
**git@github.com:Helen115111/Helen115111.github.io.git**：ssh地址
这一段的作用是修改了远程仓库的url，替换为ssh地址

---

==PS D:\md_files> git push==
ssh: connect to host github.com port 22: Connection refused
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
==PS D:\md_files> ssh -T git@github.com==
ssh: connect to host github.com port 22: Connection refused
==PS D:\md_files> ssh -T git@github.com==
ssh: connect to host github.com port 22: Connection refused
==PS D:\md_files> git config --global http.sslVerify false==

---

==PS D:\md_files>== git push github main
ssh: connect to host github.com port 22: Connection refused
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

**git push github main**：将本地修改同步到远程服务器+远程仓库别名+要同步的本地分支的名称


---

==PS D:\md_files>== ssh -T git@github.com
ssh: connect to host github.com port 22: Connection refused


**ssh -T git@github.com**：检查 GitHub SSH 配置是否生效” 的标准测试命令，配置新的 SSH 密钥或遇到 git push 失败时可以进行故障排查
**ssh**：表示在执行ssh操作
**connect to host github.com**：表示正在进行的操作，即连接到GitHub服务器
**port 22**：ssh协议默认的端口22

---

PS D:\md_files> ls $HOME\.ssh -Force


    目录: C:\Users\yli8i\.ssh


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         2025/8/24      0:08             66 config
-a----         2025/8/23     23:36            464 id_ed25519
-a----         2025/8/22     22:09             97 id_ed25519.pub
-a----         2025/8/24      0:24            861 known_hosts
-a----         2025/8/24      0:23            103 known_hosts.old

ls $HOME\.ssh -Force 查看文件的正确写法
一些错误写法： ls -al ~/.ssh/
 ls -la ~/.ssh

==PS D:\md_files>== ls ~/.ssh


    目录: C:\Users\yli8i\.ssh

```
Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         2025/8/24      0:08             66 config.txt
-a----         2025/8/23     23:36            464 id_ed25519
-a----         2025/8/22     22:09             97 id_ed25519.pub
```
ls是 "list" 的缩写，核心功能是列出指定目录下的文件和文件夹,~/.ssh是文件目录

---

PS D:\md_files> mv ~/.ssh/config.txt ~/.ssh/config
  - 这个命令的作用是 将 .ssh 目录下名为 config.txt 的文件重命名为 config，原因是在记事本保存文件自带了后缀，无法识别，需要手动删掉，解决方法，去文件夹删和这个命令行都行
  - mv 是 Linux/macOS（或 Git Bash 等类 Unix 终端）中的 “移动 / 重命名” 命令，既可以移动文件位置，也可以直接重命名文件。
  - git bash和cmd，powershell都是终端，cmd功能比较基础，powershell更强大，git bash适用于Unix/Linux操作
  - ~/.ssh/config.txt 是原文件路径：~ 代表用户主目录，.ssh 是存放 SSH 配置的目录，config.txt 是带 .txt 后缀的原文件名。~/.ssh/config 是目标路径：表示将文件重命名为 config（去掉 .txt 后缀），仍放在在 .ssh 目录下。
  
---

- 读取文件内容，确认是否正确配置ssh规则以及配置文件是否存在
==PS D:\md_files>== cat ~/.ssh/config
Host github.com
  Hostname ssh.github.com
  Port 443
  User git
  
---

- 测试是否连接畅通
PS D:\md_files> ssh -T git@github.com
The authenticity of host '[ssh.github.com]:443 ([20.205.243.160]:443)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes                  
Warning: Permanently added '[ssh.github.com]:443' (ED25519) to the list of known hosts.
Enter passphrase for key 'C:\Users\yli8i/.ssh/id_ed25519': 
Hi Helen115111! You've successfully authenticated, but GitHub does not provide shell access.
PS D:\md_files> 

切换ssh跳过的密码是GitHub的账号密码，如果用ssh每次push都还要输密码，那是我们自己给密钥设的密码，想要省略这个密码要设置代理

cat ~/.ssh/id_ed25519.pub
查看公钥