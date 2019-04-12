
1. push to remote
    ``` git
    git push origin master
    git push -f origin master
    ```

2. overwrite all local files. Match local with remote
``` git
    git fetch origin
    git reset --hard origin/master
```

* save local files in a branch before overwritten

``` git
    git commit -a -m "Save local work before overwritten"
    git branch new_branch_name
```
* delete untracked local files from your current working tree if needed
``` git
    git clean -n  # show what will be deleted
    git clean -f  # delete untraced files
```
3. push to remote
   ``` git
   git push origin master
   ```

4. Set global user.name and user.email
   ``` git
   git config --global user.name "name here"
   git config --global user.email johndoe@email.com
   ```
5. List origins
   ``` git
   git config --list --show-origin
   git config --list
   ```
6. Add files to stage. 
   ```
   # stages all files in the git repository. Currently dir can be anywhere inside the repository
   git add -A

   # stage 0nly the files in the current working dir
   git add .
   ```
7. Add a remote
   ``` git
   git remote add origin https://github.com/user/repo.git
   git remote -v
   git remote show origin
   ```

