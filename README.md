# learning-git

```
o--->o------------>o(master)
     |
     o------>o(your branch)
```
       
Step 1: git checkout master 

Step 2: (Đang ở tại nhánh master) git pull

Step 3: git checkout add

Step 4: (đang ở nhánh add) git rebase master

Exception: Xuất hiện conflict

      Step 4: Mở code lên sửa conflick : có dạng như sau 
 
      
      <<<<<<< HEAD
      
      third 
      
      =======
      
      branch 1 add third 
      
      >>>>>>> branch1

      
      giữ nguyên 2 dòng 12 và 16 hoặc chọn 1 trong 2 dòng tùy muốn.
      
      result : (maybe) : 
      
      
      
      third
      
      branch 1 add third 
      
      
      
   Step 5: Lúc này đã sửa xong conflict 
 
       ```
       $ git add .
       ```
  Step 6: $ git rebase --continue
  
  
  Step 7: git push origin -f add 
  

##Complete
  
#Không xuất hiện conflict :
 ```
 git rebase --continue 
 
 git push origin -f add 
 
 ```
