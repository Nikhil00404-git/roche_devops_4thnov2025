# roche_devops_4thnov2025

### steps to verify 

```
humanfirmware@darwin  ~  ssh ashu@15.134.107.225
ashu@15.134.107.225's password: 
   ,     #_
   ~\_  ####_        Amazon Linux 2023
  ~~  \_#####\
  ~~     \###|
  ~~       \#/ ___   https://aws.amazon.com/linux/amazon-linux-2023
   ~~       V~' '->
    ~~~         /
      ~~._.   _/
         _/ _/
       _/m/'
Last login: Tue Nov  4 08:46:11 2025 from 103.97.242.236

[ashu@ip-172-31-5-155 ~]$ cat  ~/.config/code-server/config.yaml 
bind-addr: 0.0.0.0:8033
auth: password
password: 435456547657dfgdghfh
cert: false


[ashu@ip-172-31-5-155 ~]$ curl   ifconfig.me 
15.134.107.225[ashu@ip-172-31-5-155 ~]$ 
[ashu@ip-172-31-5-155 ~]$ 
[ashu@ip-172-31-5-155 ~]$ ls /home/
akshay  anjali  ashu  ec2-user  hitesh  ketan   rpradhan  shobhit  tithi   vijayp
amit    arpit   dev   gayt      kd25    nikhil  sdas      singh    vermah  viresh

```

## git repo branching 

<img src="br1.png">

### handling git repo branches 

```
[root@ip-172-31-5-155 ashu-roche-devops-code]# ls
README.md  ec2.tf  output.tf  providers.tf  terraform.tfstate  terraform.tfstate.backup
[root@ip-172-31-5-155 ashu-roche-devops-code]# 
[root@ip-172-31-5-155 ashu-roche-devops-code]# 
[root@ip-172-31-5-155 ashu-roche-devops-code]# git checkout  -b  dryrun-aws 
Switched to a new branch 'dryrun-aws'
[root@ip-172-31-5-155 ashu-roche-devops-code]# git branch 
* dryrun-aws
  master
[root@ip-172-31-5-155 ashu-roche-devops-code]# git  checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.
[root@ip-172-31-5-155 ashu-roche-devops-code]# git branch 
  dryrun-aws
* master
[root@ip-172-31-5-155 ashu-roche-devops-code]# git  switch  dryrun-aws 
Switched to branch 'dryrun-aws'
[root@ip-172-31-5-155 ashu-roche-devops-code]# git branch 
* dryrun-aws
  master
[root@ip-172-31-5-155 ashu-roche-devops-code]# 

```
### pushing code to non master branch 

```
188  git branch 
  189  git status 
  190  git add .
  191  git commit  -m "fixed ec2 tags and update output depends"
  192  history 
  193  git push origin  dryrun-aws 

```
