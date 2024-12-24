#### Step 1:
- Initialize the exercise using the below command:
```bash
git start merge-conflict

(OR)

git status next
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_start.png)

#### Step 2:
- Check the files present.
```bash
ls
```
- You can check the correct exercise from the branch name itself.

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_ls.png)

- Task instrutions.
```bash
cat README.md
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_task_instructions.png)

#### Step 3:
- Check the logs of the current merge-conflict branch.
```bash
git log --oneline
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_initial_log.png)

#### Step 4:
- List all the branches.
```bash
git branch
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_branch_list.png)

#### Step 5:
- Switch to another branch, another-piece-of-work.
```bash
git switch another-piece-of-work
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_initial_switch.png)

#### Step 6:
- Check the logs of the new branch and observe the commits.
```bash
git log --oneline
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_another_branch_log.png)

#### Step 7:
- Switch back to the merge-conflict branch in order to merge the changes into it from the another-piece-of-work branch.
```bash
git switch merge-conflict
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_switch_back.png)

- Now, merge the changes into the merge-conflict branch.
```bash
git merge another-piece-of-work
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_merge.png)

#### Step 8:
- There will be a merge conflict here.
- The file which has conflict will be opened in the respective editor.
- Resolve the changes accordingly.

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_file.png)

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_equation_file.png)

#### Step 9:
- Add the above modified file to the staging area.
```bash
git add equation.txt
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_add.png)

- Commit the respective changes.
```bash
git commit -m "Updated equation.txt"
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_commit.png)

- Now, all the conflicts were resolved and committed.

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_log_final.png)

#### Step 10:
- After the successful merging, verify the task.
```bash
git verify
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/merge_conflict_verify.png)