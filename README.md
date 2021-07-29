## Git-tutorial

By this youtube channel, I can fully understand git and using github

[Youtube link](https://www.youtube.com/watch?v=MFJIOqxK6k8&list=PLRx0vPvlEmdD5FLIdwTM4mKBgyjv4no81&index=11)

### Before we start
  * working directory : your computer folder
  * staging area : files that are going to be a part of the next commit
  * local repo : your computer repo
  * remote repo : Github

  working dir -> staging area -> local repo -> remote repo

### Git fundamental
1. make a repo files

2. git config global user.name JustCal1MeLee

   git config global user.email ~~
   
   --> to make global ID
   
3. make git folder in your computer(also download git)

   cd : change directory
   
   after changing directory
   
   git clone https://~
   
   git pull : download all the files (remote repo -> work dir)

4. after changing directory

   git add . : All of file into your staging area 
   
   git add files.py : files.py into your staging area
   
   git commit -m "comment" : comment + into your local repo
   
   git push : into your remote repo

5. after git add or commit 

   git status : you can find what kinds of file or what kind of stage
   
   git reset : local repo -> staging area
   
   git checkout --test.py : change in orignal version

### git log
  git log shows your commit history to check the hash number
  
  And also you can revise or delete the history
  
  when you **enter** then, past history is shown 
  
  when you push **q** then, you can get out of git log
  
  1. git log --stat : how many lines are inserted
  2. git log -p -3 : explain the log in top 3
  3. git log --pretty=oneline: explain the log in oneline for fast-looking

  4. git reset --hard hash_number : reset and delete history
  5. git reset --soft hash_number : reset but not delete
  6. git push -f : There is an error in just git push so you push it by force
  7. git commit rebase -i HEAD ~3(or hash number)


        Revision : revise the word **pick** -> **reword** and simply change your comment
        
        Deletion : revise the word **pick** -> **drop**

### git branch

1. git branch : find branch in git
2. git branch develop : make 'develop' branch 
3. git checkout develop : transfer to develop branch


   git checkout main : main branch
4. git merge develop : merge it (make sure to use at main branch)
   if error just go to your code and revise it and **git add**

5. git branch -d develop : remove develop branch

### git remote 

**origin** is original repository 

1. git remote : repository name
2. git remote show origin(or other repo) : explain repo 
3. git remote add test(repo's name) https://... : save at test repo
4. git remote -v : show repo
5. git remote rename test temp: name(test -> temp)
6. git remote rm temp : delete temp repo 

### when you need zip file for your coding program
  git archive —format=zip master -o Master.zip 
  
  it will help you bring out.

### cf)

소스코드 블록은 다음과 같이 작성가능하다

```c
#include <studio.h>

int main(void){
  printf("hello world");
  return 0;
}
```

순서없는 목록은 다음과 같이 작성가능하다
* git tutorial
  * git clone
  * git pull
  * git commit
    * git commit 1)

인용구문은 다음과 같이 작성가능하다.
> '할수 있다'고 말하다 보면, 결국 실천하게 된다 - 사이먼 쿠퍼-

테이블은 다음과 같이 작성가능하다.

이름|영어|정보|수학
---|---|---|---|
이찬혁|98|96|99|

강조하는 법
**치킨** 먹으면 ~~살쪄!~~
