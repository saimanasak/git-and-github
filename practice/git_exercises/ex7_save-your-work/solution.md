#### Step 1:
- Initialize the exercise using the below command:
```bash
git start merge-conflict

(OR)

git status next
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/save_your_work_start.png)

#### Step 2:
- Check the files present.
```bash
ls
```
- You can check the correct exercise from the branch name itself.

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/save_your_work_ls.png)

- Task instrutions.
```bash
cat README.md
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/save_your_work_task_instructions.png)

#### Step 3:
- Save your current work using stashing.
```bash
git stash
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/save_your_work_stash.png)

#### Step 4:
- Remove the bug from the bug.txt file (Remove: THIS IS A BUG - remove the whole line to fix it. line)
- Commit the above changes.
```bash
git commit -am "Removed bug"
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/save_your_work_initial_commit.png)

#### Step 5:
- List all the stashes.
```bash
git stash list
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/save_your_work_stash_list.png)

#### Step 6:
- Apply the saved work.
```bash
git stash apply

(OR)

git stash apply stash@{0}
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/save_your_work_stash_apply.png)

#### Step 7:
- Modify the bug.txt file (Add: Finally, finished it! line)
- Commit the changes.
```bash
git commit -am "Updated bug.txt"
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/save_your_work_final_commit.png)

#### Step 8:
- Verify
```bash
git verify
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/save_your_work_verify.png)