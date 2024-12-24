#### Step 1:
- Initialize the exercise using the below command:
```bash
git start chase-branch

(OR)

git status next
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/chase_branch_start.png)

#### Step 2:
- Check the files present.
```bash
ls
```
- You can check the correct exercise from the branch name itself.

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/chase_branch_ls.png)

- Task instrutions.
```bash
cat README.md
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/chase_branch_task_instructions.png)

#### Step 3:
- Check the logs of the current, chase-branch branch.
```bash
git log --oneline
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/chase_branch_log_initial.png)

#### Step 4:
- Check the list of the branches.
```bash
git branch
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/chase_branch_branch_list.png)

#### Step 5: 
- Switch to the escaped branch.
```bash
git switch escaped
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/chase_branch_switch_escaped.png)

#### Step 6:
- Check the logs of the escaped branch.
```bash
git log --oneline
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/chase_branch_escaped_log_initial.png)

#### Step 6:
- Here,
    - Source Branch: escaped
    - Destination Branch: chase-branch
- So, in order to make the chase-branch point to the same commit as the escaped branch.
- Switch back to the destination branch, chase-branch.
```bash
git switch chase-branch
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/chase_branch_switch_back.png)

- Now, merge the escaped branch to the chase-branch branch.
```bash
git merge escaped
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/chase_branch_merge.png)

#### Step 7:
- Check the logs of the chase-branch branch.
```bash
git log --oneline
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/chase_branch_log_final.png)

#### Step 8:
- Verify the above steps.
```bash
git verify
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/chase_branch_verify.png)