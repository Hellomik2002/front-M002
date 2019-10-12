<h1 align="center">❤️ Hi and thanks for contributing!</h1>

---

<p align="center">
    <strong><a href="#history">History</a></strong>
    |
    <strong><a href="#workflow">Workflow</a></strong>
    |
    <strong><a href="#codestyle">Code style</a></strong>
</p>

---

<h3 id="history">History</h3>

We prefer git linear history, therefor `merge` is not permitted,
so instead you have to use `rebase`.

#### Creating branch
There is a particular branch naming convention in our project:
```bash
FM-${issue_code}
```
***Examples:*** `FM-1`, `FM-14`, `FM-542` and so on.

#### Commit messages
Our project uses
[conventional commit message style](https://www.conventionalcommits.org/en/v1.0.0/),
so `pre-commit` hooks should be enabled to lint message in an appropriate way.

#### Creating merge request
Merge request should contain only one commit with issue code at the end
of the message or pull request should be written as if it would be a
squash commit message.

***Example:*** `fix(app-template): remove listener on unmount (#135)`


<h3 id="workflow">Workflow</h3>
Tasks are managed by `code owners` in the main
[project](https://github.com/olehan/front-M002/projects/1)
of the repo. To start working on the task you:

+ Have to be assigned to it
+ Task should be on `To Do` or `In Progress` board.

All your work should be done in your own task branch
(We talked about branch name convention before at `Creating branch`).

When you're done with coding - create a pull request and assign your `code reviewer`
from `code owners`. After the acceptable count of approvals, you may `squash merge`
or `rebase` pull request and don't forget to add an automation issue command
that closes your task.


<h3 id="codestyle">Code Style</h3>
Code style is controlled by `eslint` and `code reviewers`.

