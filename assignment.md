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

<!-- EAJ NOTE: I am removing "git" from the code phrases below. I am assuming that this is part of a larger docset that has already introduced the concept of git on the command line and we've moved on to tasks users will need to complete. -->
Git includes three commands that you can use to review, update, and publish your changes to and from your local and remote repositories.
- `fetch` - Retrieve code updates from a remote repository to place into your tracking branch.
- `pull` - This command retrieves changes from a remote branch to place into your tracking branch before merging them into a local branch.
- `push` - Send changes from a local branch to a remote repository.

Find more information about these commands in the sections to follow.

### Retrieving code updates (`fetch`)
The `fetch` command first checks your local branch to determine whether an associated <!-- tracking? remote? --> branch exists. If the tracking branch exists, `fetch` will retrieve the changes from the <!-- tracking? remote? --> branch and pulls those changes into the <!-- tracking? remote? --> branch.

The `fetch` command does not update your local branch.

<!-- EAJ QUESTION: The text that was originally here was confusing and a jumble of terminology. -->

<!-- EAJ TODO:
- Be sure to include information about each command's purpose, why it's important, what problems they are expected to solve.
- Consider defining/explaining the various branches and repositories mentioned.
- Verify that the correct branches and repositories are mentioned; a brief Google search for some terms makes what's below confusing.
- Review GitHub and git documentation to make sure this information is complete.
- Consider images?
-->

<!-- DRAFT: COMMAND SUBHEADINGS -->

#### What is `git fetch`

Often `git push` and `git pull` are described as equivalent. This isn't entirely correct, since under the hood `git pull` does two things. `git push` takes our current branch, and checks to see whether or not there is a tracking branch for a remote repository connected to it. If so, our changes are taken from our branch and pushed to the remote branch. This is how code is shared with a remote repository, you can think of it as "make the remote branch resemble my local branch". This will fail if the remote branch has diverged from your local branch: if not all the commits in the remote branch are in your local branch. When this happens, your local branch needs to be synchronized with the remote branch with git pull or git fetch and git merge. To do that, you'll need to do `git merge origin/master` (for the "master" branch) to merge those changes into your branch - probably also called "master".`git pull` simply does a `git fetch` followed immediately by `git merge`. This is often what we desire to do, but some people prefer to use git fetch followed by git merge to make sure they understand the changes they are merging into their branch before the merge happens.
