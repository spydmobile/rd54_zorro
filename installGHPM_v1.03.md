# GitHub Project Management Setup for Drone Projects v1.03

**Purpose**: This document provides a complete prompt for Claude Code to set up a comprehensive GitHub-based project management system for your drone build project.

**What This Sets Up**:

- GitHub CLI installation and authentication
- Custom issue labels for drone project tracking
- GitHub Project board for visual task management (linked to repository)
- Kanban Board and Milestone Roadmap views
- Milestones for tracking major build goals
- Initial issues for pending work
- Documentation in your CLAUDE.md file
- View setup guide for project configuration

**Version History**:
- v1.03 (2025-11-17): Added project views setup (Kanban Board + Milestone Roadmap)
- v1.02 (2025-11-17): Added project-to-repository linking step
- v1.01 (2025-11-17): Initial release

---

## Prerequisites

Before starting, ensure:

- Your drone project is in a Git repository
- The repository has a GitHub remote configured
- You have a CLAUDE.md file (or are willing to create one)
- You're working on macOS (for Homebrew installation)

---

## The Prompt

Copy the text below and paste it into your Claude Code session:

---

### START OF PROMPT

I want you to set up a GitHub project management system for my drone build project. Please follow these steps:

### Step 1: Install and Configure GitHub CLI

1. Install GitHub CLI via Homebrew: `brew install gh`
2. Authenticate with GitHub: `gh auth login`
3. Request additional scopes for project management: `gh auth refresh -s project,read:project --hostname github.com`

### Step 2: Create Issue Labels

Create the following labels for my repository (replace `OWNER/REPO` with my actual GitHub repo):

**Task Type Labels**:

- `incident` (color: #d73a4a) - Crash reports and damage assessments
- `modification` (color: #0075ca) - Planned or in-progress modifications
- `parts-ordered` (color: #fbca04) - Parts ordered, awaiting delivery
- `pending-install` (color: #f9d0c4) - Parts received, awaiting installation
- `maintenance` (color: #d4c5f9) - Routine maintenance tasks
- `enhancement` (color: #a2eeef) - Improvements and upgrades

**Priority Labels**:

- `priority: critical` (color: #b60205) - Airworthiness/safety critical issues
- `priority: high` (color: #d93f0b) - Important but not safety critical

**Component Labels**:

- `video-system` (color: #c5def5) - FPV video system related
- `radio-system` (color: #bfdadc) - Radio/receiver related

Use the `gh label create` command for each label.

### Step 3: Create GitHub Project Board

1. Create a new project called "[MY DRONE NAME] Project Tracker" for my repository
2. Note the project number for future reference
3. Update the project with description and README:
   ```graphql
   mutation {
     updateProjectV2(input: {
       projectId: "PROJECT_ID"
       shortDescription: "Task tracking and milestone roadmap for [DRONE NAME]"
       readme: "# [DRONE NAME] Project\n\nTrack modifications, incidents, and build progress.\n\n## Views\n- **Kanban Board**: Status-based workflow\n- **Milestone Roadmap**: Timeline view of build goals\n- **All Items**: Complete table view"
     }) {
       projectV2 { id }
     }
   }
   ```
4. **Link the project to the repository** using the GitHub GraphQL API:
   - Get the repository node ID: `gh api graphql -f query='{repository(owner: "OWNER", name: "REPO") {id}}'`
   - Get the project node ID from the project creation output
   - Link them: `gh api graphql -f query='mutation {linkProjectV2ToRepository(input: {projectId: "PROJECT_NODE_ID", repositoryId: "REPO_NODE_ID"}) {repository {name}}}'`

### Step 4: Create Milestones

Create the following milestones using the GitHub API (`gh api`):

1. **Working Video** - FPV video system installed and operational
2. **Working GPS** - GPS system installed, configured, and acquiring satellites
3. **Ready To Fly** - All critical systems operational and airworthy
4. **Maiden Flight** - First successful flight by current operator

### Step 5: Create Initial Issues

Based on my drone's current status, create GitHub issues for:

- Any missing components (receiver, video system, etc.)
- Pending installations
- Known problems or needed repairs

For each issue:

- Assign appropriate labels
- Assign to the relevant milestone
- Assign to me (the repository owner)
- Add to the project board

### Step 6: Create Project View Setup Guide

Create a file called `GHPM_View_Setup_Guide.md` that provides step-by-step instructions for configuring project views through the GitHub web interface:

1. **Kanban Board View**: Instructions for creating a Board layout grouped by Status
2. **Milestone Roadmap View**: Instructions for creating a Roadmap layout grouped by Milestone
3. **View Management**: Tips for filters, sorting, and default view settings
4. **Workflow Automation**: Optional auto-archive and auto-add configurations

**Note**: GitHub Projects v2 does not expose view creation via GraphQL API, so views must be configured through the web interface. The guide should be comprehensive enough for quick (2-minute) setup.

### Step 7: Update CLAUDE.md

Add a comprehensive "GitHub Issues & Project Management" section to my CLAUDE.md file that documents:

1. **Dual-Track Documentation System**: Explain that we use both Markdown docs (comprehensive archive) and GitHub Issues (active task tracking)

2. **GitHub Project Structure**: Document the project board number, milestones, column structure, and available views (Kanban Board, Milestone Roadmap)

3. **Issue Label System**: List all labels and their purposes

4. **When to Create GitHub Issues**: Define when issues should be created (crashes, parts orders, modifications, bugs, maintenance)

5. **Issue Creation Workflow**: Step-by-step process for creating and documenting issues

6. **Integration Between Issues and Docs**: How to cross-reference between GitHub issues and Markdown documentation

7. **Common gh CLI Commands**: Provide a reference of frequently used commands including:
   - Creating issues with labels, assignee, and milestone
   - Listing issues by label or assignee
   - Updating issues
   - Closing issues
   - Adding issues to project board
   - Listing milestones

8. **Issue Lifecycle**: Explain the typical flow from creation to completion

9. **Best Practices**: Guidelines for issue titles, bodies, labels, and comments

10. **Milestone Assignment Guidelines**: Which types of issues go to which milestones

11. **Project Views**: Document available views and when to use each

Also update the "Future Claude Instances" section to remind future Claude sessions to check open GitHub issues when starting work.

### Step 8: Commit Changes

Create a git commit documenting the GitHub project management setup with an appropriate commit message.

### Step 9: Provide Summary

Give me a summary of:

- What was set up
- Project board number and URL
- Number of labels created
- Number of milestones created
- Number of initial issues created
- How to access the project in VS Code or GitHub web
- **Reminder**: Configure Kanban Board and Milestone Roadmap views using GHPM_View_Setup_Guide.md (~2 minutes)

### END OF PROMPT

---

## Expected Outcome

After running this prompt, you will have:

✓ GitHub CLI installed and authenticated
✓ Custom issue labels tailored for drone projects
✓ A GitHub Project board with description and README
✓ Project board linked to your repository for better integration
✓ Four milestones tracking major build goals
✓ Initial issues created for your pending work
✓ Complete documentation in CLAUDE.md for future Claude sessions
✓ GHPM_View_Setup_Guide.md for quick view configuration
✓ All changes committed to your repository

**Next Step**: Follow `GHPM_View_Setup_Guide.md` to configure Kanban Board and Milestone Roadmap views (~2 minutes via web interface).

---

## Quick View Setup

After running the automated setup, configure project views:

1. Open your project: `https://github.com/users/OWNER/projects/PROJECT_NUMBER`
2. Follow instructions in `GHPM_View_Setup_Guide.md` to create:
   - **Kanban Board** view (Board layout, grouped by Status)
   - **Milestone Roadmap** view (Roadmap layout, grouped by Milestone)
3. Set Kanban Board as default view
4. Done! Your project now has full kanban + roadmap workflow

**Why Manual Setup?** GitHub Projects v2 API does not expose view creation mutations. Views must be configured through the web UI, but the process is quick and well-documented in the guide.

---

## Customization Options

You can customize the setup by:

1. **Adding/Removing Labels**: Adjust the label list based on your project needs
2. **Changing Milestones**: Modify milestone names/descriptions for your specific goals
3. **Additional Components**: Add component-specific labels (flight-controller, esc, motors, etc.)
4. **Priority Levels**: Add medium/low priority labels if needed
5. **Project Views**: Create additional filtered views (by component, priority, etc.)
6. **Workflow Automation**: Enable auto-archive and auto-add in project settings

---

## Using the System

Once set up, Claude Code will automatically:

- Create GitHub issues when you report crashes, parts orders, or modifications
- Assign issues to you with appropriate labels and milestones
- Update Markdown documentation alongside GitHub issues
- Cross-reference between issues and documentation
- Track progress on the project board

You can access your issues and project board:

- **In VS Code**: GitHub Pull Requests and Issues extension (built-in)
- **On the Web**: <https://github.com/OWNER/REPO/issues> and <https://github.com/users/OWNER/projects/PROJECT_NUMBER>
- **Via CLI**: `gh issue list --repo OWNER/REPO` or `gh project view PROJECT_NUMBER --owner OWNER`

### Recommended Workflow

1. **Daily**: Check Kanban Board view for active tasks
2. **Weekly**: Review Milestone Roadmap to track progress toward goals
3. **On Crash/Issue**: Create GitHub issue + document in Markdown
4. **On Completion**: Close issue + update Markdown with results

---

## Maintenance

The system is self-maintaining through Claude Code, but you can:

- Review and close completed issues
- Drag issues between columns on Kanban Board
- Update milestone progress and due dates
- Add new labels or milestones as needed
- Create filtered views for specific workflows
- Enable workflow automation for auto-archiving completed items

---

## Support

This project management system was developed for drone build projects. Reference implementations:
- RD-53 "Bandit": <https://github.com/spydmobile/RD53_Bandit>
- RD-59 "Nazgul": <https://github.com/spydmobile/RD59_Nazgul>

For questions or improvements, refer to the CLAUDE.md file in your repository after setup.

---

**Pro Tip**: After setup and view configuration, ask Claude Code to "provide current status of [YOUR DRONE NAME]" to get a comprehensive status report including GitHub issue tracking, milestone progress, and airworthiness status from both the Kanban Board and Milestone Roadmap perspectives.
