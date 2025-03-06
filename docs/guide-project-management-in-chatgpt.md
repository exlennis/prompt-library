# ChatGPT Project Guidelines – A Framework for Streamlined Management  
*Enhancing Consistency, Collaboration, and Results*  

This guidelines ensures chatGPT's projects are setup properly, stay organised, collaborative, and goal-oriented. 


---

## **1. Purpose of the Guidelines**  
These guidelines:  
- **Standardise Processes**: Define scope, organise resources, and align stakeholders.  
- **Optimise Outputs**: Generate responses using tailored tone, formatting, and examples.  
- **Ensure Relevance**: Maintain consistency through updates and reviews.  

---

## **2. Project Components**  

### **2.1 Project Files**  
Centralise documents, code, or data to provide ChatGPT with contextual awareness. Prioritise **critical files** within the 20-file limit.  

#### **Essential Files by Category**  
| **Category**             | **File Examples**                                                                 | **Purpose**                                                                 |
|--------------------------|-----------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| **Project Overview**     | `Project_Brief.md`, `Style_Guide.pdf`                                             | Define goals, scope, branding, and audience.                               |
| **Reference Materials**  | `Competitor_Analysis.xlsx`, `User_Personas.pdf`, `Meeting_Notes.docx`             | Provide market insights, user demographics, and decision summaries.        |
| **Tasks & Resources**    | `Task_Breakdown.xlsx`, `Resource_Links.md`                                        | Track deadlines, responsibilities, and key links/APIs.                     |
| **Deliverables**         | `Final_Designs.zip`, `Codebase_Snapshot.zip`                                      | Store approved outputs (designs, code, reports).                           |
| **Feedback & Revisions** | `User_Feedback.xlsx`, `Change_Log.md`                                             | Capture feedback and track version history.                                |
| **Compliance**           | `Terms_of_Service.pdf`, `Privacy_Policy.pdf`                                     | Ensure legal/regulatory alignment.                                         |

#### **File Management Best Practices**  
- **Prioritise Active Files**: Upload only files ChatGPT *actively* needs for analysis (e.g., briefs, feedback, code).  
- **Compress Large Assets**: Use `.zip` or `.rar` for bulk files (e.g., `Final_Designs.zip`).  
- **Archive Completed Work**: Move outdated files to external storage to free up the 20-file limit.  

---

### **2.2 Project Instructions**  
Tailor ChatGPT’s behaviour to align with your project’s goals, tone, and processes.  

#### **Core Elements of Instructions**  
1. **Purpose & Scope**  
   - **Project Name**: `[Project Name]`  
   - **Objective**: `[Goal]` (e.g., "Create a HomeKit automation guide").  
   - **In-Scope**: `[Focus areas]` (e.g., "HomeKit-compatible devices").  
   - **Out-of-Scope**: `[Exclusions]` (e.g., "No non-HomeKit products").  

2. **Referenced Files**  
   Direct ChatGPT to critical files:  
   ```markdown
   - Use `Project_Brief.md` for scope and objectives.  
   - Follow `Style_Guide.pdf` for tone and formatting.  
   - Review `Competitor_Analysis.xlsx` for market insights.  
   ```
   
3. Tone & Style Guidelines
    - Tone: Professional, casual, or technical.
    - Audience: Developers, clients, or general users.
    - Voice: Authoritative, approachable, or neutral.
    - Avoid: Jargon, passive voice, or unsupported claims.

4. Formatting Requirements    
    - Use Markdown for structure (tables, bullet points, headings).
    - AU English spelling only

5. **Workflow & Iteration**
    - **Feedback**: Reference User_Feedback.xlsx for improvements.
	- **Revisions**: Document changes in Change_Log.md.
	- **Clarification**: Ask questions if requirements are unclear.   
   
### **2.3 File Organisation**

Use this folder structure to maintain order:

```markdown
├── 01_Project_Overview/    # Briefs, style guides
├── 02_Tasks_Resources/     # Task lists, research links
├── 03_Deliverables/        # Final outputs (designs, code)
├── 04_Feedback/            # User feedback, change logs
└── Archive/                # Completed/outdated files
```

### **2.4 Referencing System**

- **Tag Files**: Use `#ProjectBrief` or `#StyleGuide` for quick linking.
- **Central Index**: Update `README.md` with: 
  - Key milestones and deliverables.
  - Links to critical files (e.g., `[Task Breakdown](02_Tasks_Resources/Task_Breakdown.xlsx)`).
---

## **3. Project Setup Checklist**  
1. **Define Overview**: Clarify purpose, scope, and stakeholders.  
2. **Set Objectives**: Split into primary/secondary goals.  
3. **Break Down Tasks**: Assign deadlines and priorities.  
4. **Gather Resources**: Curate reference links, guides, and templates.  
5. **Write Instructions**: Specify tone, formatting, and examples.  
6. **Organise Files**: Follow the standardised folder structure.  

---

## **4. Ongoing Maintenance**  

### **4.1 Regular Reviews**  
- Conduct weekly/monthly check-ins to assess progress.  
- Example: *“Review camera comparison drafts by 10 February.”*  

### **4.2 File Updates**  
- Reflect changes in tasks/resources promptly.  
- Update the `README.md` index to maintain clarity.  

### **4.3 Archiving**  
- Move completed tasks to `Archive` with descriptive names (e.g., `2025-02-01_HomeKit_Cameras_Report`).  
- Purge outdated files quarterly.  

