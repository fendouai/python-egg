更新python egg
sudo su - root 
cd /home/zhangh/python-egg
拉取更新
git fetch
git merge origin/master
替换python egg包
cd /usr/lib/python2.6/site-packages
rm -rf mkdocs_bootstrap-0.1.1-py2.6.egg/
cd /home/zhangh/python-egg
cp -r  mkdocs_bootstrap-0.1.1-py2.6.egg/ /usr/lib/python2.6/site-packages/
rm -rf mkdocs-0.15.0.dev-py2.6.egg/
cd /home/zhangh/python-egg
cp -r mkdocs-0.15.0.dev-py2.6.egg/ /usr/lib/python2.6/site-packages/