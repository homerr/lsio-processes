# LinuxServer.io Issues & Pull Requests

This is a work in progress, and is being developed to streamline how LSIO is handling issues and pull requests, to give the users a better experience and manage our workloads more effectively.

A GitHub Project is now in place that will track all issues and pull requests across all repositories within the LinuxServer.io organisation. The rest of this page will break down the processes involved.

## Project Board
GitHub do not currently offer any automation for adding issues and pull requests to a GitHub project, unless you assign repositories to a project. This will not work for us, as there is a 5 repository limit on a project, so we must manually add any new issues and pull requests to the board.

### Adding issues and pull requests to the board for tracking
Regular monitoring of the project board is essential to keep things moving swiftly. Open the board, and click add cards in the top right. A new pane will open up which will then list all current issues and pull requests that are not already in the board. Change the filter to `is:open sort:updated` to bring the most recent items to the top of the list. Any issues for applications developed by the LSIO team should not be added to this project board e.g. Heimdall.

**For Issues:** Drag the card to the to-do column
**For PR:** Drag the card to the needs review column

As these items progress, they will move across the board in line with the automation that is set up and offered by GitHub;

#### Issues
Will need to be manually progressed from To Do across to In Progress once they have been labelled up and assigned. Once an issue is complete (closed) it will then move to the Done column

#### Pull Requests (needs Stark to make this read better)
Will begin life in the Needs review column. Here, it needs to be labelled up with the appropriate labels and assigned to the maintainer of the repository in question. If the PR is satisfactory and CI has passed the maintainer or another member of the LSIO team can approve the PR and it will then automatically move to the Reviewer approved column where it can be merged by either the maintainer, in cases where a PR has been opened by a maintainer, or it can be merged by any member of LSIO if it is a community PR.

The automation on this will only work properly if branch protection has been configured appropriately as detailed (here **replace this**)

### Labels 
Labels must be used to ensure all team members can see, at a glance, where an issue or pull request has originated from and it's current state. 

Proposed labels are:
| Name | Reason | Colour |
|--|--|--|
| new | only for use when issues are being assigned into the project board | teal
| more-info | more information has been requested | yellow 
| feature-request | for issues requesting features added to the container | green
| confirmed-issue | issues that are confirmed to be related to the functionality of the container, and will require input from development to resolve | red
| help-requested | for issues where help is needed to operate or deploy the container | orange
| in-progress | in conjunction with `confirmed-issue` denotes an issue is in progress with a developer | light-green
| blocked | issue is blocked by upstream issues, or another problem | red 
| testing | the issue has been worked on, a fix proposed, and is now being tested | light orange
| complete | issues which are complete | dark green 
| community | pull requests submitted by the community | purple 

