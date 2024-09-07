### Commit Message Generator

---

**Purpose:**
The Commit Message Generator helps you write commit messages that follow a standard format. This makes it easier for everyone to understand what changes were made and why, and it helps with automated tasks like generating changelogs.

**What It Does:**

- It converts your input into a well-structured commit message based on a set format.
- This includes specifying the type of change, optionally noting which part of the code was affected, and giving a brief description of the change.
- You can also add a detailed explanation if needed.

**What You Need to Provide:**

- **Type of Change:** What kind of change did you make? For example, was it a new feature, a bug fix, or just a code cleanup?
- **Scope (Optional):** If the change affects a specific part of the project, mention it. For example, if you updated the login system, you might write `auth`.
- **Short Description:** A brief summary of what you did. Keep it clear and to the point.
- **Detailed Explanation (Optional):** If you want to, you can explain why you made the change, what exactly was done, and how it affects the project.

**Expected Result:**

- A formatted commit message that fits the Conventional Commits standard. For example:

  ```
  feat(auth): add JWT authentication for secure routes

      - Implemented JWT-based authentication to secure routes.
      - Added middleware for token validation before route access.
      - Updated login and signup endpoints to handle token issuance.
  ```

**Use Case:**

- To make your commit messages clear and standardized, which helps in understanding the history of changes and automating some tasks.

> [!TIP]
Just copy all the content (Prompt) that is in `commit_generator.md` and paste it into a new ChatGPT chat.

---

### Pull Request (PR) Message Generator

---

**Purpose:**
The Pull Request Message Generator helps you create a detailed and organized description for your pull request. This is useful for explaining what changes you made, why you made them, and how others can test them.

**What It Does:**

- It takes the list of commits you’ve made and turns it into a structured PR description.
- This includes a title that summarizes the changes, and a detailed description with context, a list of changes, testing instructions, and links to related issues.

**What You Need to Provide:**

- **Git Log:** A list of commits that includes information like the commit messages and any changes made. This helps the tool understand what changes you’ve made.

**Expected Result:**

1. **Title:**

   - A short, clear title that summarizes the main changes. It should be easy to read and formatted for use in bash commands.
   - Example Title:
     ```bash
     [Feature] Implement Git Buddy Script, Add Commit Prompt Template, and Update Commit Process
     ```

2. **Content:**

   - **Context:** Explain what problem or need this PR addresses.
   - **Changes:** List what you changed based on the commits.
   - **How to Test:** Provide steps on how to test the changes to make sure they work.
   - **Related Issues:** Mention any related tickets or issues for more context.

   Example Content:

   ```
   ## Context
   This PR updates the Git Buddy program and improves the commit process. It includes a new script and changes to how commits are handled.

   ## Changes
   - Added a new script for the Git Buddy program.
   - Changed the commit process to use the "nano" editor for better message writing.
   - Created a prompt template for Conventional Commits.

   ## How to Test
   1. Check out the branch and run the Git Buddy program.
   2. Test the updated commit process with the "nano" editor.
   3. Review the new commit prompt template.

   ## Related Issues
   - [Ticket]()
   ```

**Use Case:**

- To provide a clear and thorough explanation of your pull request, making it easier for others to review, test, and understand the changes.

> [!TIP]
Just copy all the content (Prompt) that is in `pull_request_generator.md` and paste it into a new ChatGPT chat

---

These explanations aim to be straightforward and approachable, providing a clear understanding of what each tool does and how to use it.
