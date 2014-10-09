manifest
========

Manifest for use with the [git repo tool](https://code.google.com/p/git-repo/).
All of my true fans will use this to easily interact with all of my repos. I'm
going to use it to make it easier to check the status of multiple repos.

```bash
mkdir artloder
cd artloder
curl https://storage.googleapis.com/git-repo-downloads/repo > repo
chmod a+x repo
./repo init -m manifest.xml -u https://github.com/artloder/manifest.git
./repo sync
./repo forall -c "pwd; git checkout master"
```
