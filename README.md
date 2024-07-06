# Work with GIT for Developers

## How to start New Project

Make directory for new project

```bash
mkdir new_project
cd new_project
```

Initialize git repository

```bash
git init
```

Create README.md and .gitignore files

```bash
touch README.md
touch .gitignore
```

Commit files

```bash
git add .
git commit -m "Initial commit"
```

Create `development` branch

```bash
git checkout -b development
```

Add remote repository. _Use your repository URL_

```bash
git remote add origin https://github.com/brokerUA/devops101-w2-m2.git
```

Push `development` branch to remote repository

```bash
git push origin development
```

## Workflow

1. Create a new branch:

```bash
git checkout -b feature/your-feature
```

2. Make changes to the code.
3. Commit changes:

```bash
git add .
git commit -m "Your message"
```

4. Push changes:

```bash
git push origin feature/your-feature
```

5. Move changes to `development` branch:

```bash
git checkout development
git pull origin development
git merge feature/your-feature
git push origin development
```

6. Create a pull request to `main` branch on GitHub.
7. Merge the pull request.
8. Delete the branch:

```bash
git branch -d feature/your-feature
```
