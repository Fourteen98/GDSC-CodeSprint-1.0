# How to use Gitflow

## Development branch VS main branch

You can think about the `main` branch as a snapshot of your application that at any moment can be used for deployment to production (which often occurs automatically). You do not want to deploy broken code by accident!

The `development` branch is also a snapshot of your application , but rather than deploying to production, the `development` branch could be used at any moment for developing new features with multiple collaborators. Your teammates need a stable version of your project to start implementing changes, so maintaining a `development` branch will give them stable code to work from.

*Please, compare this description with [GitHub flow](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/github_flow.md).*

You should observe that:
- The `main` branch in GitHub flow played two roles.
- Those two roles are separated in the Gitflow.

Therefore both - the `main` branch and the `development` branch should always be perfectly maintained. Any changes required in the application should be introduced in `feature` branches and approved before merging them to the `development` branch. 
Changes to the `main` branch can be merged only from the `development` branch and **reviewed**. Because of that process, code in the `main` branch is reviewed twice, which also gives you more control over the deployed features. For example, you can decide to deploy a group of features at once.

## Feature branches

You are already familiar with `feature` branches. In Gitflow, they play the same role as in [GitHub flow](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/github_flow.md).

## Opening pull requests

Once you start working on any project, initialize its `main` branch. You also need to create a `development` branch.
Then you need to make your `development` branch [the default branch](https://docs.github.com/en/github/administering-a-repository/managing-branches-in-your-repository/changing-the-default-branch#changing-the-default-branch).

After that, add changes in a `feature` branch(es).
You will need to create a *pull request* to compare your `feature` branch with the `development` branch and submit the link to that pull request via your Dashboard.
After you submit the link to your pull request, you will get a code review from one of our code reviewers. 

You should not merge your pull requests to the `main` branch or `development` branch of your project without a code review that *approves* your changes.

Watch [this 5 minute long video](https://youtu.be/d0WEe8xH5mk) with a simple example of Gitflow and opening a pull request.

------

_If you spot any bugs or issues in this activity, you can [open an issue with your proposed change](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/open_issue.md)._