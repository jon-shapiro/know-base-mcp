# Know-Base-MCP Initialization Commands

**Purpose**: Standard commands for AI session management and project operations  
**Created**: August 04, 2025  
**Updated**: August 04, 2025 - Session 02  
**Status**: ACTIVE - Use these commands for consistent project management

## 🚀 SESSION INITIALIZATION

### **Standard Session Startup**
```
INITIALIZE KNOW-BASE-MCP SESSION
Load complete project context:
1. Read CLAUDE.md (project memory)
2. Read STATUS.md (current state) 
3. Read pm/registry/active-work.md (current sprint)
4. Read latest session file in docs/context/sessions/
5. Review docs/decisions/decision-log.md for recent decisions
6. Load any task files for active work items
Current phase: VALIDATION (no development until stakeholder approval)
PM System: OPERATIONAL - use Epic/Story/Task hierarchy
Ready to continue work on validation framework and project management.
```

## 📋 PROJECT MANAGEMENT COMMANDS

### **--update-docs**
Update all README files and documentation to reflect current project state

**Process**:
1. Update main README.md with current status and action items
2. Update STATUS.md with latest progress and blockers
3. Update pm/registry/active-work.md with current sprint status
4. Update relevant Epic/Story/Task files with progress
5. Update docs/ README files for navigation clarity
6. Highlight outstanding stakeholder review items
7. Ensure all internal links work correctly
8. Update file inventory if new files created

**Output**: "Documentation updated. Outstanding items for stakeholder review: [LIST]"

### **--create-epic [EPIC_NAME]**
Create new epic using standardized template

**Process**:
1. Copy pm/templates/epic-template.md to pm/epics/E###-epic-name/epic.md
2. Copy pm/templates/analysis-template.md to pm/analysis/E###-analysis.md
3. Copy pm/templates/plan-template.md to pm/plans/E###-plan.md
4. Update pm/registry/epic-registry.md with new epic
5. Update pm/registry/active-work.md if epic is current priority

### **--create-story [STORY_NAME] [EPIC_ID]**
Create new story using standardized template

**Process**:
1. Copy pm/templates/story-template.md to pm/stories/S###-story-name/story.md
2. Copy pm/templates/analysis-template.md to pm/analysis/S###-analysis.md
3. Copy pm/templates/plan-template.md to pm/plans/S###-plan.md
4. Update pm/registry/story-registry.md with new story
5. Update epic file to reference new story
6. Update pm/registry/active-work.md if story is current priority

### **--create-task [TASK_NAME] [STORY_ID]**
Create new task using standardized template

**Process**:
1. Copy pm/templates/task-template.md to pm/tasks/T###-task-name/task.md
2. Copy pm/templates/analysis-template.md to pm/analysis/T###-analysis.md
3. Copy pm/templates/plan-template.md to pm/plans/T###-plan.md
4. Update pm/registry/task-registry.md with new task
5. Update story file to reference new task
6. Update pm/registry/active-work.md if task is current priority

### **--update-progress [ITEM_ID] [STATUS] [PROGRESS_%]**
Update progress on Epic/Story/Task

**Process**:
1. Update specific work item file with new status and progress
2. Update relevant registry file (epic/story/task)
3. Update pm/registry/active-work.md if item is active
4. Update parent items (story for task, epic for story) with aggregated progress
5. Log progress update in time tracking section

### **--complete-item [ITEM_ID]**
Mark Epic/Story/Task as complete

**Process**:
1. Update work item file status to COMPLETE
2. Set actual end date
3. Update all registry files
4. Update parent items with completion
5. Remove from active work if applicable
6. Archive item if cleanup policy indicates

## 📊 REPORTING COMMANDS

### **--status-report**
Generate current project status report

**Output**:
- Current phase and progress percentage
- Active work items and owners
- Blockers and issues requiring attention
- Upcoming milestones and deadlines
- Stakeholder action items

### **--sprint-summary**
Generate current sprint summary

**Output**:
- Sprint goal and progress
- Completed work this sprint
- Active work and next actions
- Blockers and risks
- Velocity and timeline status

### **--stakeholder-actions**
List all items requiring stakeholder (Jon) action

**Output**:
- Critical items with deadlines
- High priority items
- Medium priority items
- Decision points requiring input

## 📝 SESSION MANAGEMENT COMMANDS

### **--end-session**
Properly close current session and prepare for next session with strategic continuity

**Process**:
1. **Strategic Work Analysis**:
   - Analyze work completed and its strategic impact on Epic/Story/Task
   - Identify strategic insights and learnings that change project understanding
   - Document strategic value created and evidence generated
   - Assess progress toward strategic decision points

2. **Git Command Generation**:
   - Check current git status (uncommitted files, branch state, remote sync)
   - Generate commit message based on strategic work completed using `git add .`
   - Create `session/04-git-state.md` with exact git commands for human execution
   - Include commit message context and expected final state
   - **DO NOT EXECUTE**: Commands are for human execution only

3. **Strategic Context Generation**:
   - Update strategic understanding based on session learnings
   - Identify strategic decisions or pivots discovered during session
   - Document changes to project hypothesis or strategic approach
   - Generate strategic context for next session handoff

4. **Session Handoff Creation**:
   - Create `session/00-session-handoff.md` with complete strategic context
   - Update `session/02-strategic-context.md` with current strategic position
   - Update `session/03-active-work-context.md` with current work status
   - Generate strategic initiation command for next session

5. **Stakeholder Communication Preparation**:
   - Identify new items requiring stakeholder review and approval
   - Update stakeholder action items with strategic context
   - Prepare strategic progress updates for stakeholder communication
   - Document strategic decisions requiring stakeholder input

6. **Strategic Continuity Validation**:
   - Ensure all strategic context captured for perfect session continuity
   - Validate that next session can resume with full strategic awareness
   - Confirm git state commands are accurate and complete
   - Verify strategic decision tracking is complete
   - **ALWAYS provide full initiate file path**: `/Users/jon/git/know-base-mcp/initiate.md`
   - **ALWAYS write session files to disk** using filesystem tools
   - **ALWAYS output complete git commit commands** for manual execution

**Output**: 
- "Session ended with strategic continuity established. Next session priorities: [STRATEGIC FOCUS]"
- **Full initiate path**: `/Users/jon/git/know-base-mcp/initiate.md`
- Strategic initiation command: `INITIALIZE KNOW-BASE-MCP SESSION STRATEGIC-VALIDATION-MODE`
- **Complete git commands** in session/04-git-state.md for repository synchronization
- **All session files written to disk** in session/ directory

### **--session-handoff [NOTES]**
Prepare handoff for different team member

**Process**:
1. Update all progress tracking
2. Document current context and decisions
3. Highlight blockers and dependencies
4. Create clear next actions list
5. Update stakeholder communication items

## 🎯 DECISION MANAGEMENT COMMANDS

### **--log-decision [DECISION] [RATIONALE]**
Record important project decision

**Process**:
1. Add decision to docs/decisions/decision-log.md
2. Include alternatives considered
3. Document rationale and impact
4. Reference supporting analysis if available
5. Update relevant work items

## 🧹 MAINTENANCE COMMANDS

### **--cleanup-workspace**
Perform routine maintenance

**Process**:
1. Archive completed work items
2. Clean up outdated analysis files
3. Update file inventory
4. Check for broken links
5. Validate registry consistency

### **--cleanup-junk**
Remove unnecessary files that accumulate during development

**Process**:
1. Remove .delete files created during cleanup
2. Remove .backup files older than 7 days
3. Clean up any orphaned analysis/plan files
4. Remove duplicate or test files
5. Report what was cleaned up

**Example**: --cleanup-junk
**Output**: "Cleaned up X junk files. Repository hygiene maintained."

### **--archive-completed**
Clean up completed work items

**Process**:
1. Create pm/archive/YYYY-MM/ directory if needed
2. Move completed items older than 30 days to archive
3. Update registry files to reflect archived items
4. Clean up pm/registry/active-work.md
5. Update file inventory

## 🔗 INTEGRATION COMMANDS

### **--git-commit [MESSAGE]**
Standardized git commit with project context

**Process**:
1. Add all relevant files
2. Create structured commit message
3. Include progress update summary
4. Reference work items completed
5. Tag with phase/milestone if applicable

---

## 🎯 COMMAND USAGE EXAMPLES

```bash
# Start new session
INITIALIZE KNOW-BASE-MCP SESSION

# Update all documentation
--update-docs

# Create new work items
--create-epic "Cannabis Content Migration"
--create-story "Unity Landing Integration" E002
--create-task "Repository Analysis" S005

# Update progress
--update-progress T001 COMPLETE 100%
--complete-item T001

# Generate reports
--status-report
--stakeholder-actions

# End session with full closure
--end-session
```

---

**Usage Note**: These commands provide structured interaction patterns for AI sessions while maintaining project consistency and quality. Always use --end-session to properly close sessions and get next session initiate command plus git sync commands.
