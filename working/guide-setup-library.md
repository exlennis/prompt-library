# Prompt Library Setup Guide

Below is a step‐by‐step guide outlining how you can build a GitHub‐hosted prompt library. This guide is designed with beginners in mind—you already know Markdown, and although you’re new to programming and GitHub, you can follow along and adapt existing ideas and even automate parts of the process with AI.

---

## Phase 1

### 1. Planning Your Prompt Library

Before you start coding, it’s useful to sketch out what you want:
	•	Core Goal: Create a repository that stores reusable prompt templates.
	•	Content: Each prompt should include a title, category, detailed instructions, roles (e.g., system, user), tone/style guidelines, example usage, and any metadata (such as creation date or tags).
	•	Linking: Some prompts might reference or build on others. You might want to include links (or “see also” sections) so users can navigate between related templates.
	•	Automation: Later you can add simple scripts (e.g., Python with the OpenAI API) to help parse or update metadata automatically.

### 2. Creating Your GitHub Repository

1.	Sign Up / Sign In to GitHub:
  - If you haven’t already, create a GitHub account at github.com.
2.	Create a New Repository:
  - On GitHub, click “New” and give your repository a name (e.g., prompt-library).
	-	Choose to make it public (so others can reuse your templates) and add a README file.
	-	Click “Create repository.”
3.	Clone the Repository Locally (Optional):
  - Open your terminal and run:
  ```bash
  git clone https://github.com/your-username/prompt-library.git
  cd prompt-library
  ```

### 3. Designing the Library Structure

A clear folder structure will help keep your prompts organized. For example:

  ```markdown
  prompt-library/
  ├── README.md
  ├── prompts/
  │   ├── general/
  │   │   ├── friendly_greeting.md
  │   │   └── ...
  │   ├── coding/
  │   │   ├── generate_code.md
  │   │   └── ...
  │   └── marketing/
  │       ├── product_launch.md
  │       └── ...
  ├── templates/
  │   └── prompt_template.md
  ├── scripts/
  │   └── parse_prompts.py
  └── data/
      └── metadata.json
  ```

- prompts/ folder: Organize prompts by category (e.g., general, coding, marketing).
- templates/ folder: Create a base prompt template that includes YAML front matter for metadata.
- scripts/ folder: (Optional) Add automation scripts to process or update prompts.
- data/ folder: (Optional) Store any JSON or CSV files if you plan to aggregate metadata or stats.

### 4. Creating a Prompt Template

Using Markdown with YAML front matter is a great way to both document and programmatically parse each prompt. Create a file (e.g., templates/prompt_template.md) with contents like:

```markdown
  ---
    title: "Example Prompt Title"
    category: "General"            # e.g., General, Coding, Marketing
    role: "system"                 # The intended role (system, user, assistant)
    tone: "friendly"               # Tone (friendly, formal, casual, etc.)
    instructions: |
      Detailed instructions on what the prompt should do.
    examples: |
      Example usage or sample input/output.
    created: 2025-02-13            # Date (ISO format)
    tags: [example, quick-start]   # Optional tags for filtering
    ---

    # Example Prompt Title

    **Description:**
    This prompt is designed to generate a friendly greeting.

    **Usage Instructions:**
    - Use this prompt when you need a friendly system message.
    - It instructs the AI to output a warm welcome message.

    **Example:**

    Hello there! How can I help you today?
```

This template lets you reuse the same structure for all prompts. As you create individual prompt files in the prompts/ subdirectories, simply copy and modify this template.

### 5. Linking and Relationships Between Prompts

For prompts that are related (for example, one that builds on another), include a “Related Prompts” section with Markdown links:

  **Related Prompts:**
  - [Advanced Greeting](../general/advanced_greeting.md)
  - [Welcome Message Variations](../general/welcome_variations.md)

This way, users can easily navigate between related templates.

### 6. Utilizing AI/Automation

Since you’re interested in using AI to automate parts of the process, consider the following ideas:
	•	Parsing and Validating Prompts:
	  Create a Python script (e.g., scripts/parse_prompts.py) that reads all Markdown files in the prompts/ directory, extracts the YAML front matter, and generates a summary JSON file in the data/ folder. Libraries such as PyYAML make this straightforward.
	•	Automatic Template Generation:
	  Use the OpenAI API (or ChatGPT) to suggest improvements or generate prompt metadata based on a simple text input. For example, you can write a script that sends a prompt description and receives back a filled-out YAML section.
	•	Example (Python snippet):

  ```python
    import os, yaml, json

    prompts_data = []
    for root, _, files in os.walk('prompts'):
        for file in files:
            if file.endswith('.md'):
                with open(os.path.join(root, file), 'r', encoding='utf-8') as f:
                    content = f.read()
                    if content.startswith('---'):
                        front_matter, _ = content.split('---', 2)[1:3]
                        data = yaml.safe_load(front_matter)
                        data['path'] = os.path.join(root, file)
                        prompts_data.append(data)

    with open('data/metadata.json', 'w', encoding='utf-8') as f:
        json.dump(prompts_data, f, indent=2)
  ```

  This script gathers metadata from each prompt, making it easier to search or index them later.

### 7. Documenting and Publishing Your Library
-	README.md:
	Write a clear README that explains what your prompt library is, how to use it, and how others can contribute. Include instructions on how to run any automation scripts.
-	GitHub Pages (Optional):
	If you’d like a web interface for your library, you can use GitHub Pages to serve the Markdown files as a website. Tools like Jekyll or MkDocs can turn your Markdown into a static site.
-	Commit Often and Use Pull Requests:
	Even if you’re new to GitHub, practice by committing your changes and using pull requests (even if it’s just you) to track improvements.

### 8. Learning and Reusing Existing Projects
- Reference Ray.so Prompts: Visit ray.so/prompts to see how their prompts are displayed, and browse their GitHub repository (raycast/ray-so for code structure). Notice how they separate content from presentation and use consistent formatting for prompt details.
- Explore Other Prompt Libraries: Look into projects like disler/marimo-prompt-library for ideas on modularizing prompts and incorporating automation.

### 9. Next Steps
1. Set Up Your Repository:
Follow the steps above to create your repository and folder structure.
2. Create Several Prompt Files:
Start by adding a few prompts using your template. Experiment with different categories and note how you might link them.
3. Develop Automation Scripts:
Write a basic parser as shown above. Experiment with simple AI automation if you’re comfortable with Python.
4. Iterate and Learn:
As you become more familiar with GitHub and programming basics, continue refining your folder structure, add more metadata fields, or even integrate continuous deployment (e.g., via GitHub Actions) to update a static website.
5. Engage with the Community:
Look for feedback by sharing your project on GitHub or forums (like GitHub Discussions or Stack Overflow).

By following this guide, you’ll have a solid foundation for a GitHub-hosted prompt library that is well organized, easy to update, and even capable of automated parsing and enhancement. Enjoy the process and feel free to adapt and expand on these ideas as you learn!


---


## Phase 2 Autoudpate structure

### Best Languages to Generate a Tree Structure Dynamically

#### 1. Shell (`tree` Command) – Simple & Quick

**Best for:** Quick tree generation on macOS/Linux/WSL

**Command:**
  ```sh
  tree -I "node_modules|.git|venv"
  ```

**Pros:**
- Native command, no coding needed.
- Supports exclusions with `-I "pattern"`.
- Easily exportable (`tree > structure.md`).

**Cons:**
- Not built-in on macOS (install via `brew install tree`).
- No deep customisation (limited formatting options).

---

#### 2. Python – Customisable & Cross-Platform

**Best for:** Automating updates to `structure.md`

**Simple script to generate a tree:**
  ```python
      import os

      def generate_tree(directory, ignore=None, indent=""):
          if ignore is None:
              ignore = []
          entries = sorted([e for e in os.listdir(directory) if e not in ignore])

          for index, entry in enumerate(entries):
              path = os.path.join(directory, entry)
              is_last = (index == len(entries) - 1)
              prefix = "└── " if is_last else "├── "
              print(f"{indent}{prefix}{entry}")

              if os.path.isdir(path):
                  new_indent = indent + ("    " if is_last else "│   ")
                  generate_tree(path, ignore, new_indent)

      # Example usage
      generate_tree(".", ignore=[".git", "node_modules", "__pycache__"])
  ```

**Pros:**
- Cross-platform (works on macOS, Windows, Linux).
- Highly customisable (e.g., can save to `structure.md`).
- Can ignore specific directories.

**Cons:**
- Requires Python to run.

---

#### 3. JavaScript (Node.js) – If You’re Using a JS-Based Stack

**Best for:** GitHub Actions or web-based automation

**Install & Use:**
  ```sh
  npm install -g tree-cli
  tree -I "node_modules|.git"
  ```

**Pros:**
- Works well with GitHub Actions for CI/CD.
- Can generate JSON output (`tree -J`).

**Cons:**
- Requires Node.js installed.

---

### Best Format to Represent a Tree Diagram

#### 1. Markdown (Plain Text) – Readable & Simple

**Best for:** Documentation, GitHub, Notion, and `README.md`

**Example:**
  ```plaintext
    /prompt-library
    │── /templates
    │   ├── AI_Art/
    │   ├── Coding/
    │   ├── Productivity/
    │   ├── Writing/
    │   ├── Miscellaneous/
    │
    │── /working
    │   ├── step-by-step/
    │   ├── experiments/
    │   ├── notes/
    │
    │── /docs
    │   ├── structure.md
    │   ├── CONTRIBUTING.md
    │   ├── LICENSE
    │
    │── .gitignore
    │── README.md
  ```

**Pros:**
- Easy to type and edit.
- Works well in GitHub, Notion, Markdown files.
- Readable without extra software.

**Cons:**
- Not interactive.
- No automatic formatting.

---

#### 2. Mermaid.js (For Diagrams in Markdown/GitHub)

**Best for:** Dynamic tree diagrams in GitHub, Notion, MkDocs

**Example (`.md` file with Mermaid):**
  ```mermaid
  graph TD;
      A[prompt-library] --> B[templates]
      B --> C[AI_Art]
      B --> D[Coding]
      B --> E[Productivity]
      B --> F[Writing]
      B --> G[Miscellaneous]
      A --> H[working]
      H --> I[step-by-step]
      H --> J[experiments]
      H --> K[notes]
      A --> L[docs]
      L --> M[structure.md]
      L --> N[CONTRIBUTING.md]
      L --> O[LICENSE]
      A --> P[.gitignore]
      A --> Q[README.md]
  ```

**Pros:**
- GitHub renders Mermaid.js natively.
- Interactive – collapsible, zoomable (when embedded).
- Can be used in Notion, MkDocs, or Obsidian.

**Cons:**
- Not fully supported in all Markdown viewers.
- Needs extra setup for local rendering.

---

#### 3. Graphviz (DOT Language) – Professional Use

**Best for:** Complex trees, programmatic diagrams

**Example (`.dot` file):**
  ```dot
  digraph G {
      "prompt-library" -> "templates";
      "templates" -> "AI_Art";
      "templates" -> "Coding";
      "templates" -> "Productivity";
      "templates" -> "Writing";
      "templates" -> "Miscellaneous";

      "prompt-library" -> "working";
      "working" -> "step-by-step";
      "working" -> "experiments";
      "working" -> "notes";

      "prompt-library" -> "docs";
      "docs" -> "structure.md";
      "docs" -> "CONTRIBUTING.md";
      "docs" -> "LICENSE";

      "prompt-library" -> ".gitignore";
      "prompt-library" -> "README.md";
  }
  ```

**Pros:**
- Graphical output (PNG, SVG, etc.).
- Automated layouting – cleaner than ASCII.
- Works in LaTeX, Markdown, or standalone tools.

**Cons:**
- Requires Graphviz installed (`brew install graphviz`).
- Not as readable as Markdown.

---

#### 4. JSON/YAML (For Programmatic Use)

**Best for:** Automation, structured data

**Example (`tree.json`):**
    ```json
        {
          "prompt-library": {
            "templates": {
              "AI_Art": {},
              "Coding": {},
              "Productivity": {},
              "Writing": {},
              "Miscellaneous": {}
            },
            "working": {
              "step-by-step": {},
              "experiments": {},
              "notes": {}
            },
            "docs": {
              "structure.md": {},
              "CONTRIBUTING.md": {},
              "LICENSE": {}
            },
            ".gitignore": {},
            "README.md": {}
          }
        }
    ```

**Pros:**
- Machine-readable for automation.
- Works with APIs, scripts, JSON-to-visual conversion tools.

**Cons:**
- Not human-readable as Markdown.
- Needs extra software to visualize.
