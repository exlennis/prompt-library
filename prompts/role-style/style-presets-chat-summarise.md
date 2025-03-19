SUMMARISE-CHAT

```
MODE:
Collaborative Professional Curiosity
Technical Insight Exploration
Peer-Level Dialogue

STYLE:
Inquisitive yet Informed
Respectfully Curious
Technical Peer Engagement

OUTPUT:
When addressing technical or complex topics:
- Ask open-ended questions that invite comprehensive explanations
- Use language that demonstrates genuine curiosity
- Frame inquiries to reveal underlying reasoning
- Maintain a balanced, non-hierarchical communication tone
- Seek to understand rather than prescribe solutions
- Use phrases that signal collaborative exploration: 
  - "Could you help me understand..."
  - "What's the reasoning behind..."
  - "I'm curious about how..."
- Provide context for questions to show thoughtful engagement
- Demonstrate technical awareness while seeking deeper insights
- Avoid overly deferential or directive language
- Focus on mutual understanding and knowledge sharing
```

Description: This template provides a generic, flexible approach for requesting a summary from Claude across various types of conversations. It ensures a structured, objective recap while allowing flexibility for different conversation types.

How to use: Here are some snappy `prompt` options when asking for a chat summary. Each provides a different tone while maintaining the core request. Try the `professional` option for clarity while still being conversational. 
- Professional Version:

```
Can you synthesise the key insights from our conversation?
```

- Succinct Technical Version:

```
Conversation summary. Go.
```

- No-Nonsense Version:

```
Break down our chat. What really happened here?
```

- Slightly Cheeky Version:

```
TL;DR: What did we just talk about?
```

---

*Options*: 
/summary-short (3 sentences) 
/summary-table/
/summary-bullets.



```
MODE: 
Comprehensive Chat Synthesis
Objective Information Extraction
Key Insight Identification

STYLE:
Neutral
Analytical
Concise

OUTPUT FORMAT OPTIONS:
- summary-short: Provide a 3-sentence overview capturing the essence of the conversation
- summary-table: Present key points in a structured markdown table format
- summary-bullets: Organise main points in a concise bullet-point list
- [default]: Provide a comprehensive structured summary

OUTPUT:
Provide a structured summary of our entire conversation, following these guidelines:
## Chat Summary [yyyyMMdd]

Query: [first message]
Topic: [topic]

### Key Points
1. [main point 1]
2. [main point 2]
3. [main point 3]

### Conclusions & Questions
- Resolved: [key conclusion]
- Open: [unresolved question]

### Next Steps
- [action item 1]
- [action item 2]

### References
- [optional: key links or documents]

```


```
## Chat Summary [timestamp]
### Context
- Initial query: [first message]
- Main topic: [topic]

### Key Discussion Points
1. [point 1]
2. [point 2]
3. [point 3]

### Action Items
- [action 1]
- [action 2]

### Next Steps
> Suggested next actions or areas to explore
```
