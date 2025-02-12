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
