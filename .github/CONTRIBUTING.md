# Contributing

## Our contribution model

Code Challenges is an **open source** project aiming to give many options for developers to practice and get ready to apply for a job in their specialty.  If you're wondering more about our contribution process, you're in the right place. First off, thank you for your
interest! This project is possible because of several community members who have invested their own time to give back
to the dev community.

## Prerequisites

Before contributing to Code Challenge, you should make sure you have the following tools
installed:

- [Node.js](https://nodejs.org/en/download/) v16 or above here or follow their
  installation through a package manager
  [here](https://nodejs.org/en/download/package-manager/))

You'll also need a code editor to make changes on the code. There are many to
choose from but some popular options are
[VSCode](https://code.visualstudio.com/), [Atom](https://atom.io), and
[Sublime](https://www.sublimetext.com/).

With that all in place, you're ready to start contributing to Code Challenge!

## Start contributing

### 1. Fork the repo:

Go to
[Code Challenge's repository on GitHub](https://github.com/RianTavares/code-challenges) and click the `Fork` button in the top-right corner. This will create a copy repo of Carbon associated with your account.

### 2. Clone your fork:

1.  Go to your [GitHub Repositories](https://github.com/settings/repositories).
1.  Click on `[your_github_username]/code-challenges`.
1.  Click on the `Clone or Download` button and copy the URL from the
    `Clone with SSH` option. It should start with `git@github.com...`

In your terminal:

```sh
git clone git@github.com:[your_github_username]/code-challenges.git
cd code-challenges
```

See [GitHub docs](https://help.github.com/articles/fork-a-repo/) for more details.

### 3. Add upstream remotes

When you clone your forked repo, running `git remote -v` will show that the
`origin` is pointing to your forked repo by default.

Now you need to add the `RianTavares/code-challenges` repo as your upstream remote branch:

```sh
# Add the upstream remote to your repo
git remote add upstream git@github.com:RianTavares/code-challenges.git

# Verify the remote was added
git remote -v
```

Your terminal should output something like this:

```sh
origin  [your forked repo] (fetch)
origin  [your forked repo] (push)
upstream    git@github.com:RianTavares/code-challenges.git (fetch)
upstream    git@github.com:RianTavares/code-challenges.git (push)
```

### 4. Work in a branch

When contributing to Code Challenges, your work should always be done in a branch off of your repo, this is also how you will submit your pull request when your work is done.

To create a new branch, ensure you are in your forked branch in your terminal and run:

```sh
git pull origin main
git checkout -b {your-branch-name}
```
Now you can add you contribution :)

### 5. Add yourself to the contributor list

We want to make sure everyone is recognized for their contributions to Code Challenges!
To add yourself to the `all-contributors` table in the README, you'll need to run the following commands from the root of the repo:

```sh
# Add new contributor <username>, who made a contribution of type <contribution>
npx all-contributors add <username> <contribution>
# Example:
npx all-contributors add facePalmUser code,doc
```

Then, you'll need to generate the updated `all-contributors` table by running

```sh
npx all-contributors generate
```

### 8. Make a pull request

**Note:** Before you make a pull request,
[search](https://github.com/RianTavares/code-challenges/issues) the issues to see if a similar issue has already been submitted. If a similar issue has been submitted, assign yourself or ask to be assigned to the issue by posting a comment. If the issue does not exist, please make a new issue. Issues give us context about what
you are contributing and expedite the process to getting your contributions merged into Code Challenges repo. It's a win for everybody :tada:

When you're at a good stopping place and you're ready for feedback from other contributors and maintainers, **push your commits to your fork**:

To do so, go to your terminal and run:

```sh
git add -A
git commit -m "YOUR  COMMIT MESSAGE HERE"
```

#### Commit tip

> **Writing commit messages**
>
> - `<type>` indicates the type of commit that's being made. This can be:
>   `feat`, `fix`, `perf`, `docs`, `chore`, `style`, `refactor`
> - `<scope>` The scope could be anything specifying place of the commit change or the thing(s) that changed.

After your changes are committed, run:

```sh
git push -u origin { YOUR_BRANCH_NAME }
```

In your browser, navigate to
[RianTavares/code-challenges](https://github.com/RianTavares/code-challenges) and click the button that reads `Compare & pull request`

Write a title and description then click `Create pull request`

- [How to write the perfect pull request](https://github.com/blog/1943-how-to-write-the-perfect-pull-request)

### 9. Updating a pull request

Stay up to date with the activity in your pull request. Maintainers from the Code challenges repo team will be reviewing your work and making comments, asking questions and suggesting changes to be made before they merge your code.

When you need to make a change, use the same method detailed above except you no longer need to run `git push -u origin { YOUR_BRANCH_NAME }` just `git push`.

Once all revisions to your pull request are complete, someone from the team will squash and merge your commits for you.
## FAQ

### Who can contribute?

Anyone! We mean it. The one and only requirement is you'll need a
[public GitHub account](https://github.com/join), as all our assets live on GitHub.
