# Professional repo - basic rules

The most important rule in maintaining a professional repo is to always think about people that you share your code with: collaborators, code reviewers, programmers, recruiters or non-technical users who might want to reuse and/or improve your project.

Ask yourself the question: *what information might they need from you in order to use your repo?*

Also keep them in mind when something unexpected happens. If you realize that you made a mistake and something is not working as it should, communicate it to your collaborators so that they know not to expect the normal behavior from that feature until it is fixed - you can leave a comment, open an issue, or leave a link to the specific line of code.

## 5 basic rules to follow in Microverse projects

Following these five rules is a simple way to make your repo look professional:

1. Respect the rules of the code review flow that your team follows. Use descriptive names for your branches (e.g., refactor-authentication, user-content-cache-key, make-retina-avatars) and make sure that your 'feature branch' is up-to-date with the 'main branch' in your repository.

2. Write a meaningful title for your pull request and always add a short summary of changes introduced in the pull request.
    ![Pull Request Description](../images/pull_request_desc.gif)

3. Use descriptive commit messages - each commit should be small enough to describe it in one sentence. The commit message should be written in the **imperative tense and capitalized**. [Read more about how to write descriptive commit messages](https://www.freecodecamp.org/news/level-you-up-to-awesome-commit-messages-a85558cb90e8).
     - Here are some examples of descriptive commits:
         ![Pull Request Description](../images/descriptive_commits_example.png)
     - Here are some commits that are not descriptive:
         ![Pull Request Description](../images/not_descriptive_commits.png)
  
4. Do not commit files that are not related to the project. Instead, add them to a [.gitignore file](https://www.freecodecamp.org/news/gitignore-what-is-it-and-how-to-add-to-repo/). **A common mistake is to commit entire `node_modules` directory which makes your pull request unreadable.**

5. Add descriptive README file to your project - please use [this template](https://github.com/microverseinc/readme-template) but remember to customize it to your project.

## Useful hints

There are a few useful hints that can help you to keep your repo professional:

1. If you need to correct your commit message you can do it for your most recent commit by using [`git commit --amend` command](https://www.atlassian.com/git/tutorials/rewriting-history#git-commit--amend). 
2. If you want to make your GitHub messages more organized you can use [Markdown syntax](https://guides.github.com/features/mastering-markdown/).
3. Remember that adding a file to the `.gitignore` cannot also be used to remove files that you added using that technique. If you committed a useless file into your repo you need to remove it manually.
4. Do not disable Eslint or Stylint using inline comments within your code if not specified in the project requirement.





------

_If you spot any bugs or issues in this activity, you can [open an issue with your proposed change](https://github.com/microverseinc/curriculum-transversal-skills/blob/main/git-github/articles/open_issue.md)._