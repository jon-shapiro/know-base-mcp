# Unity Landing Component & Use Case Index

**Purpose**: Map actual Unity Landing components to their guides and extract use cases for review  
**Source**: Direct examination of Unity Landing `/docs-copy/src/` files  
**Status**: FOR REVIEW - Components validated, use cases need approval

## 🔍 **ACTUAL UNITY LANDING COMPONENTS**

### **Components Found in `_includes/components/`**
| Component | Guide Usage | File Path | Purpose |
|-----------|-------------|-----------|---------|
| **hero-section.liquid** | All guides (18) | `components/core/hero-section.liquid` | Page headers with back navigation |
| **message-box.liquid** | All guides (18) | `components/core/message-box.liquid` | Tips, warnings, info, notes (6 types) |
| **section-wrapper.liquid** | All guides (18) | `components/layout/section-wrapper.liquid` | Layout containers with gradients |
| **grid-layout.liquid** | Multiple guides | `components/layout/grid-layout.liquid` | Multi-column content |
| **feature-card.liquid** | getting-started, site-template | `components/content/feature-card.liquid` | Feature/benefit displays |
| **section-header.liquid** | Multiple guides | `components/content/section-header.liquid` | Section titles |
| **three-columns.liquid** | getting-started, site-template | `components/admin/three-columns.liquid` | Admin interface layouts |
| **back-to-top.liquid** | Multiple guides | `components/core/back-to-top.liquid` | Page navigation |
| **quick-start-wrapper.liquid** | getting-started | `components/layout/quick-start-wrapper.liquid` | Tutorial containers |
| **benefits-section.liquid** | getting-started | `components/sections/benefits-section.liquid` | Value propositions |

### **Top-Level Components in `_includes/`**
| Component | Guide Usage | File Path | Purpose |
|-----------|-------------|-----------|---------|
| **help-section-footer.liquid** | All guides (18) | `help-section-footer.liquid` | Guide page footers |
| **animated-link.liquid** | Multiple guides | `animated-link.liquid` | Enhanced navigation |
| **admin-interface.liquid** | site-template | `admin-interface.liquid` | Admin layouts |
| **quick-start.liquid** | getting-started | `quick-start.liquid` | Quick start sections |

### **Specialized Sections in `_includes/sections/`**
| Section Group | Components | Guide Usage | Purpose |
|---------------|------------|-------------|---------|
| **site-template/** | 13 components | site-template guide only | Site setup workflow |
| **tv-location/** | 2 components | tv-location guide only | TV display setup |
| **value-sections/** | 1 component | Multiple guides | Value propositions |

## 📋 **USE CASES EXTRACTED FROM ACTUAL GUIDES**

### **Basic Guide Creation (Confirmed in All 18 Guides)**
1. **Hero + Content + Footer Pattern** - Every guide uses this structure
2. **Multi-section Layout** - Section wrappers with gradient backgrounds
3. **User Guidance Messages** - Message boxes for tips/warnings/info
4. **Responsive Content** - Grid layouts for multi-column content

### **Cannabis Industry Patterns (Found in Guides)**
1. **Compliance Warnings** - Message boxes with "warning" type for regulations
2. **Multi-device Content** - Web, kiosk, TV display optimization mentioned
3. **POS Integration** - Treez integration referenced throughout guides
4. **Cannabis Product Categories** - Flower, edibles, concentrates organization
5. **Dispensary Hours** - Store hours configuration in multiple guides
6. **License Information** - Business license references in site-template
7. **Age Verification** - 21+ verification mentioned in compliance contexts

### **Admin Interface Documentation (Site-Template Guide)**
1. **Three-column Admin Layout** - Content > Selection > Configure pattern  
2. **Step-by-step Configuration** - Header, General, SEO, Footer, Buttons, Ads
3. **Environment Management** - Test vs Production workflow documentation
4. **Save/Publish Process** - Draft, publish, maintenance mode workflow

### **Tutorial Workflows (Getting-Started Guide)**
1. **Progressive Setup** - Quick start with 3-step process
2. **Benefits Communication** - Feature cards with value propositions
3. **Multi-step Tutorials** - Quick start wrappers with progression
4. **Help Integration** - Help footer on every tutorial page

## 📊 **COMPONENT USAGE FREQUENCY**

### **Universal Components (18/18 guides)**
- **hero-section.liquid** - Page headers
- **message-box.liquid** - User guidance  
- **section-wrapper.liquid** - Layout containers
- **help-section-footer.liquid** - Page footers

### **High Usage (10+ guides)**
- **grid-layout.liquid** - Multi-column layouts
- **feature-card.liquid** - Benefits/features
- **section-header.liquid** - Section organization

### **Specialized Usage (1-3 guides)**
- **three-columns.liquid** - Admin documentation only
- **Site-template sections** - Site setup workflow only
- **TV-location sections** - TV setup workflow only

## 🎯 **PROPOSED USE CASES FOR REVIEW**

### **MVP Use Cases (Based on Universal Components)**
1. **Basic Guide Creation** - Hero + sections + footer structure
2. **User Guidance** - Tips, warnings, notes via message boxes
3. **Responsive Layout** - Multi-column content with grid layouts
4. **Cannabis Compliance** - Warning messages for regulations
5. **Multi-section Documents** - Section wrappers with styling

### **Enhanced Use Cases (Based on High Usage Components)**
6. **Feature Communication** - Benefits display with feature cards
7. **Admin Documentation** - Three-column interface layouts
8. **Tutorial Creation** - Progressive setup with quick start wrappers
9. **Value Proposition** - Benefits sections for product features

### **Advanced Use Cases (From Day-in-Life Document)**
**⚠️ THESE NEED VALIDATION - NOT CONFIRMED IN UNITY LANDING**
- Multi-guide coordination
- Dynamic component creation
- Interactive mockup testing
- Content impact analysis
- Cross-guide reference tracking
- Terminology consistency checking
- Multi-guide deployment
- Content performance analytics
- Pattern learning
- Visual design iteration
- [... 14 more advanced capabilities from day-in-life document]

## ❓ **QUESTIONS FOR REVIEW**

### **Component Validation**
1. Are the 14 universal/high-usage components sufficient for MVP?
2. Should we include the 15 specialized sections for site-template/tv-location guides?
3. Which components from the original 30-component list should we eliminate?

### **Use Case Validation**  
1. Which of the 9 confirmed use cases are priority for MVP?
2. Are any of the 24 advanced use cases from day-in-life document actually needed?
3. Should we focus only on single-guide creation initially?
4. What cannabis industry features are actually required vs. nice-to-have?

### **Scope Definition**
1. MVP = 14 components + 9 basic use cases?
2. Enhanced = Add specialized sections for complex workflows?
3. Advanced = Multi-guide features from day-in-life scenarios?

---

**Next Step**: Review this index and approve which components and use cases to include in the actual MCP implementation.
