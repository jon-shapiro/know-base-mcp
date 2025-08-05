# Session File Templates

**Task ID**: T008-initiation-testing  
**Related Epic**: E001-foundation-validation  
**Related Story**: S003-unity-analysis  
**Document Type**: Implementation  
**Created**: August 04, 2025  
**Status**: ACTIVE  

## Task Context
**Purpose**: Provide templates for --end-session command to create strategic handoff files with perfect session continuity  
**Success Criteria**: Templates enable consistent strategic context preservation across sessions  
**Dependencies**: End-session command integration, strategic validation requirements  
**Strategic Value**: Ensures reliable session handoffs for systematic cannabis documentation development

---

**Purpose**: Templates for --end-session command to create strategic handoff files  
**Usage**: These templates are used by --end-session to ensure consistent strategic continuity

---

## 📋 **Session Handoff Template**

```markdown
# Session Strategic Handoff
**Date**: [DATE]
**Session Duration**: [START] - [END]  
**Phase**: [VALIDATION/DEVELOPMENT/DEPLOYMENT]

## Strategic Work Completed
### Epic Progress: [E###: Epic Name]
- **Strategic Impact**: [How this advances the project hypothesis]
- **Key Insights**: [What was learned that changes strategic understanding]
- **Strategic Value**: [What stakeholder value was created/validated]

### Story Progress: [S###: Story Name] 
- **Completion**: [X%] - [COMPLETE/IN_PROGRESS/BLOCKED]
- **Strategic Validation**: [What assumptions were validated/invalidated]
- **Next Strategic Decision**: [What decision this work enables]

### Task Progress: [T###: Task Name]
- **Status**: [COMPLETE/IN_PROGRESS/BLOCKED]
- **Strategic Learning**: [Key insights that affect larger strategy]
- **Quality**: [How work meets 8+/10 standards and strategic goals]

## Strategic Context for Next Session
### Current Strategic Position
- **Hypothesis Status**: [How current work proves/disproves core hypothesis]
- **Phase Rationale**: [Why we're in current phase vs. alternatives]
- **Key Strategic Risk**: [Biggest risk and current mitigation approach]

### Next Strategic Move
- **Primary Objective**: [Most important strategic thing to accomplish next]
- **Strategic Decision Point**: [Key decision next session should work toward]
- **Success Criteria**: [How next session success will be measured strategically]

### Stakeholder Context
- **Approval Status**: [What's approved vs. awaiting stakeholder review]
- **Communication Needed**: [Strategic updates stakeholders need]
- **Decision Points**: [Strategic decisions requiring stakeholder input]

## Next Session Initiation Command
```
INITIALIZE KNOW-BASE-MCP SESSION STRATEGIC-VALIDATION-MODE
```

**Strategic Focus**: [Brief strategic theme for next session]
**Key Validation**: [Main strategic understanding to validate during initiation]
```

---

## 📋 **Git State Template**

```markdown
# Git State for Next Session
**Created**: [DATE] by --end-session
**Repository**: /Users/jon/git/know-base-mcp

## Current Git Status
- **Branch**: [branch-name]
- **Last Commit**: [commit-hash] - "[commit-message]"
- **Remote Status**: [ahead/behind/up-to-date] 
- **Uncommitted Files**: [count] files

## Git Commands for Human Execution
**Execute these commands manually after session:**

```bash
# Navigate to repository
cd /Users/jon/git/know-base-mcp

# Add all files (cleaner approach)
git add .

# Commit with strategic context
git commit -m "[GENERATED COMMIT MESSAGE BASED ON SESSION WORK]

- [Specific accomplishments]
- [Files modified and strategic purpose]  
- [Epic/Story/Task progress]

Task: [TASK_ID] - [STATUS]
Epic: [EPIC_ID] - [PROGRESS]"

# Push to remote repository
git push origin main

# Check final status
git status
```

## Commit Message Context
**Strategic Work**: [Summary of strategic work completed]
**Files Modified**: [Key files changed and their strategic purpose]  
**Epic/Story/Task**: [Work items advanced and their strategic impact]

## Git State Validation
After executing commands, git status should show:
- **Working directory**: Clean (no uncommitted changes)
- **Branch status**: Up to date with origin/main
- **Repository state**: Ready for new work

**If git state doesn't match expected**: Report discrepancy immediately for investigation
```

---

## 📋 **Strategic Context Template**

```markdown
# Strategic Context - Updated
**Last Updated**: [DATE]
**Phase**: [VALIDATION/DEVELOPMENT/DEPLOYMENT]

## Project Strategic Identity
### Core Mission
Transform Unity Landing's 18+ cannabis retail guides via MCP + conversational AI
- **Code Reduction Target**: 89% (from 18,940 lines to ~2,041 lines)
- **Quality Standard**: 8+/10 automatically enforced
- **Speed Improvement**: 10x faster content creation
- **Industry Focus**: Cannabis retail with compliance integration

### Strategic Hypothesis
**Primary**: Component architecture + conversational AI = 10x faster content creation
**Current Test**: [What we're currently testing about this hypothesis]
**Evidence**: [What evidence supports/challenges the hypothesis]

## Current Phase Strategic Rationale
### Why Validation Phase
- **Assumption Risk**: [Key assumptions that could be wrong]
- **Stakeholder Value**: [What stakeholders need to see to approve]
- **Evidence Needed**: [What evidence will prove hypothesis]
- **Decision Point**: [What decision validation phase works toward]

### Success Criteria for Phase
- **Strategic Success**: [What strategic success looks like]
- **Evidence Collection**: [What evidence we're gathering]
- **Stakeholder Approval**: [What stakeholders need to approve next phase]
- **Risk Mitigation**: [How we're reducing strategic risk]

## Strategic Decision Framework
### Current Decision Point
**Decision**: [Key strategic decision pending]
**Options**: [Strategic alternatives being considered]
**Evidence Needed**: [What evidence will inform decision]
**Timeline**: [When decision must be made]

### Strategic Risks & Mitigation
**High Risk**: [Biggest strategic risk]
**Mitigation**: [How we're addressing it]
**Early Warning**: [What would signal this risk is materializing]

## Stakeholder Value Proposition
### Value Created
**For Jon**: [Strategic value for primary stakeholder]
**For Cannabis Industry**: [Value for target market]
**For Documentation**: [Value for documentation field]

### Approval Strategy
**Evidence Needed**: [What evidence stakeholders need]
**Communication Strategy**: [How to present strategic progress]
**Decision Timeline**: [When strategic approval needed]
```

---

## 📋 **Active Work Context Template**

```markdown
# Active Work Context
**Last Updated**: [DATE]
**Current Epic**: [E###: Epic Name]
**Current Story**: [S###: Story Name]  
**Current Task**: [T###: Task Name]

## Epic Strategic Context
### Epic Purpose: [E###: Epic Name]
**Strategic Value**: [How this Epic advances core project hypothesis]
**Success Criteria**: [What Epic success looks like strategically]
**Strategic Risk**: [What could go wrong and impact strategy]
**Timeline**: [Strategic timeline and milestone dependencies]

### Epic Progress
- **Completion**: [X%]
- **Stories Complete**: [X of Y]
- **Strategic Insights**: [Key learnings affecting strategy]
- **Next Strategic Milestone**: [Next major strategic milestone]

## Story Strategic Context  
### Story Purpose: [S###: Story Name]
**Strategic Value**: [How this Story validates/advances Epic goals]
**Hypothesis Test**: [What assumption this Story tests]
**Evidence Goal**: [What evidence this Story should produce]
**Strategic Connection**: [How Story connects to larger project vision]

### Story Progress
- **Completion**: [X%] 
- **Tasks Complete**: [X of Y]
- **Key Insights**: [Strategic insights from Story work]
- **Next Decision**: [Strategic decision this Story works toward]

## Task Strategic Context
### Task Purpose: [T###: Task Name]  
**Strategic Value**: [How this Task advances Story goals]
**Quality Standard**: [How Task meets 8+/10 strategic quality goals]
**Evidence Generation**: [What strategic evidence Task produces]
**Decision Support**: [What strategic decision Task informs]

### Task Progress
- **Status**: [COMPLETE/IN_PROGRESS/BLOCKED]
- **Next Actions**: [Next 3 specific actions and their strategic purpose]
- **Success Criteria**: [How Task success will be measured strategically]
- **Completion Timeline**: [When Task should be strategically complete]

## Technical Context (Strategic Framework)
### Technical Approach
**Strategic Rationale**: [Why current technical approach serves strategic goals]
**Quality Alignment**: [How technical quality serves strategic quality goals]
**Decision Architecture**: [What strategic decisions depend on technical work]

### Cannabis Industry Context
**Compliance Alignment**: [How work addresses cannabis industry compliance]
**Industry Value**: [Strategic value for cannabis industry stakeholders]
**Specialization**: [How work demonstrates cannabis industry expertise]

## Next Session Strategic Focus
**Primary Objective**: [Most strategically important thing to accomplish]
**Strategic Decision**: [Key strategic decision to work toward]
**Evidence Goal**: [Strategic evidence to generate]
**Success Measure**: [How strategic success will be measured]
```

---

**Templates Status**: READY FOR --END-SESSION INTEGRATION  
**Usage**: --end-session command should populate these templates with session-specific strategic context  
**Integration**: Templates designed for seamless strategic continuity across sessions
