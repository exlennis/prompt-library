# Preset/Style: Summarise Chat 

NAME: Summarise
MODEL: Claude

### Description

A generic and flexible approach for requesting a summary of various conversations. This style ensures a structured, objective summary while providing flexibility for different conversation types.

### Prompt

The prompt below provides different tones while maintaining the core request—ensuring clarity while still being conversational. Try these options when asking for a chat summary:

- Default: `You are tasked with analysing the entire conversation and providing a structured summary. Please follow the <instructions> below; use Australian English spelling throughout.`
- Professional: `Please synthesise key insights from the session.`
- Succinct: `Conversation summary. Go.`
- Technical: `Analyse our chat. What did we discuss?`
- Concise: `TL;DR: What did we talk about?`

### Commands

The summary format can be customised using the slash commands below. If not specified, the default format will provide a comprehensive structured summary using the following template.

- /summary
- /summary-concise, -short
- /summary-list, -bullet
- /summary-table

---

### Instructions

<instructions>
MODE: SUMMARISE
Comprehensive Chat Synthesis
Objective Information Extraction
Key Insight Identification

STYLE:
Neutral and Objective
Analytical and Structured
Concise and Succinct

FORMATS:
- summary-short: Provide a 3-sentence overview capturing the essence of the conversation
- summary-table: Present key points in a structured markdown table format
- summary-bullets: Organise main points in a concise bullet-point list
- [default]: Provide a comprehensive structured summary

OUTPUT:
- Start by capturing the key aspects of the discussion using the <template> below.
- In the "Context" section, record the initial query and all main topics discussed throughout the conversation.
- Include crucial discussion points from the chat in "Key Points"; summarise resolved issues and list pending queries in "Conclusions & Questions".
- Optionally, add a "Next Steps" and "References" section if needed.
- Ensure the summary is objective, insightful, and covers the evolution of the conversation.

    <template>
    ## Chat Summary [yyyyMMdd]
    
    ### Context
    
    -  Query: [first message of the conversation]
    -  Topic: [main topic(s) discussed, ensuring all significant shifts in focus are captured]
    
    ### Key Points
    
    1. [main point 1]
    2. [main point 2]
    3. [main point 3]
    
    ### Conclusions & Questions
    
    -  Resolved: [key conclusions reached]
    -  Open: [unresolved questions]
    
    ### Next Steps (Optional)
    
    -  [action item 1]
    -  [action item 2]
    
    ### References (Optional)
    
    -  [include links or documents if necessary]
    </template>

</instructions>
