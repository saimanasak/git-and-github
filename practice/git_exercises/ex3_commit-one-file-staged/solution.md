#### Step 1:
- Initialize the exercise using the below command:
```bash
git start commit-one-file-staged

(OR)

git status next
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/commit_one_file_staged_next.png)

#### Step 2:
- Check the files present.
```bash
ls
```
- You can check the correct exercise from the branch name itself.

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/commit_one_file_staged_ls.png)

#### Step 3:
- Check the status of the files.
```bash
git status
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/commit_one_file_staged_status_initial.png)

#### Step 4:
- Commit only one file from the staging area/tracked files.
```bash
git commit -m "Added B.txt file" B.txt
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/commit_one_file_staged_commit_B_file.png)

- Now check the status of the files
```bash
git status
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/commit_one_file_staged_status.png)

#### Step 5:
- Verify the above steps.
```bash
git verify
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/commit_one_file_staged_verify.png)