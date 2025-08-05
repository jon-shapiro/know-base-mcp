# Session Management File Index

**Purpose**: Index of all session management files and their relationships
**Critical**: Ensures session continuity system integrity
**Updated**: When session files are modified

## 🔄 **SESSION FILE STRUCTURE**

```
session/
├── 00-session-handoff.md          # Strategic handoff (CRITICAL)
├── 02-strategic-context.md        # Strategic context preservation
├── 03-active-work-context.md      # Current work context
├── 04-git-state.md               # Git commands for next session (CRITICAL)
└── session-templates.md          # Session file templates
```

## 📋 **SESSION FILE RELATIONSHIPS**

### **Critical Session Files (Never Delete)**
| File | Purpose | Created By | Used By | Dependencies |
|------|---------|------------|---------|--------------|
| `00-session-handoff.md` | Strategic handoff between sessions | --end-session | --initiate | Strategic context |
| `04-git-state.md` | Git commands for session | --end-session | Human execution | Repository state |

### **Context Preservation Files**
| File | Purpose | Created By | Used By | Dependencies |
|------|---------|------------|---------|--------------|
| `02-strategic-context.md` | Strategic context preservation | --end-session | --initiate | Project strategy |
| `03-active-work-context.md` | Current work context | --end-session | --initiate | PM work items |

### **Template Files**
| File | Purpose | Created By | Used By | Dependencies |
|------|---------|------------|---------|--------------|
| `session-templates.md` | Templates for session files | Manual | --end-session | Session process |

## 🔧 **SESSION FILE MAINTENANCE**

### **Update Triggers**
- **Every --end-session**: Update all session files with current context
- **Work item changes**: Update 03-active-work-context.md
- **Strategic decisions**: Update 02-strategic-context.md and 00-session-handoff.md
- **Repository changes**: Update 04-git-state.md

### **Validation Rules**
- Session files must be written to disk (not just displayed)
- Git state file must contain executable commands
- Handoff file must contain strategic context for next session
- All session files must reference correct work item IDs from PM registry

---

**Index Status**: COMPLETE - Session management file organization documented
**Integration**: Works with existing PM registry system without duplication