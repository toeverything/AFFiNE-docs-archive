---
description: >-
  Affine welcomes open source enthusiasts to collaborate and contribute
  interesting ideas and code.
---

# ❤ Making Code Contributions

## What Does It Mean to Contribute <a href="#what-it-means-to-contribute" id="what-it-means-to-contribute"></a>

If you are a new open source contributor, the process can be daunting - What if you don't know how to code? What if something goes wrong?

Don't worry! This article will provide detailed guidance for you.

## Get Started

### Create Issue

You should usually open an issue when you have trouble with:

* Presenting a problem you have that you cannot solve
* Presenting a valid idea, expectation, or conjecture about a topic
* Proposing a new feature
* Propose to improve or refactor existing code through code generation

Tips for communicating on issues:

* **If you see an open issue that you want to tackle,** comment on the issue. That way, people are less likely to duplicate your work.
* **If an issue was opened a while ago,** it’s possible that it’s being addressed somewhere else, or has already been resolved, so comment to ask for confirmation before starting work.
* **If you opened an issue, but figured out the answer later on your own,** comment on the issue to let people know, then close the issue. Even documenting that outcome is a contribution to the project.

### [**Fork Repository**](https://guides.github.com/activities/forking/)

You can fork the repository and clone the code repository to the local workspace.

Connect your local workspace to the original "upstream" repository by adding it as a remote.

Sync upstream branches from time to time keeps your code up to date. When you submit a pull request, the possibility of encountering conflict can be greatly reduced (see more detailed instructions [here](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork)).

### [**Create Branch**](https://guides.github.com/introduction/flow/) & Start Development

Create a local branch in your workspace and make the necessary changes.

### Test Changes

Run your changes against any existing test and create new ones when needed. Whether tests exist or not, make sure your changes would not break the existing project.

It's important to maintain a consistent style with existing code (e.g. indentation, semicolons, the way comments are written), which makes it easier for maintainers to merge and for others to understand and maintain in the future.

### [Open Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) <a href="#opening-a-pull-request" id="opening-a-pull-request"></a>

Pull requests do not necessarily mean completed work. It is often better to open pull requests early on so that others can see your progress or give feedback. Simply mark it as "WIP" (Work in Progress) in the subject line. You can add more commits later.

* Reference any relevant issues or supporting documentation in your PR (for example, "Closes Issues#2345").
* If the view layer has changed, please include a comparison diagram of the difference before and after the change. If the performance metrics have changed, please detail the reasons for the change. So that the code review can be more focused.

{% hint style="info" %}
To ensure the security of our product, we kindly request that you share any scripts that may have been used to generate code changes. This allows us to audit the code and prevent any malicious code execution.
{% endhint %}

{% hint style="info" %}
Where appropriate, please consider submitting larger changes into smaller, separate pull requests.
{% endhint %}

## Tips

If your pull request has not progressed for a long time (close or merge), please send the relevant information to contact@toeverything.info.

Remember: you need to include the issue number in the content of your email.
