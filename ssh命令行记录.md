
PS D:\md_files> git remote -v
github  https://github.com/Helen115111/Helen115111.github.io.git (fetch)
github  https://github.com/Helen115111/Helen115111.github.io.git (push)
PS D:\md_files> git branch
* main
PS D:\md_files> git branch -r
  github/HEAD -> github/main
  github/main
PS D:\md_files> git branch --set-upstream-to=github/main main
branch 'main' set up to track 'github/main'.
PS D:\md_files>
 *  还原的历史记录 

PS D:\md_files> git remote -v
github  https://github.com/Helen115111/Helen115111.github.io.git (fetch)
github  https://github.com/Helen115111/Helen115111.github.io.git (push)
PS D:\md_files> git pull origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS D:\md_files> git remote -v
github  https://github.com/Helen115111/Helen115111.github.io.git (fetch)
github  https://github.com/Helen115111/Helen115111.github.io.git (push)
PS D:\md_files> git push -u github main --allow-unrealted-histories
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

PS D:\md_files> git pull --allow-unrelated-histories github main
From https://github.com/Helen115111/Helen115111.github.io
 * branch            main       -> FETCH_HEAD
fatal: Could not read from '.git/MERGE_MSG': No such file or directory
PS D:\md_files> git romote -v
git: 'romote' is not a git command. See 'git --help'.

The most similar command is
        remote
PS D:\md_files> git remote -v
github  https://github.com/Helen115111/Helen115111.github.io.git (fetch)
github  https://github.com/Helen115111/Helen115111.github.io.git (push)
PS D:\md_files>
 *  还原的历史记录 

PS D:\md_files> 
 *  还原的历史记录 

PS D:\md_files> 
 *  还原的历史记录 

PS D:\md_files> cd D:\my_vscode\notoriginal
PS D:\my_vscode\notoriginal> git clone https://github.com/Helen115111/first-contributions.git
Cloning into 'first-contributions'...
remote: Enumerating objects: 27453, done.
remote: Counting objects: 100% (560/560), done.
remote: Compressing objects: 100% (93/93), done.
remote: Total 27453 (delta 546), reused 468 (delta 467), pack-reused 26893 (from 4)
Receiving objects: 100% (27453/27453), 12.24 MiB | 86.00 KiB/s, done.
Resolving deltas: 100% (17739/17739), done.
PS D:\my_vscode\notoriginal> 
 *  还原的历史记录 

PS D:\md_files> git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Disable this message with "git config set advice.addEmptyPathspec false"
PS D:\md_files> ssh-keygen -p -f ~/.ssh/id_ed25519
~/.ssh/id_ed25519: No such file or directory
PS D:\md_files> ssh-keygen -p -f ~/.ssh/id_ed25519
~/.ssh/id_ed25519: No such file or directory
PS D:\md_files> ssh-keygen -p -f ~/.ssh/id_ed25519
~/.ssh/id_ed25519: No such file or directory
PS D:\md_files> ls -al ~/.ssh
Get-ChildItem : 找不到与参数名称“al”匹配的参数。
所在位置 行:1 字符: 4
+ ls -al ~/.ssh
+    ~~~
    + CategoryInfo          : InvalidArgument: (:) [Get-ChildItem]，ParameterBindingException
    + FullyQualifiedErrorId : NamedParameterNotFound,Microsoft.PowerShell.Commands.GetChildItemCommand

PS D:\md_files> Get-ChildItem -Path ~/.ssh -Force


    目录: C:\Users\yli8i\.ssh


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         2025/8/22     22:09            411 id_ed25519
-a----         2025/8/22     22:09             97 id_ed25519.pub


PS D:\md_files> ssh-keygen -t ed25519 -f ~/.ssh/id_ed25519
Generating public/private ed25519 key pair.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Saving key "~/.ssh/id_ed25519" failed: No such file or directory
PS D:\md_files> ssh-keygen -p -f $HOME\.ssh\id_ed25519
Key has comment 'yli8i3@163.com'
Enter new passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved with the new passphrase.
PS D:\md_files> git add
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Disable this message with "git config set advice.addEmptyPathspec false"
PS D:\md_files> git add .
PS D:\md_files> git commit -m "关于新建ssh密钥的笔记“
[main c8a2c92] 关于新建ssh密钥的笔记
 3 files changed, 38 insertions(+), 9 deletions(-)
 create mode 100644 1.md
 create mode 100644 tw.md
PS D:\md_files> git status
On branch main
Your branch is ahead of 'github/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS D:\md_files> git push
fatal: unable to access 'https://github.com/Helen115111/Helen115111.github.io.git/': SSL certificate problem: unable to get local issuer certificate
PS D:\md_files> git remote set-url origin git@github.com:Helen115111/Helen115111.github.io.git
error: No such remote 'origin'
PS D:\md_files> git remote -v
github  https://github.com/Helen115111/Helen115111.github.io.git (fetch)
github  https://github.com/Helen115111/Helen115111.github.io.git (push)
PS D:\md_files> git remote set-url github git@github.com:Helen115111/Helen115111.github.io.git                                              
PS D:\md_files> git push
ssh: connect to host github.com port 22: Connection refused
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS D:\md_files> ssh -T git@github.com
ssh: connect to host github.com port 22: Connection refused
PS D:\md_files> ssh -T git@github.com
ssh: connect to host github.com port 22: Connection refused
PS D:\md_files> git config --global http.sslVerify false
PS D:\md_files> git push github main
ssh: connect to host github.com port 22: Connection refused
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS D:\md_files> ssh -T git@github.com
ssh: connect to host github.com port 22: Connection refused
PS D:\md_files> ls ~/.ssh


    目录: C:\Users\yli8i\.ssh


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         2025/8/24      0:08             66 config.txt
-a----         2025/8/23     23:36            464 id_ed25519
-a----         2025/8/22     22:09             97 id_ed25519.pub


PS D:\md_files> mv ~/.ssh/config.txt ~/.ssh/config
PS D:\md_files> cat ~/.ssh/config
Host github.com
  Hostname ssh.github.com
  Port 443
  User git
PS D:\md_files> ssh -T git@github.com
The authenticity of host '[ssh.github.com]:443 ([20.205.243.160]:443)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes                  
Warning: Permanently added '[ssh.github.com]:443' (ED25519) to the list of known hosts.
Enter passphrase for key 'C:\Users\yli8i/.ssh/id_ed25519': 
Hi Helen115111! You've successfully authenticated, but GitHub does not provide shell access.
PS D:\md_files> 