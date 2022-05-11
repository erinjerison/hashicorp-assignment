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

<!-- EAJ TODO: Determine best structure for the document after working with the material. Ideas: Subheadings for each command; ol that contains an extended explanation; table that keeps command, description, and why to use it in rows -->
# Managing code via the command line
Git offers you many ways to manage your code both locally and remotely. Create branches to separate updates from production code, create patches, test ideas, and merge your changes into the codebase. The command line makes it easy to download, review, modify, and push changes between your local machine and a remote repository. <!-- New audiences may require a more in-depth intro, so we're leaving room for that here. -->

<!-- Thought again; we could either link off to docs around local/remote branches and repositories if users need a refresh on this documentation or if they're newer to git and would require this information. -->

## Git code management commands

<!-- EAJ NOTE: Rearranging because the foundations build on each other -->
Git includes three commands that you can use to review, update, and publish your changes to and from your local and remote repositories.
- `fetch` - Retrieve code updates from a remote repository to place into your tracking branch.
- `pull` - This command retrieves changes from a remote branch to place into your tracking branch before merging them into a local branch.
- `push` - Send changes from a local branch to a remote repository.

Find more information about these commands in the sections to follow.

### Retrieving code updates (`fetch`)
The `fetch` command first checks your local branch to determine whether an associated tracking branch exists remotely. If the tracking branch exists, `fetch` retrieves the changes and history from the tracking branch and pulls those changes into the <!-- tracking? remote? --> branch.

The `fetch` command does not update your local branch.

<!-- EAJ QUESTIONS:
    - The text that was originally here was confusing and a jumble of terminology. I am primarily trying to get straight what is updated and where. I understand that it downloads a branch from a remote repository (either the origin or an upstream branch), including the history of each asset. What I don't understand is when we say "retrieve" or "download," where is this downloaded to? It says my local branch isn't updated, but how can I review it locally if my local branch isn't updated? Is it updated on a remote repository?
    - Does the user need to run fetch before they pull or push? How often?
-->

### Retrieving changes and merging them to your local repository (`pull`)
The `pull` command fetches changes from the tracking branch or repository, then applies those changes to your local repository so that you have the latest copy.

### Sending your changes to the remote repository (`push`)
The `push` command checks for a tracking branch or remote repository, then updates the remote branch with your changes.

To ensure that you can successfully push updates to the remote branch, pull the latest version of your objects from the repository or branch.

NOTE: Track the updates you make through pull requests and commits. [Create a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) and [commits](https://github.com/git-guides/git-commithttps://github.com/git-guides/git-commit) before you [merge](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/keeping-your-local-repository-in-sync-with-github/syncing-your-branch#merging-another-branch-into-your-project-branch) your updates into the main branch of the repository. 
<!-- TODO: Add info around the fact that pull must be run to ensure that push commands work -->

<!-- EAJ TODO:
- Be sure to include information about each command's purpose, why it's important, what problems they are expected to solve.
- Consider defining/explaining the various branches and repositories mentioned.
- Verify that the correct branches and repositories are mentioned; a brief Google search for some terms makes what's below confusing.
- Review GitHub and git documentation to make sure this information is complete.
- Consider images?
-->