# GitHub Labels Configuration

This file documents the labels used in this repository for issue management and backlog refinement.

## Label Definitions

### Priority Labels
- `priority-high` (🔴 #d73a4a) - Critical items that must be completed
- `priority-medium` (🟡 #fbca04) - Important items for current sprint
- `priority-low` (🟢 #0e8a16) - Nice to have items

### Type Labels  
- `enhancement` (🟦 #0052cc) - New features or improvements that add customer value
- `technical-debt` (🟡 #fbca04) - Code improvements with no direct customer value
- `bug` (🔴 #d73a4a) - Something isn't working correctly
- `user-story` (🟪 #8b5cf6) - Product backlog items with user value

### Process Labels
- `sprint-ready` (🟢 #0e8a16) - Story has sufficient detail for sprint planning
- `needs-refinement` (🟠 #ff9500) - Story needs more details before sprint planning
- `blocked` (⚫ #000000) - Cannot proceed due to dependencies
- `in-progress` (🔵 #0052cc) - Currently being worked on

### Component Labels
- `api` (🟦 #1d76db) - Related to REST API endpoints
- `database` (🟫 #8b4513) - Database related changes
- `testing` (🟣 #663399) - Test related work
- `documentation` (📝 #ffffff) - Documentation updates
- `devops` (🔧 #2ea043) - CI/CD, deployment, infrastructure

## GitHub CLI Commands to Create Labels

If you have GitHub CLI installed, you can create these labels with:

```bash
# Technical debt label (yellow)
gh label create "technical-debt" --description "Code improvements with no direct customer value" --color "fbca04"

# Sprint ready label (green)  
gh label create "sprint-ready" --description "Story has sufficient detail for sprint planning" --color "0e8a16"

# Priority labels
gh label create "priority-high" --description "Critical items that must be completed" --color "d73a4a"
gh label create "priority-medium" --description "Important items for current sprint" --color "fbca04" 
gh label create "priority-low" --description "Nice to have items" --color "0e8a16"

# Process labels
gh label create "needs-refinement" --description "Story needs more details" --color "ff9500"
gh label create "blocked" --description "Cannot proceed due to dependencies" --color "000000"
gh label create "in-progress" --description "Currently being worked on" --color "0052cc"
```
