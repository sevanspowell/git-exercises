# Git exercises

A series of exercises designed to improve your git-fu!

Feel free to ask questions by raising an issue on this repository.

Start by forking this repository.

<details>
  <summary>Clone your fork</summary>
  
  ```
  git clone https://github.com/<your-github-username-here>/git-exercises.git
  ```
</details>

<details>
  <summary>Show the list of branches</summary>
  
  ```
  git branch
  git branch --list
  ```
  
  ```
  * master
    my-cool-feature
    branch-a
    branch-b
  ```
</details>

<details>
  <summary>Switch to the "my-cool-feature" branch</summary>
  
  ```
  git checkout -b my-cool-feature
  ```
</details>

<details>
  <summary>Show some evidence you are on the "my-cool-feature" branch</summary>
  
  ```
  git branch
  git status
  ```
</details>

<details>
  <summary>View the difference between "my-cool-feature" branch and master</summary>
  
  ```
  git diff master...my-cool-feature
  ```
</details>

<details>
  <summary>View the difference between "my-cool-feature" branch and the remote master</summary>
  
  ```
  git diff origin/master...my-cool-feature
  ```
</details>

<details>
  <summary>View the history of the "my-cool-feature" branch</summary>
  
  ```
  git log
  ```
</details>

<details>
  <summary>View only the history that the "my-cool-feature" branch adds</summary>
  
  ```
  git log master...my-cool-feature
  ```
</details>

<details>
  <summary>Create a new branch called "my-branch"</summary>
  
  ```
  git checkout -b my-branch
  ```
</details>

<details>
  <summary>Do some work on "my-branch" and commit it</summary>
  
  ```
  echo "Hello world!" > fileA.c
  git add fileA.c
  git commit -m "My new file"
  ```
</details>

<details>
  <summary>Create a new branch "branch-c", based off master, and merge "branch-a" into it</summary>

  ```
  git checkout master
  git checkout -b branch-c
  git merge branch-a
  ```
</details>

<details>
  <summary>Show what "branch-a" changed</summary>

  ```
  git diff master...branch-a
  ```
</details>

<details>
  <summary>Also merge "branch-b" into "branch-c"</summary>

  ```
  git checkout branch-c
  git merge branch-b
  git status
  # Use text editor to resolve conflict, choosing version you like better
  git commit
  ```
</details>
