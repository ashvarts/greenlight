# GitHub Copilot Instructions

## Git Commit Messages

When writing commit messages, always follow these two guides:

1. **Conventional Commits** (https://www.conventionalcommits.org/)
   - Use the format: `<type>[optional scope]: <description>`
   - Common types: `feat`, `fix`, `build`, `chore`, `ci`, `docs`, `style`, `refactor`, `perf`, `test`
   - Example: `feat: add user authentication`

2. **Chris Beams' Seven Rules** (https://cbea.ms/git-commit/)
   - Separate subject from body with a blank line
   - Limit the subject line to 50 characters
   - Capitalize the subject line (the description part after the type)
   - Do not end the subject line with a period
   - Use the imperative mood in the subject line
   - Wrap the body at 72 characters
   - Use the body to explain what and why vs. how

### Example Commit Message

```
build: remove indirect marker from httprouter dependency

The httprouter package is now being used directly in the codebase
(in routes.go for request routing), so it should no longer be marked
as an indirect dependency in go.mod.
```

3. Favor multiple commit messages in logically grouped hunks per commit that tell a story.
