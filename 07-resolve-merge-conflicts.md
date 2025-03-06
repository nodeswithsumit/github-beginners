# Resolve Merge Conflicts

## Objective:
Learn how to resolve merge conflicts when merging branches.

## Steps:
1. Make conflicting changes in two branches:
    - In `main` branch, change a line in `hello.txt`.
    - In `new-feature` branch, change the same line in `hello.txt`.
2. Attempt to merge the branches:
    ```bash
    git checkout main
    git merge new-feature
    ```
3. Git will show a conflict in the `hello.txt` file.
4. Open the file, look for conflict markers (e.g., `<<<<<<<`, `=======`, `>>>>>>>`), and manually resolve the conflict.
5. After resolving, save the file and add the resolved file:
    ```bash
    git add hello.txt
    git commit -m "Resolved merge conflict"
    ```

## Outcome:
You have successfully resolved a merge conflict.
