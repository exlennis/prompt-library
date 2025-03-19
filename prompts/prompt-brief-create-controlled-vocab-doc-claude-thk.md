## Brief: Create Controlled-Vocabulary-v01.md

<brief>
### Purpose

Create a comprehensive list of standardised terminology for consistent folder naming throughout the FOMO system. This controlled vocabulary will ensure uniform metadata application, improve searchability, and provide clear guidance for both manual and automated file organisation.

### Document Structure

1. **Introduction**
   - Purpose and benefits of the controlled vocabulary
   - Relationship to other FOMO documents
   - Implementation guidelines
2. **Core Terminology Categories**
   - Project-related terms
   - Resource-related terms
   - Knowledge-related terms
   - System-related terms
   - Temporal/versioning terms
   - Status/workflow terms
3. **Term Formatting Standards**
   - Level 1 (top-level) folder terminology
   - Level 2+ (nested) folder terminology
   - Special case terminology
   - Prohibited terminology
4. **Implementation Guidelines**
   - When to use controlled terms
   - How to combine terms
   - Handling special cases
   - Extending the vocabulary
5. **Term Dictionary**
   - Alphabetically ordered master list
   - Definition/purpose of each term
   - Usage examples
   - Related terms
6. **Domain-Specific Extensions**
   - Design-specific terminology
   - Development-specific terminology
   - Content-specific terminology

### Key Requirements

1. Align with established kebab-case naming convention while respecting macOS conventions for top-level folders
2. Support the defined directory structure's organisation principles
3. Balance comprehensiveness with practical usability
4. Account for domain-specific needs while maintaining system-wide consistency
5. Include common prefixes and suffixes for version control and status indication
6. Provide clear examples for each term category
7. Support the automation goals of the FOMO project

### Integration Points

- Must complement the directory structure outlined in directory-structure-GUIDELINES-v02.md
- Must support the naming standards from naming-STANDARDS-v02.md
- Should support the workflows identified in the project charter and implementation plan
- Consider the automation requirements outlined in project documents
</brief>

## Prompt: Create Controlled Vocabulary Document (Claude Thinking)

<prompt> 
```markdown
## Background
The next step for FOMO project (File Organisation, Management & Optimisation) system is to develop the "Controlled-Vocabulary-v01.md" document. This document will provide a standardised list of terms for consistent folder naming across my file system. The vocabulary needs to align with my existing FOMO documents which establish a kebab-case naming convention for files and a structured directory system.

## Task
Create a comprehensive controlled vocabulary list that standardises terminology for naming (directories, folders, files, tags etc.) within FOMO system. The document should be structured as a markdown file following the outline provided below.

## Document Requirements

1. Follow the structure outlined in the brief:
   - Introduction
   - Core Terminology Categories
   - Term Formatting Standards
   - Implementation Guidelines
   - Term Dictionary
   - Domain-Specific Extensions

2. Ensure all terminology aligns with these principles:
   - Top-level folders use one-word with capitalisation (Projects, Resources)
   - Nested folders use lowercase with hyphens when necessary (archive, dev, client-projects)
   - Terms should be concise, clear, and descriptive
   - Follow Australian English spelling conventions

3. Include terms that support these directory categories:
   - Projects (design and development work)
   - Resources (assets, templates, references)
   - Knowledge (documentation, notes, research)
   - System (configuration, automation, maintenance)
   
4. For each term in the dictionary, provide:
   - Clear definition
   - Usage context
   - Formatting example
   - Any related terms

5. Consider these special requirements:
   - Include terms for versioning and workflow states
   - Support design project terminology (briefs, mockups, assets)
   - Support development terminology (src, components, utils)
   - Include terms for temporal organisation (archive, current, upcoming)

## Key Integration Points
The controlled vocabulary must integrate seamlessly with:
- The kebab-case naming convention specified in naming-STANDARDS-v02.md
- The directory structure outlined in directory-structure-GUIDELINES-v02.md
- The principles outlined in the project-charter-v01.md
- The implementation approach in implementation-plan-v01.md

Please create a comprehensive, well-organised Controlled-Vocabulary-v01.md document that will serve as the standardised terminology reference for the entire FOMO system.
```
</propmt>
