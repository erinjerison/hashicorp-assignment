<!-- ## Overview

This is a technical writing and editing project as part of your interview.

This project is designed to take between 1 - 2 hours.
Please take the time to carefully review the [writing style guide](../styling-guide-snippet.md).

## Instructions

Create a new GitHub repository with the following content (See [content](#content)) as the first commit. Make a branch and open a PR to edit the text for clarity, and include any questions about the content's meaning, as if you were editing a colleague’s work. 

 **Any changes that you think will improve the text and explain the concepts better are welcome**. If anything in the text doesn’t match your opinion on a best practice, feel free to correct the meaning of the text. The result should be a document that you, as a technical writer, would be comfortable sharing with end-users.


Construct your PR to teach the author:
- Make atomic commits.
- Write your commit messages to show your rationale for edits.
- Please construct your commits, commit messages, and PR description as you would for an actual PR as if you were collaborating with a team.
- It is best to edit the files on your local machine and push with the `git` command or a desktop Git application rather than editing directly on the GitHub.com website.

Edit the text so that it is easy to read:
- Correct errors.
- Put the text in active voice and present tense.
- Address the reader as you, not we.
- Phrase statements as positive rather than negative.
- Make the language simple and plain. 
- Avoid euphemisms.
- Structure the text so it has a logical flow. 

Once you're finished with your edits, send the PR link to the HashiCorp recruiter.

**NOTE**: DO NOT FORK THE PROJECT. MAKE A COPY OF ALL FILES, CREATE YOUR OWN FRESH REPOSITORY AND SUBMIT A PULL REQUEST TOWARDS YOUR OWN PROJECT. DO NOT MERGE THE PULL REQUEST.

---

OVERALL QUESTIONS
2. 
3. 

## Content
-->
# Managing code via the command line
Git offers you many ways to manage your code both locally and remotely. Create branches to separate updates from production code, create patches, test ideas, and merge your changes into the codebase. The command line makes it easy to download, review, modify, and push changes between your local machine and a remote repository.<!-- New audiences may require a more in-depth intro, so we're leaving room for that here. -->

## Git code management commands

Git includes three commands that you can use to review, retrieve, and publish changes to and from your local and remote repositories:
- `git fetch` - Retrieve code updates from a remote repository to place into your tracking branch.
- `git pull` - This command retrieves changes from a remote branch to place into your tracking branch before merging them into a local branch.
- `git push` - Send changes from a local branch to a remote repository.

Find more information about these commands in the sections to follow.

### Retrieving updates from a branch (`git fetch`)
The `git fetch` command retrieves the changes and history from a tracking branch to a locally-cached version of your remote repository. The `git fetch` command gives you an opportunity to review the changes that others have made to the tracking branch before merging them with the assets in your local branch. You can use `git fetch` to resolve conflicts before they are merged to your local branch.

The `git fetch` command does not update your local branch.

To learn more about `git fetch`, review [Git's `git fetch` documentation](https://git-scm.com/docs/git-fetch).

### Retrieving changes and merging them to your local repository (`git pull`)
The `git pull` command fetches changes from a remote repository, then applies those changes to your local repository so that you work from the latest copy. The `git pull` command serves as the basis for which code comparisons are made before you push or merge local changes to a branch or repository.

You must run `git pull` often to ensure that your local assets match the remote repository.

To learn more about `git pull`, review [GitHub's Git Pull guide](https://github.com/git-guides/git-pull).

### Sending your changes to the remote repository (`git push`)
The `git push` command updates the remote branch with your local changes. To ensure that you can successfully push updates to the remote branch, pull the latest version of your objects from the repository or branch.

NOTE: Track the updates you make through pull requests and commits. [Create a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) and [commits](https://github.com/git-guides/git-commithttps://github.com/git-guides/git-commit) before you [merge](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/keeping-your-local-repository-in-sync-with-github/syncing-your-branch#merging-another-branch-into-your-project-branch) your updates into the main branch of the repository.

To learn more about `git push`, review [GitHub's Git Push guide](https://github.com/git-guides/git-push).

## Additional resources
- [Git Guide](https://github.com/git-guideshttps://github.com/git-guides)
- [Git documentation](https://git-scm.com/doc)