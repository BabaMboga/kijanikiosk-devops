# Tuesday Git Notes

## Working Directory vs Staging vs History

- **Working Directory**: The area where you create and modify files on your local machine.
- **Staging Area**: A temporary area where you prepare changes before committing them using `git add`.
- **History**: The collection of commits stored in the Git repository, representing the project's version history.

## Branching Rules

- Create a new branch for each feature or bug fix.
- Use descriptive branch names (e.g., `feature/login`, `bugfix/navbar`).
- Keep branches focused on a single task.
- Merge branches only after they have been reviewed and tested.
- Delete branches after they have been successfully merged.

## Pull Request Expectations

- Ensure all tests pass before opening a pull request.
- Provide a clear title and description of the changes.
- Keep pull requests small and focused.
- Request at least one code review.
- Address reviewer feedback before merging.