# Github/Gitbash scripts and such 

# Setup Instructions
```
cd seanabrahamsen.com
# if there is not a venv folder
python -m venv venv
pip install -r requirements.txt

# when venv exists (or after last commands)
# run this every time new terminal is opened
source venv/Scripts/activate
```
# To install themes
```
git clone --recursive https://github.com/getpelican/pelican-themes ~/pelican-themes
pelican-themes --install ~/pelican-themes/attila --verbose

# to make easier for deployment the attila theme has been moved into the
themes/attila directory.
# make sure to add the following command into your conveyor deploy script

git submodule init

# to update theme to latest code if needed..
cd themes/attila
git checkout master
git pull
```
# How to run locally
```
# open two terminals and activate `venv` in both 
# with `source venv/Scripts/activate`
make regenerate
make serve
```
# To view locally
```
# http://localhost:8000/
```
# To upload to github
```
git add .
git commit -m 'notes for whatever added'
git push
```
# To make a files/directories
```
For directories:
mkdir path/path/dir
For files:
touch path/path/filename.md
```
# To remove files/directories
```
For file:
rm path/path/filename
For Directory:
rm -r path/path/dirname
```
# Symbol meanings
``` 
"~" This means I am in the domain or directory of users/seanDog
```
# To add a youtube video
```
Go to youtube video, click on "share", embeded code.
```

# Next level terminals or shells
```
Currently using Git Bash...
Others that might be better:
Hyper Shell
Commander
```
