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
CD CI Down to Upstream

The Docker way

1. aws ecr get-login-password --region eu-north-1 | docker login --username AWS --password-stdin 686255954747.dkr.ecr.eu-north-1.amazonaws.com
2. docker build -t 686255954747.dkr.ecr.eu-north-1.amazonaws.com/crossplane-blanketops-ecr-repository:latest
3. docker tag 686255954747.dkr.ecr.eu-north-1.amazonaws.com/crossplane-blanketops-ecr-repository:latest
4. docker push 686255954747.dkr.ecr.eu-north-1.amazonaws.com/crossplane-blanketops-ecr-repository:latest

From the dockerhub docs

1. docker build -t some-content-nginx .
2. docker run --name some-nginx -d -p 8081:80 some-content-nginx

Deploy To ECS Using Github Action

1. See .github/workflows/aws.yaml
```