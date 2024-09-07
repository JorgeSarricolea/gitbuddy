**Prompt:**

Hello! I need your help to generate a Conventional Commit message. Please follow these guidelines:

### 1. **Commit Message Structure:**

- **First line**: Provide a commit type, optional scope, and a brief description of the change.

  - **Type**: Choose from the following based on the nature of the change:
    - `feat` (for new features or functionalities)
    - `fix` (for bug fixes)
    - `refactor` (for changes in code structure without altering functionality)
    - `style` (for code formatting changes)
    - `docs` (for documentation updates)
    - `test` (for test additions or updates)
    - `chore` (for maintenance tasks or trivial updates)
  - **Scope** (optional): Mention the part of the codebase affected, enclosed in parentheses (e.g., `feat(auth)`).
  - **Short description**: A concise description of the change, in present tense, no longer than 72 characters.

- **Second line**: Leave this line blank to separate the subject from the details.

- **Third line onwards**: If needed, add a detailed explanation of the change. This should be indented by four spaces and include:
  - Why the change was necessary.
  - What was done in detail.
  - How this affects the codebase.

### 2. **Examples:**

#### Example 1: Adding a Feature

```
feat(auth): add JWT authentication for secure routes

    - Implemented JWT-based authentication to secure routes.
    - Added middleware for token validation before route access.
    - Updated login and signup endpoints to handle token issuance.
```

#### Example 2: Fixing a Bug

```
fix(login): correct email validation issue

    - Fixed validation issue where email addresses were not properly checked.
    - Added tests to ensure email validation works as expected.
```

#### Example 3: Refactoring Code

```
refactor(user-service): enhance user data processing

    - Refactored user data handling into separate helper functions.
    - Improved code readability and maintainability.
```

#### Example 4: Updating Styles

```
style(header): adjust header padding and margins

    - Fixed padding and margins in the header component.
    - Ensured header is responsive and looks correct on mobile devices.
```

#### Example 5: Documentation Update

```
docs(readme): update setup instructions and examples

    - Added Docker setup instructions to the README.
    - Clarified example usage and corrected typos.
```

### 3. **Detailed Instructions:**

- Start with the commit type and, if applicable, a scope in parentheses.
- The short description should clearly describe what was changed and be within 72 characters.
- Use the third section for additional details if necessary, explaining the why and how of the change.
- Write in present tense and avoid passive voice.
- Ensure proper capitalization and punctuation.

### 4. **Additional Notes:**

- Do **not** include `git commit -m`. Provide only the commit message text.
- Avoid phrases like "this commit does" or "in this commit."
- Be precise and specific to ensure clarity.

### 5. **Language Output\_:**

- Always write the Conventional Commit in English.