# File Creation Process

**Process ID**: PROC001  
**Purpose**: Systematic file creation with automatic registry updates and linking  
**Integration**: Part of strategic initiation system  

## 🔧 **AUTOMATIC REGISTRY & LINKING REQUIREMENTS**

### **For Any New File Creation**
When creating any project file, **automatically**:

1. **Identify File Type**: Epic, Story, Task, Analysis, Plan, or other
2. **Add to Registry**: Update appropriate registry (epic-registry.md, story-registry.md, task-registry.md, plans-registry.md, analysis-registry.md)
3. **Establish Relationships**: Link file to appropriate task/story/epic hierarchy
4. **Update Cross-References**: Add bidirectional links in related files
5. **Document in Active Work**: Update active-work.md if file affects current priorities

### **Registry Update Templates**

#### **New Task Creation**
```markdown
# In task-registry.md
| T### | S### | Task Name | Status | Priority | Effort | Dependencies | Owner | Due Date |

# In task file
- **Story**: S### - Story Name
- **Epic**: E### - Epic Name  
```

#### **New Plan Creation**
```markdown  
# In plans-registry.md
| P### | T### | S### | E### | Plan Name | Status | Created | Owner |

# In plan file
- **Task**: T### - Task Name
- **Story**: S### - Story Name
- **Epic**: E### - Epic Name
```

#### **New Analysis Creation**
```markdown
# In analysis-registry.md  
| T###-analysis | T### | S### | E### | Analysis Name | Status | Created | Owner |

# In analysis file
- **Task**: T### - Task Name
- **Story**: S### - Story Name  
- **Epic**: E### - Epic Name
```

## 📋 **INTEGRATION WITH EXISTING PROCESSES**

### **Strategic Initiation Update**
Add to STRATEGIC-INITIATION-SYSTEM.md Phase 2:
```markdown
### Step 2D: File Creation Process Validation
**Purpose**: Ensure all new files follow systematic creation process
**Validation**: Check that registries are updated and relationships established
```

### **File Cleanup Process Update**
Add to existing cleanup process:
```markdown
### Registry Validation & Cleanup
- Verify all files exist that are referenced in registries
- Remove registry entries for deleted/archived files
- Validate task/story/epic relationships are maintained
- Archive completed work items from active registries
```

## ⚠️ **PROCESS ENFORCEMENT**

### **Quality Gates**
- **No orphaned files**: Every project file must be in appropriate registry
- **No broken links**: All task/story/epic relationships must be valid
- **Registry consistency**: Registry entries must match actual files
- **Active work accuracy**: active-work.md must reflect current registry state

### **Violation Recovery**
If file creation process not followed:
1. **Immediate correction**: Add missing registry entries and links
2. **Relationship establishment**: Connect orphaned files to appropriate hierarchy
3. **Process review**: Understand why process was missed
4. **Prevention**: Update process to prevent similar issues

---

**Process Status**: DEFINED - Ready for integration with strategic initiation
**Next Action**: Integrate with strategic initiation system and file cleanup process
**Enforcement**: All future file creation must follow this process automatically
