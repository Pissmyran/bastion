# Issues

GitHub Issues in `Pissmyran/bastion` takes issues that concern every platform. Issues for a single platform belong in that platform's repo; move them there with **Transfer issue**.

## Working with issues

- Read the whole issue before working on it: text, labels, comments and linked pull requests.
- An issue should describe one coherent problem, with acceptance criteria and blockers in the text.
- Decisions that should last go into the documentation, not only into a comment.

## From a cloud session

`gh issue` does not work in cloud sessions (GraphQL is disabled). Use REST:

Set the issue number first:

```bash
ISSUE=1
```

Read an issue:

```bash
gh api repos/Pissmyran/bastion/issues/$ISSUE
```

Read its comments:

```bash
gh api repos/Pissmyran/bastion/issues/$ISSUE/comments
```

List open issues:

```bash
gh api 'repos/Pissmyran/bastion/issues?state=open'
```

Create an issue:

```bash
gh api repos/Pissmyran/bastion/issues -f title='…' -f body='…'
```

Comment on an issue:

```bash
gh api repos/Pissmyran/bastion/issues/$ISSUE/comments -f body='…'
```

Close an issue:

```bash
gh api -X PATCH repos/Pissmyran/bastion/issues/$ISSUE -f state=closed
```

Projects (GitHub Projects) cannot be read or changed from a cloud session.
