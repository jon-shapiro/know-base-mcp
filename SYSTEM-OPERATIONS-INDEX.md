# System Commands & Operations File Index

**Purpose**: Index of all system operation files (commands, initialization, setup)
**Critical**: Ensures system operations integrity and prevents command conflicts
**Updated**: When command files are modified

## ⚙️ **SYSTEM OPERATIONS STRUCTURE**

```
/ (root level)
├── COMMANDS.md                    # All system commands (CRITICAL)
├── STRATEGIC-INITIATION-SYSTEM.md # Initiation process (CRITICAL)
├── initiate.md                   # Initiation instructions
├── CLAUDE.md                     # AI system memory
├── STATUS.md                     # Project status
├── GIT-SETUP.md                  # Git configuration
└── INITIALIZE.md                 # System initialization
```

## 📋 **SYSTEM COMMAND FILES**

### **Core Command System (Never Delete)**
| File | Purpose | Contains | Dependencies | Update Triggers |
|------|---------|----------|--------------|-----------------|
| `COMMANDS.md` | All system commands | --end-session, --update-docs, --cleanup-junk, etc. | Session system, PM system | Command changes |
| `STRATEGIC-INITIATION-SYSTEM.md` | Strategic initiation process | Phase 1-4 initiation steps | Session files, PM registry | Initiation process changes |
| `initiate.md` | Initiation instructions | Command reference, context | Strategic initiation system | Process updates |

### **System Context Files**
| File | Purpose | Contains | Dependencies | Update Triggers |
|------|---------|----------|--------------|-----------------|
| `CLAUDE.md` | AI system memory | Project context, key decisions | All project operations | Major project changes |
| `STATUS.md` | Project status | Current state, blockers | Work items, decisions | Status changes |

### **Setup & Configuration Files**
| File | Purpose | Contains | Dependencies | Update Triggers |
|------|---------|----------|--------------|-----------------|
| `GIT-SETUP.md` | Git configuration | Git setup instructions | Repository operations | Git process changes |
| `INITIALIZE.md` | System initialization | Setup procedures | System requirements | Setup process changes |

## 🔧 **COMMAND SYSTEM MAINTENANCE**

### **Command Dependencies**
- **--end-session** → Requires session/ directory and templates
- **--initiate** → Requires pm/WORK-ITEM-REGISTRY.md and session files
- **--cleanup-junk** → Requires file system access
- **--update-docs** → Requires all documentation files

### **Critical Integration Points**
- COMMANDS.md references session management system
- Strategic initiation loads PM registry to prevent ID confusion
- All commands must maintain file index accuracy

### **Update Rules**
- New commands must be added to COMMANDS.md with full specification
- Command changes must update dependent files
- System files must maintain backward compatibility with existing sessions

---

**Index Status**: COMPLETE - System operations file organization documented  
**Integration**: Coordinates with PM registry and session management without duplication