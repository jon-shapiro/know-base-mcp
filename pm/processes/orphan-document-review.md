# Orphan Document Review Process

**Task ID**: T008-initiation-testing  
**Purpose**: Prevent document drift by regularly auditing task-document relationships  
**Frequency**: Weekly review during --end-session process  

## Weekly Orphan Document Audit

### **Step 1: Identify Orphan Documents**
```bash
# Search for documents without task ID headers
grep -r "Task ID" . --include="*.md" -L
```

### **Step 2: Orphan Document Checklist**
- [ ] **Analysis documents**: All analysis files have task references
- [ ] **Plan documents**: All implementation plans linked to tasks  
- [ ] **Implementation documents**: All code/system docs linked to tasks
- [ ] **Review documents**: All assessment docs linked to originating tasks
- [ ] **Template documents**: Exception - templates don't need task links
- [ ] **README/Navigation documents**: Exception - structural docs

### **Step 3: Link or Archive Orphan Documents**
For each orphan document:
- [ ] **Identify related task**: Which task does this document serve?
- [ ] **Add task header**: Use task-linked-document-template.md format
- [ ] **Update task files**: Reference document in task analysis/plan
- [ ] **Archive if obsolete**: Move to archive/ if no longer relevant

### **Step 4: Validate Task References**
- [ ] **Task IDs exist**: All referenced tasks exist in PM system
- [ ] **Epic/Story accuracy**: All Epic/Story references are current
- [ ] **Bidirectional links**: Tasks reference their documents
- [ ] **Status consistency**: Document status matches task status

## Orphan Prevention Guidelines

### **When Creating New Documents**
1. **Always start with template**: Use task-linked-document-template.md
2. **Validate task exists**: Ensure task ID is real before creating document
3. **Update task files**: Add document reference to related task
4. **Strategic alignment**: Ensure document serves task strategic purpose

### **When Completing Tasks**
1. **Archive task documents**: Move completed task docs to archive/
2. **Update document status**: Mark all related docs as COMPLETE
3. **Preserve links**: Maintain task references even in archive
4. **Clean references**: Remove active work references to completed tasks

## Current Document Audit (Session Implementation)

### **Documents Requiring Task Links**
- [ ] **STRATEGIC-INITIATION-SYSTEM.md** → T008-initiation-testing
- [ ] **INITIATION-COMPREHENSIVE-FIX.md** → T008-initiation-testing  
- [ ] **session/session-templates.md** → T008-initiation-testing
- [ ] **END-SESSION-SUMMARY.md** → T008-initiation-testing
- [ ] **foundation-docs/*.md** → Need task assignment or archive status

### **Documents Correctly Linked** 
- ✅ **This document** → T008-initiation-testing (properly linked)

### **Exception Documents (No Task Link Required)**
- ✅ **README.md** → Structural navigation document
- ✅ **PROJECT-OVERVIEW.md** → Structural overview document  
- ✅ **STATUS.md** → Structural status document
- ✅ **templates/*.md** → Template documents
- ✅ **COMMANDS.md** → Structural command reference

---

**Next Action**: Implement task linking for all documents requiring links during this session.
