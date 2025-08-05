# Know-Base-MCP Project Management System

**Purpose**: Complete PM system with Epic > Story > Task hierarchy, analysis, and planning capabilities  
**Created**: August 04, 2025  
**Status**: ACTIVE PM SYSTEM - Use for all project work

## 📂 DIRECTORY STRUCTURE

```
pm/
├── README.md                    # This file - PM system overview and usage
├── templates/                   # Standardized templates for all PM artifacts
│   ├── epic-template.md         # Epic creation template
│   ├── story-template.md        # Story creation template  
│   ├── task-template.md         # Task creation template
│   ├── analysis-template.md     # Analysis framework template
│   └── plan-template.md         # Planning template
├── registry/                    # Master tracking and indexes
│   ├── epic-registry.md         # All epics with status
│   ├── story-registry.md        # All stories with relationships
│   ├── task-registry.md         # All tasks with dependencies
│   └── active-work.md           # Current sprint/active work view
├── epics/                       # Epic definitions and tracking
│   └── [EPIC-ID]-[NAME]/        # One directory per epic
├── stories/                     # Story definitions and tracking  
│   └── [STORY-ID]-[NAME]/       # One directory per story
├── tasks/                       # Task definitions and tracking
│   └── [TASK-ID]-[NAME]/        # One directory per task
├── analysis/                    # Analysis artifacts
│   └── [ITEM-ID]-analysis.md    # Analysis for epics/stories/tasks
└── plans/                       # Planning artifacts
    └── [ITEM-ID]-plan.md        # Execution plans for epics/stories/tasks
```

## 🎯 PM SYSTEM USAGE WORKFLOW

### **Creating New Work Items**

#### 1. Epic Creation Process
```bash
# Copy template and create epic directory
cp pm/templates/epic-template.md pm/epics/E001-epic-name/epic.md
cp pm/templates/analysis-template.md pm/analysis/E001-analysis.md
cp pm/templates/plan-template.md pm/plans/E001-plan.md

# Update epic registry
# Edit pm/registry/epic-registry.md to add new epic
```

#### 2. Story Creation Process  
```bash
# Copy template and create story directory
cp pm/templates/story-template.md pm/stories/S001-story-name/story.md
cp pm/templates/analysis-template.md pm/analysis/S001-analysis.md
cp pm/templates/plan-template.md pm/plans/S001-plan.md

# Update story registry and link to epic
# Edit pm/registry/story-registry.md to add new story
```

#### 3. Task Creation Process
```bash
# Copy template and create task directory  
cp pm/templates/task-template.md pm/tasks/T001-task-name/task.md
cp pm/templates/analysis-template.md pm/analysis/T001-analysis.md
cp pm/templates/plan-template.md pm/plans/T001-plan.md

# Update task registry and link to story
# Edit pm/registry/task-registry.md to add new task
```

### **Work Management Workflow**

#### Daily Workflow
1. **Check active work**: Review `pm/registry/active-work.md`
2. **Update task status**: Modify task files with progress
3. **Log blockers**: Document any impediments in task files
4. **Plan next actions**: Update task plans with next steps

#### Weekly Planning
1. **Review epic progress**: Check epic status and timeline
2. **Plan story work**: Break down stories into tasks
3. **Update registries**: Ensure all tracking is current
4. **Stakeholder communication**: Generate status reports from registries

### **Analysis & Planning Integration**

#### Analysis Framework
- **Epic Analysis**: Business value, stakeholder impact, success criteria
- **Story Analysis**: User value, technical approach, risk assessment  
- **Task Analysis**: Implementation approach, effort estimate, dependencies

#### Planning Framework
- **Epic Plan**: Timeline, resource allocation, milestone definition
- **Story Plan**: Technical approach, acceptance criteria, testing strategy
- **Task Plan**: Step-by-step execution, quality gates, completion criteria

## 🔄 PM SYSTEM INITIALIZATION FOR AI SESSIONS

### **Session Startup Commands**
Add to CLAUDE.md or session initialization:

```markdown
## PM SYSTEM USAGE
1. **Check active work**: Read pm/registry/active-work.md for current priorities
2. **Review blockers**: Check task files for impediments requiring attention
3. **Update progress**: Modify task status and log work completed
4. **Plan next actions**: Update task plans with next steps and decisions needed
```

### **Key Files to Load Each Session**
- `pm/registry/active-work.md` - Current sprint and priorities
- `pm/registry/epic-registry.md` - High-level project status
- Task files for any active work items

## 🧹 CLEANUP AND MAINTENANCE

### **Automated Cleanup Rules**
- **Completed items**: Move to `pm/archive/` after 30 days
- **Cancelled items**: Move to `pm/cancelled/` immediately
- **Old analysis**: Archive when superseded by newer versions
- **Stale plans**: Update or archive when no longer relevant

### **Monthly Maintenance Tasks**
- [ ] Archive completed epics/stories/tasks
- [ ] Clean up outdated analysis documents
- [ ] Update registry files for accuracy
- [ ] Review and optimize directory structure
- [ ] Generate lessons learned from completed work

## 📊 REGISTRY SYSTEM

### **Epic Registry Format**
| Epic ID | Name | Status | Progress | Start Date | Target End | Owner |
|---------|------|--------|----------|------------|------------|-------|
| E001 | Project Management | Active | 20% | 2025-08-04 | 2025-08-15 | Jon |

### **Story Registry Format**  
| Story ID | Epic | Name | Status | Progress | Dependencies | Owner |
|----------|------|------|--------|----------|--------------|-------|
| S001 | E001 | Create PM Capabilities | Active | 40% | None | Jon |

### **Task Registry Format**
| Task ID | Story | Name | Status | Priority | Effort | Dependencies | Owner |
|---------|-------|------|--------|----------|--------|--------------|-------|
| T001 | S001 | PM Requirements Analysis | Active | High | 4h | None | Jon |

## 🎯 SUCCESS CRITERIA

### **PM System Effectiveness**
- [ ] All work tracked in Epic > Story > Task hierarchy
- [ ] Every work item has analysis and plan artifacts
- [ ] Dependencies and blockers clearly documented
- [ ] Progress visible through registry system
- [ ] Easy migration path to database/web service

### **Database Migration Readiness**
- [ ] Standardized data structure in templates
- [ ] Consistent ID and naming conventions
- [ ] Relationship tracking between work items
- [ ] Historical data preservation approach
- [ ] Export/import capabilities defined

---

**NEXT STEPS**: Create templates and implement first Epic/Story/Task set for PM system requirements analysis
