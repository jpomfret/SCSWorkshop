# Lesson 6 - Clean up those branches

## Prerequisites

- Worked through the other lessons and left branches all over the place.

## Lesson

### Stage 1 - View our local branches

1. Checkout main

    ```bash
    git checkout main
    ```

2. View our local branches

    ```bash
    git branch -v
    ```

3. View branches in VSCode

    ![image](https://user-images.githubusercontent.com/981370/195087374-3644f25e-279b-492f-9e5a-ad1e0d4e81b8.png)


4. View branches that have been merged into main

    ```bash
    git branch --merged
    ```

5. Delete a single branch

    ```bash
    git branch -d addFriends
    ```

6. Delete all merged branches

    ```bash
    git branch --merged | ?{-not ($_ -like "*main")} | %{git branch -d $_.trim()}
    ```

    >https://gist.github.com/srkirkland/63ed5730da1bf607a4b3

### Stage 2 - Clean up GitHub Branches

1. Navigate to your GitHub Repo (e.g. www.github.com/jpomfret/SCSWorkshop)
2. Click branches (or navigate to e.g. www.github.com/jpomfret/SCSWorkshop/branches)
3. Delete any unneeded branches
