Step by step how to make an empty branch:

git checkout —orphan new_branch_name.


Make sure you are in the right directory before executing the following command: ls -la. | awk '{print $9}' | ...


git rm -rf .


touch new_file.


git add new_file.


git commit -m 'added first file in the new branch'


git push origin new_branch_name.
