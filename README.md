# BlanketOps Nginx Example

```
Typical Developer Workflow Process

1. Checkout new branch: git checkout -b feature/<branch name>, git checkout -b bugfix/<branch name>
2. Do Developer changes
3. When tested successfully and ready for submission, do git commit -m "<commit message, usually branch name"
4. Do git push to commit the changes in the branch to the remote repository.
5. Create a pull request to the branch develop if feature/, the release if bugfix/.
6. Merge Once Ready, branch policies and or deletion of branch to take place depending on branch policies.
```

```
GitHub process for Developement
```

```
CD CI Down to Upstream

The Docker way 

1. docker login -u <username>
2. Enter Docker Account Personal Access account as password
3. docker build -t <registry>/<username>/<repository>:<tag> .
4  docker push <registry>/<username>/<repository>:<tag>