### Install Git
```
sudo apt install git git-lfs -y
```
### push flow
```
git init
git lfs track AAA
git add AAA
git add BBB
git commit -m "update"
git branch -m main
git remote add origin repo@url
git push origin main
```
