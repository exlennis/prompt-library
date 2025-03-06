# Prompt Library

Welcome to my collection of prompts for various tasks!

- Goal: Create a repository that stores reusable prompt templates.
- Content: Each prompt should include a title, category, detailed instructions, roles (e.g., system, user), tone/style guidelines, example usage, and any metadata (such as creation date or tags).
- Linking: Some prompts might reference or build on others. You might want to include links (or “see also” sections) so users can navigate between related templates.
- Automation: Later you can add simple scripts (e.g., Python with the OpenAI API) to help parse or update metadata automatically.

## **Categories:**

- [Writing](/categories/ai-writing/)
- [Coding](/categories/coding/)
- [General](/categories/general/)
- ... (list all your categories with links) to be updated

## **How to Use:**

1.  Browse the [Prompts](/prompts/) folder.
2.  Find prompts that are relevant to you.
3.  Copy the "Prompt" section and paste it into your AI tool of choice.
4.  Customise the placeholders (like `[Topic]`) as needed.


---

## Project Structure

```markdown
/prompt-library
│── README.md                 # Main repository overview, explains how to use the prompt library, and how others can contribute. Include instructions on how to run any automation scripts.
│── prompts/                   # Collection of curated prompt organised by category
│   ├── Writing/              # Creative & technical writing prompts
│   ├── Coding/               # Prompts for coding assistance
│   ├── Productivity/         # Prompts for automation, task management
│   ├── General/              # Misc prompts that don’t fit other categories
│   └── ...
│
│── templates/                 # Collection of base templates
│   ├── prompt_tempalte.md    # Base prompt template that includes YAML front matter for metadata.
│   └── ...
│
│── scripts/                    # Collection of base templates
│   ├── parse_prompts.py       # automation scripts to process or update prompts.
│   └── ...
│
│── data/                      # Store any JSON or CSV files if you plan to aggregate metadata or stats.
│   ├── metadata.json
│   ├── category.csv
│   └── ...
│
│── working/             # Personal work-in-progress section (optional for Git tracking)
│   ├── guides/          # Step-by-Step, workflows, automation steps
│   ├── experiments/    # Test prompts, iterative improvements
│   ├── notes/          # Research, references, general thoughts
│
│── docs/                # Public-facing documentation
│   ├── structure.md    # Folder structure reference & future expansion notes
│   ├── CONTRIBUTING.md # Guidelines for contributing
│   ├── LICENSE         # Repository license information
│
└── .gitignore           # Specifies ignored files/directories (consider adding /working/)
```




---


## **Userful links**
- Add other prompt libaries and prompt engineering tools.


## **Contributing:**

If you have a great prompt, feel free to:
- Open an Issue to suggest a new prompt.
- Submit a Pull Request with a new prompt in the appropriate category.

Happy prompting!
