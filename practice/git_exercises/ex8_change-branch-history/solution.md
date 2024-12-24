#### Step 1:
- Initialize the exercise using the below command:
```bash
git start change-branch-history

(OR)

git status next
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/change_branch_history_start.png)

#### Step 2:
- Check the files present.
```bash
ls
```
- You can check the correct exercise from the branch name itself.

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/change_branch_history_ls.png)

- Task instrutions.
```bash
cat README.md
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/change_branch_history_task_instructions.png)

#### Step 3:
- Check the logs of the current, change-branch-history branch.
```bash
git log --oneline
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/change_branch_history_initial_log.png)

#### Step 4:
- Check the list of the branches.
```bash
git branch
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/change_branch_history_branch_list.png)

#### Step 5: 
- Rebase will reapply the commits from change-branch-history (commit B) on top of hot-bugfix, which includes commit C.
```bash
git rebase hot-bugfix
```
- When you are rebasing make sure to stay on the change-branch-history branch.

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/change_branch_history_rebase.png)

#### Step 6:
- Check the logs of the change-branch-history branch.
```bash
git log --oneline
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/change_branch_history_final_log.png)

#### Step 7:
- Check the logs of the hot-bugfix branch as well and observe the commits.
```bash
git log --oneline
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/change_branch_history_bugfix_logs.png)

#### Step 8:
- Verify the above steps.
```bash
git verify
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/change_branch_history_verify.png)