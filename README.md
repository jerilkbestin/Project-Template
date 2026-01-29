# Project Management with SCRUM Methodology - GitHub Projects Guide

## Overview

This guide provides comprehensive instructions on managing projects using the SCRUM methodology with GitHub Projects. The template includes customizable views, issue tracking with parent-child relationships, and various fields to track progress, priority, and effort estimation.

---

## Table of Contents

1. [Getting Started - Copying the Project Template](#1-getting-started---copying-the-project-template)
2. [Creating Issues and Sub-Issues](#2-creating-issues-and-sub-issues)
3. [Understanding Issue Field Options](#3-understanding-issue-field-options)
4. [Assigning Issues to Team Members](#4-assigning-issues-to-team-members)
5. [Project Views Explained](#5-project-views-explained)
6. [SCRUM Best Practices](#6-scrum-best-practices)
7. [Additional Notes](#7-additional-notes)

---

## 1. Getting Started - Copying the Project Template

To use this project template for your own repository, follow these steps:

### Step-by-Step Instructions: 

1. **Navigate to the Project Board**
   - Go to the project URL:  `https://github.com/users/jerilkbestin/projects/3`
   - Or access it from the repository's "Projects" tab

2. **Access the Project Menu**
   - Click on the **three dots (⋯)** in the top-right corner of the project board
   - This opens the project settings menu

3. **Make a Copy**
   - Select **"Make a copy"** from the dropdown menu
   - Choose whether to copy: 
     - **Draft issues** (issues not yet added to the repository)
     - **Automation workflows**
     - **Custom fields**

4. **Configure Your Copy**
   - Choose the owner (your personal account or organization)
   - Name your new project
   - Select the repository to link it with
   - Click **"Copy project"**

5. **Verify the Copy**
   - Navigate to your newly created project
   - Confirm all views, fields, and configurations are present

> **💡 Tip:** When copying a project, all views and custom fields are duplicated, but actual issues are not copied. You'll need to create new issues in your repository. 

---

## 2. Creating Issues and Sub-Issues

### Creating a Standard Issue

1. **From the Repository**
   - Navigate to the **Issues** tab in your repository
   - Click **"New Issue"**
   - Add a clear, descriptive title
   - Provide details in the description (use Markdown for formatting)
   - Add labels, assignees, and link to project
   - Fill the Fields of the issue according to the your understanding. For more information on the fields, please look into [Understanding Issue Field Options](#3-understanding-issue-field-options)
   - Click **"Submit new issue"**

2. **From the Project Board**
   - In any project view, click **"+ Add item"** at the bottom
   - Type your issue title and press Enter
   - Click on the issue to add more details
   - The issue will automatically link to your repository

### Creating Sub-Issues (Child Issues)

Sub-issues help break down larger tasks (User Stories, Epics) into smaller, manageable work items. 

#### Method 1: Using the Issue Sidebar

1. **Open a Parent Issue**
   - Navigate to the issue that will be the parent

2. **Add Sub-Issue**
   - In the right sidebar, find the **"Sub-issues"** section
   - Click **"Add sub-issue"**
   - Choose **"Create new issue"** or **"Add existing issue"**

3. **Create New Sub-Issue**
   - Enter the sub-issue title
   - Select the repository (if working across multiple repos)
   - Click **"Create"**

4. **View Relationships**
   - The parent issue will show all sub-issues listed
   - Sub-issues will show their parent relationship

#### Method 2: Converting Tasks to Issues

1. **Add Task List to Parent Issue**
   - Edit your parent issue description
   - Add a task list using Markdown: 
     ```markdown
     - [ ] Task 1
     - [ ] Task 2
     - [ ] Task 3
     ```

2. **Convert to Issue**
   - Hover over any task item
   - Click the **"Convert to issue"** button (circular icon)
   - This creates a linked sub-issue

#### Sub-Issue Best Practices

- **User Story → Tasks**:  Break user stories into technical tasks
- **Epic → User Stories**: Decompose epics into user stories
- **Limit Depth**: Try to keep hierarchy to 2-3 levels maximum
- **Clear Naming**: Use prefixes like `[Parent]`, `[Story]`, `[Task]` for clarity
- **Track Progress**: Parent issues automatically show completion percentage based on sub-issues

---

## 3. Understanding Issue Field Options

GitHub Projects allows custom fields to track various aspects of your work.  Here are the typical fields used in SCRUM:

### Standard Fields

#### **Status**
Tracks the current state of the issue through the workflow:
- **📝 Todo**: Ready to be worked on in the current sprint
- **🏗️ In Progress**:  Actively being worked on
- **👀 Under Review**: Completed and awaiting review/QA
- **✅ Done**: Completed and accepted
- **❌ Blocked**: This has been blocked by dependencies or other priorities

#### **Priority**
Indicates the urgency and importance of the work:
- **🔴 Critical/P1**:  Blockers, production issues, must be done immediately
- **🟠 High/P2**: Important features, should be done soon
- **🟡 Medium/P3**: Standard priority, planned work
- **🟢 Low/P4**: Nice to have, can be deferred
- **⚪ None**:  Not yet prioritized

*Use the MoSCoW method:  Must have, Should have, Could have, Won't have*

#### **Size**
Estimates the complexity and effort required (Fibonacci sequence):
- **S**:  Small feature, ~1 day
- **M**: Medium feature, 2-3 days
- **L**: Large feature, ~1 week

*Size is relative estimate, not absolute time*

#### **Hours (Estimated/Actual)**
- **Estimated Hours**: Initial time estimate
- **Actual Hours**:  Time actually spent (for tracking velocity)
- Use for capacity planning and burndown tracking

#### **Sprint**
Tracks which sprint the issue belongs to:
- **Sprint 1, Sprint 2, etc.**
- Typically 1-2 weeks per sprint
- Use sprint field to filter current work

#### **Assignee**
The team member responsible for the issue:
- Can assign multiple people
- Helps with workload distribution
- Makes accountability clear

#### **Labels**
Categorize issues by type, component, or theme:
- **Type**: `bug`, `feature`, `enhancement`, `documentation`
- **Component**: `frontend`, `backend`, `database`, `API`
- **Theme**: `security`, `performance`, `ux`, `infrastructure`

---

## 4. Assigning Issues to Team Members

### How to Assign Issues

#### From the Issue Page: 

1. **Open the Issue**
   - Click on the issue from the project board or repository

2. **Find Assignees Section**
   - Look in the right sidebar for **"Assignees"**

3. **Add Assignees**
   - Click on **"Assignees"**
   - Start typing the GitHub username
   - Select the user from the dropdown
   - You can assign up to 10 people per issue

4. **Save Changes**
   - The assignment is saved automatically

#### From the Project Board:

1. **Open Item in Project**
   - Click the issue in any project view

2. **Set Assignee Field**
   - Find the **"Assignees"** field in the side panel
   - Click and select user(s)

3. **Bulk Assignment**
   - Select multiple issues (hold Ctrl/Cmd)
   - Use bulk edit menu to assign to same person

### Assignment Best Practices

- **Single Owner**: For accountability, prefer one primary assignee
- **Pair Programming**: Assign two people for complex tasks
- **Workload Balance**: Check each person's current assignments
- **Skills Match**: Assign based on expertise and learning goals
- **Sprint Planning**: Assign all sprint issues during sprint planning meeting
- **Self-Assignment**: Allow team members to self-assign during standup

### Viewing Assignments

- **Personal View**: Filter to show only your assigned issues
- **Team View**: Group by assignee to see workload distribution
- **Unassigned Filter**: Find issues that need owners

---

## 5. Project Views Explained

This template uses five focused views aligned with SCRUM. Configure them as below to match the attached views.

### View 1: **Board**

**Purpose**: Track day-to-day sprint work on a simple board

**Layout**: Board or Table grouped by Status

**Columns**:
- Title
- Assignees
- Status
- Priority
- Size
- Hours
- Iteration
- Linked pull requests
- Sub-issues progress

**Filters**:
- `status:! Done`
- Optional: `iteration:current`

**Use Cases**:
- Daily standups
- Visual workflow management
- Bottleneck identification

**Configuration**:
```
Group by: Status
Sort by: Priority, then Size
Filter: status:! Done AND iteration:current
Columns: Title, Assignees, Status, Priority, Size, Hours, Iteration, Linked pull requests, Sub-issues progress
```

### View 2: **Team Workload**

**Purpose**: Understand workload, capacity, and dates by assignee

**Layout**: Table grouped by Assignees

**Columns**:
- Title
- Assignees
- Status
- Hours
- Iteration
- Start date
- Target date
- Linked pull requests
- Sub-issues progress

**Filters**:
- `iteration:current` (adjust as needed)

**Use Cases**:
- Capacity planning
- Balancing workload across the team
- Tracking start/target dates

**Configuration**:
```
Group by: Assignees
Sort by: Target date
Filter: iteration:current
Columns: Title, Assignees, Status, Hours, Iteration, Start date, Target date, Linked pull requests, Sub-issues progress
```

### View 3: **Current Iteration**

**Purpose**: Focus only on items in the active iteration

**Layout**: Table

**Columns**:
- Title
- URL (optional)
- Assignees
- Status
- Linked pull requests
- Sub-issues progress

**Filters**:
- `iteration:current`
- Optional: `status:! Done`

**Use Cases**:
- Sprint execution and tracking
- Preparing for sprint review

**Configuration**:
```
Group by: None (flat list)
Sort by: Status, then Title
Filter: iteration:current AND status:! Done
Columns: Title, URL, Assignees, Status, Linked pull requests, Sub-issues progress
```

### View 4: **Roadmap**

**Purpose**: High-level planning and tracking of larger items

**Layout**: Table (Timeline optional if you add dates)

**Columns**:
- Title
- Assignees
- Status

**Filters**:
- Optional: `status:! Done` to focus on active work

**Use Cases**:
- Release planning
- Stakeholder updates
- Epic progress overview

**Configuration**:
```
Group by: None
Sort by: Title
Filter: status:! Done
Columns: Title, Assignees, Status
```

### View 5: **My Items**

**Purpose**: Personal focus view for an individual contributor

**Layout**: Table filtered to your assignments

**Columns**:
- Title
- Priority
- Size
- Hours
- Iteration
- Linked pull requests
- Sub-issues progress

**Filters**:
- `assignee:@me`
- Optional: `status:! Done`

**Use Cases**:
- Daily planning
- Reviewing personal workload within the sprint

**Configuration**:
```
Group by: Status (optional)
Sort by: Priority
Filter: assignee:@me AND status:! Done
Columns: Title, Priority, Size, Hours, Iteration, Linked pull requests, Sub-issues progress
```

---

## 6. SCRUM Best Practices

### Sprint Planning

1. **Review Backlog**:  Ensure stories are refined and estimated
2. **Set Sprint Goal**: Define clear objective for the sprint
3. **Capacity Planning**: Calculate team capacity (story points)
4. **Select Issues**: Pull highest priority items that fit capacity
5. **Break Down Issues**: Create sub-issues for each story
6. **Assign Work**: Team members commit to specific issues

### Daily Standup

Use the **Sprint Board** view: 
- What did you complete yesterday?
- What will you work on today?
- Any blockers or dependencies?

Update issue statuses in real-time during standup. 

### Sprint Review

1. **Demo Completed Work**: Show work marked as Done
2. **Update Documentation**: Ensure README and docs are updated
3. **Collect Feedback**: Add comments to issues with feedback
4. **Accept or Reject**:  Move work to Done or back to In Progress

### Sprint Retrospective

1. **Review Metrics**: Velocity, burndown, completion rate
2. **Identify Improvements**: What went well, what to improve
3. **Action Items**: Create issues for process improvements
4. **Update Workflow**: Adjust project board if needed

### Backlog Refinement

1. **Regular Sessions**: Weekly refinement meetings
2. **Add Details**:  Expand issue descriptions and acceptance criteria
3. **Estimate Work**: Add story points to issues
4. **Prioritize**:  Reorder backlog based on value
5. **Split Large Items**: Break down issues >13 points

---

## 7. Additional Notes

### Tips for Success

- **Keep Issues Small**:  Aim for issues that take 1-3 days maximum
- **Clear Acceptance Criteria**: Define "done" for each issue
- **Regular Updates**: Comment on progress, blockers, and questions
- **Use Labels**: Consistent labeling helps filtering and reporting
- **Link Related Work**: Use keywords like "fixes #123" in commits
- **Archive Old Sprints**: Keep project board clean and focused

### Common Workflows

#### Bug Workflow
```
1. Bug reported → Create issue with `bug` label
2. Triage → Set priority (Critical bugs skip sprint planning)
3. Sprint Planning → Add to sprint if fits
4. Fix → Assign, develop, test
5. Review → Code review and QA
6. Done → Close issue, deploy fix
```

#### Feature Workflow
```
1. Feature request → Create epic/story
2. Refinement → Add details, break into sub-issues
3. Estimation → Add story points
4. Prioritization → Move to appropriate spot in backlog
5. Sprint Planning → Pull into sprint
6. Development → Move through workflow
7. Review → Demo and acceptance
8. Done → Close and document
```

### Automation Ideas

GitHub Projects supports automation workflows: 

- **Auto-add to project**:  New issues automatically added
- **Status transitions**: Move to "In Progress" when PR created
- **Close on merge**: Move to "Done" when PR merges
- **Stale issue management**: Label and close old issues

### Integration with Pull Requests

- **Link PRs to Issues**: Use "Closes #X" in PR description
- **Draft PRs**:  Keep status "In Progress" for draft PRs
- **Review Status**: Move to "In Review" when PR ready
- **Merge and Close**: Auto-move to Done on merge

---

## License

This project template is available under the MIT License. Feel free to customize and adapt to your team's needs. 

---

**Happy Sprint Planning!  🚀**
