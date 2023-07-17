# Github_actions
https://docs.github.com/en/actions/quickstart

https://www.udemy.com/course/github-actions-the-complete-guide/

## Github actions key Components: Workflows, Jobs, Steps & More
![image](https://github.com/luiscoco/Github_actions/assets/32194879/920a80f7-7ae4-47c2-9370-2b1b4e4a7e01)

- Workflow
A workflow is a configurable automated process that will run one or more jobs. Workflows are defined by a YAML file checked in to your repository and will run when triggered by an event in your repository, or they can be triggered manually, or at a defined schedule.

Workflows are defined in the .github/workflows directory in a repository, and a repository can have multiple workflows, each of which can perform a different set of tasks. For example, you can have one workflow to build and test pull requests, another workflow to deploy your application every time a release is created, and still another workflow that adds a label every time someone opens a new issue.

You can reference a workflow within another workflow. For more information, see "Reusing workflows."

For more information about workflows, see "Using workflows."

- Jobs
A job is a set of steps in a workflow that is executed on the same runner. Each step is either a shell script that will be executed, or an action that will be run. Steps are executed in order and are dependent on each other. Since each step is executed on the same runner, you can share data from one step to another. For example, you can have a step that builds your application followed by a step that tests the application that was built.

You can configure a job's dependencies with other jobs; by default, jobs have no dependencies and run in parallel with each other. When a job takes a dependency on another job, it will wait for the dependent job to complete before it can run. For example, you may have multiple build jobs for different architectures that have no dependencies, and a packaging job that is dependent on those jobs. The build jobs will run in parallel, and when they have all completed successfully, the packaging job will run.

For more information about jobs, see "Using jobs."


- Steps


- Actions



## Sequential or parallel jobs in Github actions

- Parallel jobs


- Sequential jobs




## Triggers for starting the workflow in the Github actions

https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows

### Events. 
An event is a specific activity in a repository that triggers a workflow run. For example, activity can originate from GitHub when someone creates a pull request, opens an issue, or pushes a commit to a repository. You can also trigger a workflow to run on a schedule, by posting to a REST API, or manually.
For a complete list of events that can be used to trigger workflows, see Events that trigger workflows.

### Events list for triggering a workflow:

- branch_protection_rule

- check_run

- check_suite

- create

- delete

- deployment

- deployment_status

- discussion

- discussion_comment

- fork

- gollum

- issue_comment

- issues

- label

- merge_group

- milestone

- page_build

- project

- project_card

- project_column

- public

- pull_request

- pull_request_comment (use issue_comment)

- pull_request_review

- pull_request_review_comment

- pull_request_target

- push

- registry_package

- release

- repository_dispatch

- schedule

- status

- watch

- workflow_call

- workflow_dispatch

- workflow_run

