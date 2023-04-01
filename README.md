# kodluyoruzilkrepo

## git clone
- Bu repo [kodluyoruz](https://www.kodluyoruz.org) eğitiminde oluşturduğumuz ***ilkrepo*** **githubda** oluşturup *clone* ettim sonra içine bir *index.html* ekleyeceğim.

- $ cd kodluyoruzilkrepo : git bashi kodluyoruz ilk repo klasörüne konumlandırdı

- vs code u açarak .md dosyası düzenlendi

## git add
- index.html i önce git add index.html deyip takibe aldım sonra modified ettim. note: dosyaları eklerken büyük küçük harflere dikkat et nasıl görünüyorsa bashe öyle yaz

```bash
seçkin@DESKTOP-V9MDHC8 MINGW64 ~/kodluyoruzilkrepo (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   index.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        modified:   index.html

```

- index.html içine yaptığım bir hatayı ekledim hata şuydu önce masaüstünde yeni klasör açıp git bash here dedikten sonsa git clone ettim sonra bu yeni klasörde git init yaptım dolayısıyla hem yeni klaörde hemde kodluyoruzilkrepo klasöründe .git olduğu için fatal submodule verdi  

```bash
git clone https://github.com/seckinkorkmaz/kodluyoruzilkrepo.git
```
#### code satırı oluşturma örneği
```javascript
 console.log{

 }
```
***

#### Lists

- li1
- li2
* li1
* li2
- li1 alt alta farklı semboller kullanınca listeleriayırıyor.

#### git add --all
```
seçkin@DESKTOP-V9MDHC8 MINGW64 ~/kodluyoruzilkrepo (main)
$ git add --all

seçkin@DESKTOP-V9MDHC8 MINGW64 ~/kodluyoruzilkrepo (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        new file:   index.html

```
#### git commit

```
$ git commit -m 'index.html eklendi ve git kullanımaşamaları readme.md de düzenlendi'
[main 5fb02f0] index.html eklendi ve git kullanımaşamaları readme.md de düzenlendi
 2 files changed, 62 insertions(+)
 create mode 100644 index.html

seçkin@DESKTOP-V9MDHC8 MINGW64 ~/kodluyoruzilkrepo (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

```
#### git log
#### gitk
#### git checkout <-commit adress->
#### git diff

## git branch

```
 git switch -c <-branch-name->
 Switched to a new branch 'new-branch'
 
 seçkin@DESKTOP-V9MDHC8 MINGW64 ~/kodluyoruzilkrepo (new-branch)
$ git branch -a
  main
* new-branch
  remotes/origin/HEAD -> origin/main
  remotes/origin/main

$ git push origin new-branch
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.65 KiB | 1.65 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'new-branch' on GitHub by visiting:
remote:      https://github.com/seckinkorkmaz/kodluyoruzilkrepo/pull/new/new-branch
remote:
To https://github.com/seckinkorkmaz/kodluyoruzilkrepo.git
 * [new branch]      new-branch -> new-branch

```
