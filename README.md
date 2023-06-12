# how-to
how-to instructions for anything git related

1. find repositories that are using git LFS
2. git clone repositories locally
3. remove hooks `git lfs uninstall`
4. list all lfs files `git lfs ls-files`
5. on web browser version of git repository, delete contents in `.gitattributes` file. Do not delete the file
6. Do the following git CLI instructions
```git lfs untrack '<pattern>' (in my case, all files "*.*")
git add --renormalize .
git commit -m 'Restore file contents that were previously in LFS' 
```
7. `git lfs ls-files` again to check if lfs files all removed
8. Check billings if any change in usage, still no change, fetch, pull, add, commit, push. 
9. Then delete repository, and create new repository with different name (can change name back to previous name later)
10. copy contents into new repository using local computer
11. git add ., git commit, git push
12. check billings again - should change
