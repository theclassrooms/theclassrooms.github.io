## Git and Github

### Knowledge required.

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

| complexity          | Material                                       |
| ------------------- | ---------------------------------------------- |
| `choose-your-path` | [Github Labs][1a]                              |
| `become-a-pro`      | Tim Roughgarden's [lecture catalogue][1c]      |
| `Geek-Out`          | [Introduction to Algorithms - Book][1d]        |
| `become-a-pro`      | [Basics of Data structures and Algorithms][1e] |

<!--Reference links in article-->

[1a]: https://lab.github.com/


- Gaming/visual version of learning Git by doing from Day 0 to Advanced:
  - https://github.com/Gazler/githug
  - https://learngitbranching.js.org/
  - https://git-school.github.io/visualizing-git/#rewritten-history
- Following a Manual:
  - beginner to ramped-up: https://githubtraining.github.io/training-manual/book.pdf
  - App based training(if you have not used git before) https://github.com/jlord/git-it-electron#what-to-install
  - Everything : https://git-scm.com/book/en/v2
- Video
  - For absolute begineers: https://www.youtube.com/watch?v=8JJ101D3knE

_Github_

> prerequisite: knowledge on `git`

- Already Githubbing? , but just winging it - here: the docs are really well written and organised , would recommend just going through it with practice - https://docs.github.com/en
- Starting from scratch: https://lab.github.com/githubtraining/introduction-to-github

- Github Actions:
  - Already doing CI/CD in someother tool : https://docs.github.com/en/actions/learn-github-actions (recommend for aggressive learning, if already using any CI/CD)
  - Starting from scratch: https://lab.github.com/githubtraining/github-actions:-hello-world (slow learning path for beginners into CI/CD)

### Usecases Yardstick

#### Git

- You have pushed a commit to github, undo the commit.
- Amend commit message of previous commits
- undo local changes on certain files that are committed locally.
- Reset the whole repository to remote or a paticular commit.
- You made a commit , undid the commit , but want those changes back.
- you made lots of changes , but realised you were on master/main and actually need those changes on a feature branch
- Synchronise your lagging branch with master
- You have some files that you want to keep , but not yet to commit , but need to switch branches to make changes in another feature.
- Bulk changes
  - you've been doing a lots of commits and you want to remove lots of commits (you got a better solution) , reorder some, merge few commits together , reword commit messages.
- Resolve complex merge conflicts across multiple files

#### Github

_Repository management and security_

- Create a repository and setup branch protection, with multiple reviewers
- Protect certain directories with code owners
- Use github CLI to check pull requests etc
- Use github on vscode/IDE (to see changes, diff, stage)
- Coauthoring on github
- Signing commits on github
- Creating ssh , gpg, pat tokens with expiry and RBAC. know the right RBAC needed for tokens.

** Github Actions**

- Create workflow to deploy build an app (anything - https://expressjs.com/en/starter/hello-world.html) and create a zip file that you can download unzip and run in local
- Build a docker file into github packages , tag it with the sha of the commit and tag it as latest as well, and test to pull and run the docker contianer on local
- Write a composite action for printing "hello" or doing a build
- Write a reusable workflow that you call to just do any of the above.
- Handling secrets and Environments
  - Conditionally check hierarchy of secrets to a value (org secret, repo secret , environment secret)
