## Creating Pull Requests
### Titling
Generally, we like to use the following format when titling our pull requests:
```
<Jira Ticket Number> - Short summary of changes
```
For example, [this Jira ticket](https://blooom.atlassian.net/browse/IA-889)'s pull request might looks something like:
```
IA-889 - Only log missing input fields when automation is not headless
```

### Drafts
We highly encourage the use of draft pull requests. This gives the team a good way to preview and help guide changes to the code.

### Ready for Review
When a draft pull request is ready for review, mark it as such and post a link in Slack.

## Reviewing Pull Requests
### Required Reviews
We require at least one review from a teammate to merge a pull request into our primary branch, Staging. This is enforced by GitHub. Comments, questions, and suggestions are welcome on pull requests (even if still a draft), and it's encouraged that a subject matter expert takes some time to review changes of code they're familiar with.

### Approval to Merge into Staging
Once a pull request is approved, it can be merged into Staging. This will automatically begin a deploy to the staging environments.

## Releases
Generally, an admin will make a pull request from the Staging to the Master branch. This will give another chance to review the collection of changes, before pushing to production. Once a Staging to Master pull request is merged, this will begin a deployment to produciton.

### Changes with Required Post-Release Work
At times, a pull request will require some amount of work after release. This might be database changes, scheduling tasks, starting experiments, or any number of other tasks. This post-release work needs to be documented in the pull request.
