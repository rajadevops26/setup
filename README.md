# DEVOPS CONFIGUARATION TOOLS BY R RAJENRA PRASAD :+1:
# GIT INSTALLATION STEPS
![logo](https://www.rosehosting.com/blog/wp-content/uploads/2014/05/how-to-install-and-set-up-git-on-ubuntu-14-04-lts-vps.jpg)
```
sudo -i
apt-get update
apt-get install git*

* * generate ssh key for authoticate permission to remote location * *
ssh-keygen -t rsa
enter-key
enter-key
enter-key
cd .ssh
cat id_rsa.pub
** copy id_rsa.pub key **
cat>>authorized_keys
** paste id_rsa.pub key into here **
ctrl+d
enter

mkdir gitpractice
cd gitpractice
git init
git config --global user.name "raja"
git config --global user.email "rajarani@love.com"
git remote -v
git remote add origin hhtps@github.com:loverajarani/devops.git
git remote -v

vi sample.txt
** i ** for insert mode
** ADDING CODE **
welcome to git

------------------->>esc:wq!

git status
git add sample.txt
git status
git commit -m "java code added"
git status
git push origin master
username
passwd

```
