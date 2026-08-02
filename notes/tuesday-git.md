# Tuesday Git Notes

These notes summarize the Git concepts covered during today's DevOps lab.

---

## Working Directory vs Staging vs History

Understanding these three areas is essential to using Git effectively.

### Working Directory
The **Working Directory** is where you create and edit files on your computer. Any changes made here are not yet tracked by Git until you stage them.

**Example**

```bash
echo "Hello, DevOps!" >> README.md
```

At this point, the change exists only in your working directory.

---

### Staging Area

The **Staging Area** (also called the **Index**) is where you prepare changes before creating a commit.

Stage a file:

```bash
git add README.md
```

You can think of the staging area as a shopping basket—you decide exactly which changes will be included in your next commit.

---

### Commit History

The **History** is a permanent record of your commits.

Create a commit:

```bash
git commit -m "docs: update README"
```

View previous commits:

```bash
git log --oneline
```

Every commit represents a snapshot of your project at a specific point in time.

---

## Branching Rules

Branches allow developers to work on features independently without affecting the main codebase.

### Good Practices

- Create one branch per feature or bug fix.
- Give branches meaningful names.
- Keep branches focused on a single task.
- Merge only after testing and review.
- Delete branches after they have been merged.

### Example

```bash
git switch -c feature/login-page
```

---

## Pull Request Expectations

A Pull Request (PR) is a request to merge your branch into another branch, usually `main`.

Before opening a PR:

- Ensure your code builds successfully.
- Run all tests.
- Write a clear description of your changes.
- Keep the PR small and focused.
- Request a review from another developer.
- Address review comments before merging.

A good pull request makes it easier for teammates to understand, review, and safely merge your work.

---

## Key Takeaways

- Changes begin in the **Working Directory**.
- Use **git add** to move changes to the **Staging Area**.
- Use **git commit** to save changes into **Git History**.
- Use **branches** to isolate work.
- Use **Pull Requests** to collaborate and maintain code quality.