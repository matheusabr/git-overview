## Commit Messages Best Practices

Use this as a guide on how to write good and effective commit messages in Git.

### Contents

1.  [Why Commit Messages Matter](#why-commit-messages-matter)
2.  [Structure of a Commit Message](#structure-of-a-commit-message)
3.  [Common Commit Types](#common-commit-types)
4.  [Examples of Good Commit Messages](#examples-of-good-commit-messages)
5.  [Common Mistakes to Avoid](#common-mistakes-to-avoid)

---

### Why Commit Messages Matter

Commit messages are an important aspect of version control. They provide context and reasoning for changes, making it easier for others to understand the history and purpose of the code.

### Structure of a Commit Message

A well-structured commit message typically consists of three parts:

1.  **Header**: A short, concise summary of the change (max 50 characters).
2.  **Body**: A detailed explanation of the change, including the reasoning behind it (if necessary).
3.  **Footer**: Any additional information, such as references to issues or breaking changes.

Example:

```
type(scope): subject

body

footer
```

### Common Commit Types

- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation only changes
- **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- **refactor**: A code change that neither fixes a bug nor adds a feature
- **perf**: A code change that improves performance
- **test**: Adding missing or correcting existing tests
- **chore**: Changes to the build process or auxiliary tools and libraries such as documentation generation

### Examples of Good Commit Messages

1.  **Feature Addition**:

    ```
    feat(auth): add user login feature

    Implemented user login functionality using JWT for authentication. Updated the login API endpoint to return a token upon successful login.
    ```

2.  **Bug Fix**:

    ```
    fix(products-api): resolve 500 error on data fetch

    Fixed a bug causing a 500 Internal Server Error when fetching products data from the API. The issue was due to an unhandled null value in the response.
    ```

3.  **Documentation Update**:

    ```
    docs: update README with setup instructions

    Added detailed setup instructions to the README file to help new developers get started with the project.
    ```

4.  **Style Change**:

    ```
    style: format code to match coding standards

    Applied consistent formatting across the codebase to adhere to the project's coding standards. This change does not affect the functionality of the code.
    ```

5.  **Code Refactoring**:

    ```
    refactor(utils): simplify date parsing logic

    Refactored the date parsing logic to use a more efficient library, reducing the code complexity and improving readability.
    ```

6.  **Performance Improvement**:

    ```
    perf(cache): improve caching mechanism

    Enhanced the caching mechanism to reduce database queries and improve overall application performance.
    ```

7.  **Adding Tests**:

    ```
    test(auth): add unit tests for login feature

    Added unit tests for the user login functionality to ensure the authentication process works correctly.
    ```

8.  **Chore Task**:

    ```
    chore(deps): update dependencies

    Updated project dependencies to their latest versions to ensure compatibility and security. This change does not affect the application's functionality.
    ```

### Common Mistakes to Avoid

- **Vague Messages**: Avoid vague messages like "fixed stuff" or "updated code".
- **No Context**: Ensure your commit message provides enough context for someone else to understand the changes.
- **Too Long**: Keep the header under 50 characters and wrap the body at 72 characters.
- **Irrelevant Details**: Stick to relevant information and avoid unnecessary details.
