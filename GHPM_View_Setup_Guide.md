# GitHub Project Views Setup Guide
# RD-54 Zorro Project Tracker

**Project**: RD-54 Zorro Project Tracker (Project #15)
**Project URL**: https://github.com/users/spydmobile/projects/15
**Setup Time**: ~2 minutes
**Last Updated**: November 19, 2025

---

## Overview

This guide provides step-by-step instructions for configuring project views through the GitHub web interface. GitHub Projects v2 does not expose view creation via GraphQL API, so views must be configured manually.

You will create:
1. **Kanban Board** - Status-based workflow (Board layout)
2. **Milestone Roadmap** - Timeline view of build goals (Roadmap layout)

---

## Prerequisites

- GitHub project created and linked to repository ✓
- Repository issues created ✓
- Milestones created ✓

---

## Step 1: Access Your Project

1. Navigate to: https://github.com/users/spydmobile/projects/15
2. You should see the default "All Items" table view

---

## Step 2: Create Kanban Board View

### 2.1 Create New View

1. Click the **"+"** button next to the current view tabs (top of project)
2. Select **"New view"**
3. Choose **"Board"** layout
4. Name it: **"Kanban Board"**
5. Click **"Create"**

### 2.2 Configure Board Grouping

1. In the Kanban Board view, click **"..."** (view options menu)
2. Select **"Group by"**
3. Choose **"Status"**

The board will now show columns: **Todo**, **In Progress**, **Done**

### 2.3 Configure Board Filters (Optional)

To hide closed issues:

1. Click **"Filter"** at the top
2. Add filter: `is:open`
3. This keeps the board focused on active work

### 2.4 Board Usage

- **Drag issues** between columns to change status
- **Click an issue** to view details and add comments
- **Use labels** for additional categorization
- **Filter by milestone** to see progress toward specific goals

---

## Step 3: Create Milestone Roadmap View

### 3.1 Create New View

1. Click the **"+"** button next to view tabs
2. Select **"New view"**
3. Choose **"Roadmap"** layout
4. Name it: **"Milestone Roadmap"**
5. Click **"Create"**

### 3.2 Configure Roadmap Grouping

1. In the Milestone Roadmap view, click **"..."** (view options menu)
2. Select **"Group by"**
3. Choose **"Milestone"**

The roadmap will now show swim lanes for each milestone:
- Working Video
- Working GPS
- Ready To Fly
- Maiden Flight

### 3.3 Configure Roadmap Timeline

The roadmap will automatically display:
- **Start dates** (issue creation date)
- **Due dates** (milestone due dates, when set)
- **Progress bars** showing completion percentage per milestone

### 3.4 Roadmap Usage

- **Drag issues** horizontally to adjust timelines
- **Drag issues** vertically to reassign milestones
- **Click milestones** to view/edit milestone details
- **Set milestone due dates** for better timeline visualization

---

## Step 4: Set Default View

1. Navigate to your preferred view (Kanban Board recommended)
2. Click **"..."** (view options menu)
3. Select **"Set as default view"**

Now when you open the project, you'll land on your preferred view.

---

## Step 5: Configure Workflow Automation (Optional)

### Auto-Archive Closed Issues

1. Go to project **Settings** (gear icon, top right)
2. Navigate to **"Workflows"** section
3. Enable **"Auto-archive items"**
4. Configure: Archive items when **"Status"** is set to **"Done"**

This automatically removes completed issues from active views while preserving them in the project.

### Auto-Add New Issues

1. In project **Settings** → **"Workflows"**
2. Enable **"Auto-add to project"**
3. Configure: Automatically add issues from **spydmobile/rd54_zorro**
4. Optional: Filter by labels (e.g., only add issues with specific labels)

This automatically adds new repository issues to your project.

---

## Available Views Summary

After completing this guide, you'll have:

| View Name | Layout | Grouped By | Purpose |
|-----------|--------|------------|---------|
| **All Items** | Table | None | Complete list of all issues with full details |
| **Kanban Board** | Board | Status | Active workflow management (Todo → In Progress → Done) |
| **Milestone Roadmap** | Roadmap | Milestone | Timeline view of build progress toward major goals |

---

## View Selection Guide

**Use Kanban Board when**:
- Working on daily tasks
- Prioritizing what to work on next
- Moving issues through workflow stages
- Quick status updates

**Use Milestone Roadmap when**:
- Planning long-term build goals
- Tracking progress toward major milestones
- Understanding project timeline
- Identifying blockers to airworthiness

**Use All Items when**:
- Searching for specific issues
- Bulk editing multiple issues
- Generating reports
- Reviewing complete project history

---

## Customization Tips

### Creating Additional Views

You can create unlimited custom views:

1. **By Component**: Filter by `video-system` or `radio-system` labels
2. **By Priority**: Filter by `priority: critical` or `priority: high`
3. **By Assignee**: Filter by assignee for multi-operator fleets
4. **By Label**: Create views for `incident`, `modification`, `maintenance`, etc.

### Advanced Filters

Combine filters for powerful views:

- `is:open label:priority:critical` - Open critical issues only
- `is:open milestone:"Working Video"` - Active video system tasks
- `is:closed closed:>2024-11-01` - Recently completed work
- `label:incident` - All crash reports and incidents

### Sorting and Display

- **Sort by**: Priority, creation date, update date, assignee
- **Show/hide fields**: Customize visible columns in table view
- **Field widths**: Resize columns to optimize display

---

## Maintenance

Your project views are now configured! Regular maintenance:

- **Weekly**: Review Kanban Board, move issues through workflow
- **Monthly**: Review Milestone Roadmap, update milestone due dates
- **As needed**: Create filtered views for specific workflows
- **After flight**: Update issues with test results and close completed items

---

## Troubleshooting

**Issues not appearing in project?**
- Check if auto-add workflow is enabled
- Manually add: Open issue → Click "Projects" on right sidebar → Select "RD-54 Zorro Project Tracker"

**Roadmap not showing timeline?**
- Set milestone due dates for timeline visualization
- Check that issues are assigned to milestones

**Board columns not showing?**
- Verify "Group by: Status" is selected
- Check that issues have status field populated

**Can't find a view?**
- Use view tabs at top of project
- Check if view was accidentally deleted (recreate using this guide)

---

## Next Steps

1. ✓ Configure Kanban Board view
2. ✓ Configure Milestone Roadmap view
3. ✓ Set default view
4. ✓ Enable workflow automation (optional)
5. Start using the project!

Open your project: https://github.com/users/spydmobile/projects/15

---

## Reference

- **Project Number**: 15
- **Project ID**: PVT_kwHOABBD-s4BIifE
- **Repository**: spydmobile/rd54_zorro
- **Milestones**: 4 (Working Video, Working GPS, Ready To Fly, Maiden Flight)
- **Initial Issues**: 7 (created November 19, 2025)

For detailed issue management workflows, see `CLAUDE.md` → GitHub Issues & Project Management section.

---

**Document Version**: 1.0
**Created**: November 19, 2025
**RD-54 Archivist**: Claude Code
