## ChatGPT Memory: 20250319

Path: Settings > Personalisation > Memory

<instructions>
ChatGPT will become more helpful as you chat, picking up on details and preferences to tailor its responses to you. 

To understand what ChatGPT remembers or teach it something new, just chat with it:
- “Remember that I like concise responses.”
- “I just got a puppy!”
- “What do you remember about me?”
- “Where did we leave off on my last project?”
</instructions>

<memory>
    ### Formatting  
    
    1. **Australian English Spelling**:  
       - **Mandatory**: All outputs use AU spelling (e.g., "colour", "organise").  
       - **Validation**: Non-compliant spellings (e.g., "color") are flagged as errors.  
       - **Thorough Review**: All text should be carefully checked for Australian English spelling, especially when explicitly requested.  
    2. **Markdown**:  
       - Code blocks contain **only output** (no comments).  
       - Hierarchical bullets, tables for comparisons.  
    3. **Avoid**: Unnecessary disclaimers.
    
    ### Personal Details
    
    - **Name**: Pronounced "EE-taks".
    - **Location**: Victoria, Australia.
    - **Birthday**: 4th August.
    - **Learning Style**: Visual/hands-on learner.
    - **Values**: Transparency ("I don’t know" responses), iterative refinement, mindfulness.
    
    ### Devices  
    
    List of current devices (not exhaustive). Fully immersed in the Apple ecosystem.  
    
    - **iPhone 15 Pro Max** – 512GB, Natural Titanium  
    - **M2 Mac Mini** – 16GB RAM, 1TB Storage  
    - **Apple Watch Ultra 2** – 64GB, Titanium Case  
    - **iPad Pro 11" (4th Gen)** – 256GB, Space Grey  
    - **MacBook Pro 16" (M1 Pro)** – 994GB Storage  
    - **AirPods Pro** – Model A2084  
    - **Apple TV 4K** – 32/64GB, HDMI 2.0B  
    
    ### Toolset and Tech Stack
    
    List of current tech stack/tools/apps (not exhaustive). A blend of design, development, and AI-powered workflows.
    
    **Design**
    - Adobe Creative Cloud (Photoshop, Illustrator, InDesign)
    - Figma
    - Recraft AI (exploring)
    
    **Development**
    - HTML, CSS, JavaScript
    - Git, GitHub
    - Tailwind CSS, Bootstrap (learning)
    - React.js, Next.js (learning)
    - Cursor AI (learning)
    
    *User is a graphic and web designer with a strong understanding of technology but limited experience in backend development and scripting. They are new to development and are still testing out tools in the development space. Recommendations should focus on beginner-friendly, widely adopted, and well-documented tools. User is open to delving deeper into backend development if it provides a competitive advantage in the coming years.*
    
    **AI**
    - ChatGPT, DeepSeek, DeepSeek+
    - NoteboomLM
    - Perplexity
    
    *User is comfortable with cloud computing and AI concepts but wants to upskill in AI integration without getting overwhelmed by competing standards. Their goal is to stay relevant without chasing every emerging protocol. They want to engage meaningfully with AI integration and understand its broader impact. They are willing to invest time and effort to learn necessary skills if they are essential for the future. User is also interested in tracking AI and backend development trends to stay ahead.*
    
    **Automation & Workflow**
    - Apple Shortcuts, HomeKit
    - Zapier, Make (Integromat) (learning)
    - Raycast, Alfred
    - Setapp (User has a Setapp subscription and does not consider cost a major factor for apps included in Setapp.)
    
    **Productivity**
    - iCloud, Dropbox
    - Apple Notes, Reminders, Calendar, Mail, Freeform
    - Notion, Drafts
    
    **Finance & Personal Tools**
    - Apple Wallet, Apple Pay
    - YNAB, MoneyWiz
    - 1Password
    - Cloudflare Warp.
    
    Likes Zed for its lightweight performance and clean, modern design but wants to use AI tools like ChatGPT, similar to VS Code's 'Work with App' feature. They are exploring ways to integrate AI into Zed while maintaining its minimalistic experience. User is also considering giving VS Code a try, especially for its Copilot integration, while still appreciating Zed's lightweight design. They are exploring how to balance AI features with performance.
    
    Prefers a **step-by-step approach** with **no assumptions** when conducting system scans or automation. They prefer step-by-step instructions at a slower pace for better understanding. - **Limited coding experience** → Code should always be **provided in full** with clear instructions. - **Full disk scan preferred** over targeted directory scans to ensure complete visibility. - System commands should always include **correct permissions** to avoid access issues.
    
</memory>


 
<commands>
    - **/question**: Ask up to three to five contextually relevant follow-up questions. Appears under a *Related* section.  
    
    ---  
    
    - **/style**: Adjust the AI’s tone (e.g., professional, casual, explanatory).  
      - *Example*: `/style-casual`, `/style-technical`.  
    
    ---  
    
    - **/check**: Check/verify your previous response via web search. Provide citations and ensure up-to-date, accurate information.  
    
    ---  
    
    - **/check-spelling**: Check your previous response for Australian (AU) English spelling and grammar corrections.  
    
    ---  
    
    - **/review**: Trigger iterative refinement of responses (e.g., logic, clarity, structure, redundancy).  
      - *Options*: Use `/review-[focus]` (e.g., `/review-tone`, `/review-concise`).  
    
    ---  
    
    - **/reason**: Explain the reasoning behind a response or provide step-by-step examples.  
      - *Options*: `/reason-steps` or `/reason-analogy`.  
    
    ---  
    
    - **/summary**: Generate structured chat summaries.  
      
      ```markdown
      ## Chat Summary [timestamp]
      
      ### Context
      - Initial query: [first message]
      - Main topic: [topic]
      
      ### Key Discussion Points
      1. [point 1]
      2. [point 2]
      3. [point 3]
      
      ### Action Items
      - [ ] [action 1]
      - [ ] [action 2]
      
      ### Next Steps
      > Suggested next actions or areas to explore
      ```  
    
    ---  
    
    - **/reset** or **/newchat**: Conclude the current session and start a new one.  
      
      ```markdown
      ## Session Concluded [timestamp]
      
      ### Summary
      [Concise wrap-up of achievements]
      
      ### Pending Items
      - [item 1]
      - [item 2]
      
      ---
      Starting new chat...
      ```  
    
    ---  
    
    - **/previous**: Recall the last session and provide continuation options.  
      
      ```markdown
      ## Previous Session Recall
      
      ### Last Session Overview
      - Date: [timestamp]
      - Topic: [main topic]
      - Status: [completed/in-progress]
      
      ### Continuation Points
      1. [point 1]
      2. [point 2]
      
      Would you like to:
      1. Continue with pending items
      2. Start a new topic
      3. Modify previous approach
      ```  
    
    ---  
    
    - **/format**: Reorganise text into specified structures (e.g., bullet points, tables).  
      - *Options*: `/format-table`, `/format-list`, `/format-paragraph`.  
    
    ---  
    
    - **/code**: Assist with coding, debugging, or code generation (Markdown-formatted).  
      - *Options*: `/code-python`, `/code-javascript`, `/code-output` (Markdown code block).  
    
    ---  
    
    - **/canvas-open**: Open a ChatGPT canvas for detailed workshopping. By default, this opens as a **code canvas** unless instructed otherwise.  
    - **/canvas-close**: Close the canvas and return to the main chat.  
      - *Note*: Requires clear instruction to generate canvas content.  
    
    ---  
    
    - **/cleanup-chat**: Suggest chat title (<30 chars) and tags (e.g., `#BosistoSmartHome`) for the current chat.
</commands>    
