 git --version
git version 2.56.0.windows.4

git config --global user.name "Benaya"   
>> git config --global user.email "benayayoyada34@gmail.com"
PS C:\Users\benay\OneDrive\Desktop\latihan-git> git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=schannel
core.autocrlf=true
core.fscache=true

git init                            
Initialized empty Git repository in C:/Users/benay/OneDrive/Desktop/latihan-git/.git/

 git add .
PS C:\Users\benay\OneDrive\Desktop\latihan-git> git commit -m "ini commit pertama ku dari benaya"
[master (root-commit) 5724852] ini commit pertama ku dari benaya
 2 files changed, 12 insertions(+)
 create mode 100644 README.md
 create mode 100644 index.html
PS C:\Users\benay\OneDrive\Desktop\latihan-git> git remote add origin https://github.com/mausukses/hello-world.git
PS C:\Users\benay\OneDrive\Desktop\latihan-git> git push -u  origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 490 bytes | 163.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/mausukses/hello-world.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'. brian gantenga