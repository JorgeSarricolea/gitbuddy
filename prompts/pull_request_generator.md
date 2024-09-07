### Prompt

Hello! I need your help to generate a Pull Request (PR) message based on the provided git log of commits. Please follow these guidelines and generate the output in separate sections: one for the title and one for the content. Additionally, provide the title in a bash-friendly format only.

### 1. **Initial Response**

Please confirm that you understand the request and that you are waiting for the git log of commits.

### 2. **Input Format:**

Please provide the `git log` of your commits. Example:

```
commit af1fb5e4a0c94dd60ee20d5804f8fcb241142ae9 (HEAD -> main, origin/main)
Author: Jorge Sarricolea <jjorgesarricolea18@email.com>
Date:   Sat Sep 7 04:41:07 2024 -0600

    refactor(script): update commit process to use nano editor

        - Changed commit procedure to open the "nano" editor for writing commit messages.
        - Updated workflow to include commit editing in "nano" followed by "pull" and "push" commands.
        - Improved clarity and consistency in the commit process.

commit 36a1b8d7b6d3160d9a4ebc18bf347ef5bc5bd315
Author: Jorge Sarricolea <jjorgesarricolea18@email.com>
Date:   Sat Sep 7 04:23:33 2024 -0600

    feat: add prompt template for generating Conventional Commits in ChatGPT

        - Created a prompt template for generating Conventional Commit messages in natural language.
        - Ensured the template includes guidelines for commit structure, examples, and detailed instructions.
        - Added notes on language and formatting requirements to maintain consistency.

commit 3785f1a68e8cfcacdbcd75e67caa3396ce1f7e32
Author: Jorge Sarricolea <jjorgesarricolea18@email.com>
Date:   Sat Sep 7 01:47:01 2024 -0600

    feat: implemented the main script for the Git Buddy program
```

### 3. **Output Sections:**

#### Title

Generate a concise and descriptive title for the PR based on the `git log`. The title should summarize the main change and include the appropriate category in square brackets. Provide the title in bash-friendly format only.

Example format:

```bash
[Feature] Implement Git Buddy Script, Add Commit Prompt Template, and Update Commit Process
```

#### Content

Generate the detailed content for the PR based on the `git log`. The content should include the following sections:

```
## Context
Describe the issue or need that this PR addresses. Include any relevant background information.

## Changes
- List the main changes made in the PR, based on the `git log`. Be specific about what was done.

## How to Test
1. Provide step-by-step instructions for testing the changes. Include steps to verify that the changes work as expected.

## Related Issues
- [Ticket]()
```

### Example Execution

**Bash-friendly Title:**

```bash
[Feature] Implement Git Buddy Script, Add Commit Prompt Template, and Update Commit Process
```

**Content:**

```
## Context
This PR introduces a series of updates to the Git Buddy program and refines the commit process. The changes include a new main script for the Git Buddy program and an updated commit workflow that utilizes the "nano" editor for improved commit message writing.

## Changes
- Implemented the main script for the Git Buddy program, adding core functionality.
- Updated the commit process to use the "nano" editor for writing commit messages, enhancing clarity and consistency.
- Created a prompt template for generating Conventional Commit messages in ChatGPT, including guidelines, examples, and detailed instructions.

## How to Test
1. Pull the branch and test the Git Buddy program to ensure the main script is functioning as expected.
2. Verify that the updated commit process works with the "nano" editor, ensuring it integrates smoothly with the "pull" and "push" commands.
3. Review the prompt template for Conventional Commits to ensure it meets the provided guidelines and formatting requirements.

## Related Issues
- [Ticket]()
```
