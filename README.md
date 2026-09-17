# Pull Request Practice

In this activity, you will practice contributing to another person’s GitHub repository by creating a **pull request**.

A pull request asks the owner of a repository to review and merge your changes into the original project.

## What You Will Practice

- Forking a repository
- Cloning your fork
- Creating a Markdown file
- Staging and committing changes
- Pushing changes to GitHub
- Creating a pull request
- Responding to review comments

## Important Terms

### Fork

A fork is your own GitHub copy of another person’s repository.

### Pull Request

A pull request, also called a **PR**, is a request to have your changes reviewed and added to another repository.

### Merge

Merging accepts the proposed changes and combines them with the original repository.

> `git pull` brings changes from GitHub to your computer. A **pull request** asks someone to review and accept your changes.

## Your Contribution

You will create a Markdown file inside the `student-contributions` folder.

Name the file using your first and last name:

```text
firstname-lastname.md
```

For example:

```text
taylor-smith.md
```

Do not edit the example file or another student’s file.

## Required File Content

Use the following format:

```markdown
# Your Name

## Something I Have Learned About Git

Write two or three sentences explaining something you have learned about Git or GitHub.

## Helpful Git Command

`git status`

Explain what the command does and when someone might use it.
```

You may use a Git command other than `git status`.

# Instructions

## Step 1: Fork the Repository

1. Select **Fork** near the upper-right corner of this repository.
2. Keep the default repository name.
3. Select **Create fork**.
4. Make sure the username above the repository name is your GitHub username.

You now have your own copy of the repository.

## Step 2: Clone Your Fork

Make sure you are viewing your fork, not the instructor’s original repository.

1. Select the green **Code** button.
2. Choose **HTTPS**.
3. Copy the repository URL.
4. Open a terminal.
5. Run:

```bash
    git clone https://github.com/spilman6/pull-request-practice.git
```

Move into the repository:

```bash
cd pull-request-practice
```

Open the repository in Visual Studio Code:

```bash
code .
```

> Make sure you clone your fork. Do not clone the instructor’s original repository.

## Step 3: Create Your Contribution

1. Open the `student-contributions` folder.
2. Create a new Markdown file.
3. Name the file using your first and last name.
4. Add the required content.
5. Save the file.

Your file should be located at:

```text
student-contributions/firstname-lastname.md
```

Do not:

- Edit `README.md`
- Edit `example-student.md`
- Edit another student’s file
- Add unrelated files

## Step 4: Check Your Changes

Run:

```bash
git status
```

Your new file should be listed as an untracked file.

## Step 5: Stage Your Changes

Run:

```bash
git add .
```

Check the status again:

```bash
git status
```

Your file should now be staged and ready to commit.

## Step 6: Commit Your Changes

Create a commit with a descriptive message:

```bash
git commit -m "Add Firstname Lastname's contribution"
```

For example:

```bash
git commit -m "Add Taylor Smith's contribution"
```

## Step 7: Push Your Changes

Run:

```bash
git push
```

Your changes are now stored in your fork on GitHub. They have not been added to the instructor’s original repository yet.

## Step 8: Open a Pull Request

1. Return to your fork on GitHub.
2. Refresh the page.
3. Select **Contribute**.
4. Select **Open pull request**.

Before continuing, verify the following:

```text
Base repository: Instructor's repository
Base branch: main

Head repository: Your fork
Compare branch: main
```

- **Base** is where you want your changes to go.
- **Head** contains your proposed changes.

## Step 9: Review Your Changes

Before creating the pull request, review the changed files.

You should see only:

```text
student-contributions/firstname-lastname.md
```

If you see `README.md`, another student’s file, or unrelated changes, stop and ask for help.

## Step 10: Create the Pull Request

Use a descriptive title:

```text
Add Firstname Lastname's contribution
```

Add this description:

```markdown
## What I Added

I added my student contribution file.

## My Contribution Includes

- Something I learned about Git
- A helpful Git command
- An explanation of when to use the command
```

Select **Create pull request**.

## Responding to Review Comments

Your instructor may leave a comment or ask you to improve something.

If a change is requested:

1. Return to Visual Studio Code.
2. Update your file.
3. Save the file.
4. Run:

```bash
git status
git add .
git commit -m "Update my student contribution"
git push
```

Do not create another pull request.

Your existing pull request will update automatically when you push the new commit.

## Before Submitting

Make sure:

- Your file is inside `student-contributions`.
- Your filename includes your first and last name.
- You completed every required section.
- You changed only your own file.
- Your pull-request title clearly describes your contribution.
- You reviewed the **Files changed** section.
- You submitted the pull request to the instructor’s repository.

## Blackboard Submission

Submit:

- The URL of your pull request
- A screenshot showing your pull request
- Your answer to this question:

> What is the difference between `git pull` and a pull request?

## Workflow Summary

```text
Fork → Clone → Edit → Add → Commit → Push → Pull Request → Review → Merge
```
