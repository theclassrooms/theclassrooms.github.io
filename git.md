## Git

### What you will learn

- Expert in `git`
  - push/pull/branch/rebase/merge
- Expert in `github`
  - repository management
  - security on the repository
  - user management
  - using github apps (eg: probot for repository management)
  - github actions

### Learning Paths

_Git_

| complexity         | Material                                    |
| ------------------ | ------------------------------------------- |
| `choose-your-path` | [Github Labs][1a]                           |
| `in-an-hour`       | [video tutorial][1c]                        |
| `become-a-pro`     | [git scm guide][1b]                         |
| `crash-course`     | [training-manual][1d]                       |
| `crash-course`     | [training-manual][1d]                       |
| `learn-with-fun`   | gaming and learning [1][1e] [2][1g] [3][1h] |

<!--Reference links in article-->

[1a]: https://lab.github.com/
[1b]: https://git-scm.com/book/en/v2
[1c]: https://www.youtube.com/watch?v=8JJ101D3knE
[1d]: https://githubtraining.github.io/training-manual/book.pdf
[1e]: https://learngitbranching.js.org/
[1f]: https://learngitbranching.js.org/
[1g]: https://git-school.github.io/visualizing-git/#rewritten-history
[1h]: https://github.com/jlord/git-it-electron#what-to-install

## Github

> prerequisite: knowledge on `git`. Look [here](git.md#git)

- Are you already Githubbing? but just winging it - here: the docs are really well written and organised, would recommend just going through it with practice - https://docs.github.com/en
- Starting from scratch: https://lab.github.com/githubtraining/introduction-to-github

- Github Actions:
  - Are you already doing CI/CD in some other tool: https://docs.github.com/en/actions/learn-github-actions (recommend for aggressive learning, if already using any CI/CD)
  - Starting from scratch: https://lab.github.com/githubtraining/github-actions:-hello-world (slow learning path for beginners into CI/CD)

### Usecases Yardstick

#### Git

- You have pushed a commit to Github, undo the commit.
- Amend the commit message of previous commits
- undo local changes on certain files that are committed locally.
- Reset the whole repository to remote or a particular commit.
- You made a commit, undid the commit, but want those changes back.
- You made lots of changes but realised you were on master/main and need those changes on a feature branch
- Synchronise your lagging branch with master
- You have some files that you want to keep, but not commit yet, but need to switch branches to make changes in another feature.
- Bulk changes
  - you've been doing lots of commits, and you want to remove lots of commits (you got a better solution), reorder some, merge a few commits, and reword commit messages.
- Resolve complex merge conflicts across multiple files

#### Github

_Repository management and security_

- Create a repository and setup branch protection, with multiple reviewers
- Protect certain directories with code owners
- Use GitHub CLI to check pull requests etc.
- Use Github on vscode/IDE (to see changes, diff, stage)
- Coauthoring on Github
- Signing commits on GitHub
- Creating ssh, gpg, pat tokens with expiry and RBAC. Know the right RBAC needed for tokens.

** Github Actions**

- Create a workflow to deploy build an app (anything - https://expressjs.com/en/starter/hello-world.html) and create a zip file that you can download unzip and run in local
- Build a docker file into GitHub packages, tag it with the sha of the commit and tag it as latest as well, and test to pull and run the docker container on local
- Write a composite action for printing "hello" or doing a build
- Write a reusable workflow that you call to just do any of the above.
- Handling secrets and Environments
  - Conditionally check the hierarchy of secrets to a value (org secret, repo secret, environment secret)
