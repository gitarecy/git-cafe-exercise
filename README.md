# git-cafe-exercise

## Bundle 5 
### Exerecise 2 

```bash

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop (main)
$ git clone https://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@github.com/gitarecy/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (14/14), done.
remote: Compressing objects: 100% (10/10), done.
remote: Total 107 (delta 5), reused 4 (delta 4), pack-reused 93
Receiving objects: 100% (107/107), 1.95 MiB | 362.00 KiB/s, done.
Resolving deltas: 100% (5/5), done.

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop (main)
$ cd git-cafe-exercise/

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (main)
$ git config --global user.name 'gitarecy'

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (main)
$ git config --global user.email 'gitarecynthia@gmail.com'

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (main)
$ ls
README.md  css/     index-1.html  index-3.html  index.html
bat/       images/  index-2.html  index-4.html  js/

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (main)
$ vi index.html

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (main)
$ git add .

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (main)
$ git commit -m 'updates on index'
[main 9ae8ab9] updates on index
 1 file changed, 2 insertions(+), 2 deletions(-)

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 322 bytes | 322.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/gitarecy/git-cafe-exercise.git
   d1d3f9c..9ae8ab9  main -> main
```

## Bundle 6 
### Exercise 1

```bash

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (main)
$ git checkout -b ft/menu
Switched to a new branch 'ft/menu'

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/menu)
$ vi menu.html

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/menu)
$ git add .
warning: in the working copy of 'menu.html', LF will be replaced by CRLF the next time Git touches it

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/menu)
$ git commit -m 'menu page '
[ft/menu 4291aaa] menu page
 1 file changed, 17 insertions(+)
 create mode 100644 menu.html

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/menu)
$ git push origin ft/menu
Enumerating objects: 113, done.
Counting objects: 100% (113/113), done.
Delta compression using up to 8 threads
Compressing objects: 100% (106/106), done.
Writing objects: 100% (113/113), 1.95 MiB | 1.17 MiB/s, done.
Total 113 (delta 8), reused 105 (delta 5), pack-reused 0
remote: Resolving deltas: 100% (8/8), done.
remote:
remote: Create a pull request for 'ft/menu' on GitHub by visiting:
remote:      https://github.com/gitarecy/git-cafe-exercise/pull/new/ft/menu
remote:
To https://github.com/gitarecy/git-cafe-exercise.git
 * [new branch]      ft/menu -> ft/menu
```
### Exercise 2 
```bash

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/menu)
$ git checkout -b ft/bugfix
Switched to a new branch 'ft/bugfix'

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/bugfix)
$ ls
README.md  css/     index-1.html  index-3.html  index.html  menu.html
bat/       images/  index-2.html  index-4.html  js/

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/bugfix)
$ mv index-4.html contact.html

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/bugfix)
$ ls
README.md  contact.html  images/       index-2.html  index.html  menu.html
bat/       css/          index-1.html  index-3.html  js/

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/bugfix)
$ vi contact.html

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/bugfix)
$ git add .

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/bugfix)
$ git commit -m 'rename index4 to contact'
[ft/bugfix f8ff46e] rename index4 to contact
 1 file changed, 203 insertions(+), 203 deletions(-)
 rename index-4.html => contact.html (97%)

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/bugfix)
$ git push origin ft/bugfix
fatal: User canceled device code authentication


LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/bugfix)
$ git push origin ft/bugfix
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 2.49 KiB | 1.25 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bugfix' on GitHub by visiting:
remote:      https://github.com/gitarecy/git-cafe-exercise/pull/new/ft/bugfix
remote:
To https://github.com/gitarecy/git-cafe-exercise.git
 * [new branch]      ft/bugfix -> ft/bugfix
```

### Exercise 3
```bash

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (main)
$ git checkout -b ft/hotfix
Switched to a new branch 'ft/hotfix'

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/hotfix)
$ ls
README.md  css/     index-1.html  index-3.html  index.html
bat/       images/  index-2.html  index-4.html  js/

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/hotfix)
$ vi index-4.html

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/hotfix)
$ git add .

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/hotfix)
$ git commit -m 'change telephone on index 4'
[ft/hotfix cc6825e] change telephone on index 4
 1 file changed, 2 insertions(+), 2 deletions(-)

LENOVO@DESKTOP-5GQ3HIK MINGW64 ~/Desktop/git-cafe-exercise (ft/hotfix)
$ git push origin ft/hotfix
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 303 bytes | 151.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/hotfix' on GitHub by visiting:
remote:      https://github.com/gitarecy/git-cafe-exercise/pull/new/ft/hotfix
remote:
To https://github.com/gitarecy/git-cafe-exercise.git
 * [new branch]      ft/hotfix -> ft/hotfix
```
