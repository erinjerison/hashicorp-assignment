# Managing code via the command line
Git offers you many ways to manage your code both locally and remotely. Create branches to separate updates from production code, create patches, test ideas, and merge your changes into the codebase. The command line makes it easy to download, review, modify, and push changes between your local machine and a remote repository.

## Git code management commands

Git includes three commands that you can use to review, retrieve, and publish changes to and from your local and remote repositories:
- `git fetch` - Retrieve code updates from a remote repository to place into your tracking branch.
- `git pull` - This command retrieves changes from a remote branch to place into your tracking branch before merging them into a local branch.
- `git push` - Send changes from a local branch to a remote repository.

Find more information about these commands in the sections to follow.

### Retrieving updates from a branch (`git fetch`)
The `git fetch` command retrieves the changes and history from a tracking branch to a locally-cached version of your remote repository. The `git fetch` command gives you an opportunity to review the changes that others have made to the tracking branch before merging them with the assets in your local branch. You can use `git fetch` to resolve conflicts before you merge them to your local branch.

The `git fetch` command does not update your local branch.

To learn more about `git fetch`, review [Git's `git fetch` documentation](https://git-scm.com/docs/git-fetch).

### Retrieving changes and merging them to your local repository (`git pull`)
The `git pull` command fetches changes from a remote repository, then applies those changes to your local repository so that you work from the latest copy. Git can compare that version of your assets to any updates you make, making it easier for git to know what has changed before pushing or merging changes to the repository.

You must run `git pull` often to ensure that your local assets match the remote repository.

To learn more about `git pull`, review [GitHub's Git Pull guide](https://github.com/git-guides/git-pull).

### Sending your changes to the remote repository (`git push`)
The `git push` command updates the remote branch with your local changes. To ensure that you can successfully push updates to the remote branch, pull the latest version of your objects from the repository or branch.

NOTE: Track the updates you make through pull requests and commits. [Create a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) and [commits](https://github.com/git-guides/git-commithttps://github.com/git-guides/git-commit) before you [merge](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/keeping-your-local-repository-in-sync-with-github/syncing-your-branch#merging-another-branch-into-your-project-branch) your updates into the main branch of the repository.

To learn more about `git push`, review [GitHub's Git Push guide](https://github.com/git-guides/git-push).

## Additional resources
- [Git Guide](https://github.com/git-guideshttps://github.com/git-guides)
- [Git documentation](https://git-scm.com/doc)