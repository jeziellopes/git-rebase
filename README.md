### Updating Commits on GitHub

- With `git log` get the <em>commit hash</em>

  > `git rebase -i <commit hash>`

- Inside <em>Vim</em> editor, change 'pick' to 'edit' on commit that will be updated.

  > from: `pick de0e7ec added gh-pages`
  >
  > to: `edit de0e7ec added gh-pages`

- Update the data

  > close <em>Vim</em> saving changes: `qw`
  >
  > user from commit:
  > `git commit --amend --author="username <user@email.com>"`

- Finish rebase!
  > `git rebase --continue`
  >
  > `git log` and it's done!

\*<em>do it for each commit that have to be changed</em>

;)

---

> [source article](https://confluence.atlassian.com/bitbucketserverkb/how-do-you-make-changes-on-a-specific-commit-779171729.html)

> written with [StackEdit](https://stackedit.io/).
