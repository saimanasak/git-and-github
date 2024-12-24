#### Step 1:
- Initialize the exercise using the below command:
```bash
git start ignore-them

(OR)

git status next
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/ignore_them_start.png)

#### Step 2:
- Check the files present.
```bash
ls
```
- You can check the correct exercise from the branch name itself.

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/ignore_them_ls.png)

- Instructions of the task.
```bash
cat README.md
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/ignore_them_task_instructions.png)

#### Step 3:
- Check the status of the files.
```bash
git status
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/ignore_them_status_initial.png)

#### Step 4:
- Create a file named **.gitignore**
```bash
touch .gitignore
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/ignore_them_touch.png)

- Add the below content in the file. the list of files that are to be ignored by Git.
```bash
vi .gitignore

=========================

File Content:
*.exe
*.o
*.jar
libraries/
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/ignore_them_cat.png)

#### Step 5:
- Add the .gitignore file to the staging area.
```bash
git add .gitignore
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/ignore_them_add.png)

- Commit the .gitignore file from the staging area.
```bash
git commit -m "Added .gitignore file"
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/ignore_them_commit.png)

- Now check the status of the files, the files which are untracked previously were ignored.
```bash
git status
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/ignore_them_status.png)

#### Step 6:
- Verify the above steps.
```bash
git verify
```

![screenshot](https://github.com/saimanasak/git-and-github/blob/main/practice/git_exercises/assets/ignore_them_verify.png)