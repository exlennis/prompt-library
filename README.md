# prompt-library

Welcome to my collection of prompts for various AI tasks!

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


## **Userful links**
- Add other prompt libaries and prompt engineering tools.


## **Contributing:**

If you have a great prompt, feel free to:
- Open an Issue to suggest a new prompt.
- Submit a Pull Request with a new prompt in the appropriate category.

Happy prompting!

---

## Library Structure (TBC)

prompt-library/
├── README.md
├── prompts/
│   ├── general/
│   │   ├── prompt_name1.md
│   │   └── ...
│   ├── coding/
│   │   ├── prompt_name2.md
│   │   └── ...
│   └── writing/
│       ├── prompt_name3.md
│       └── ...
├── templates/
│    └── prompt_template.md
├── scripts/
│    └── parse_prompts.py
└── data/
      ├── library_structure.md
      ├── prompt_categories.md
      └── metadata.json

- README.md: a clear README that explains what your prompt library is, how to use it, and how others can contribute. Include instructions on how to run any automation scripts.
- prompts/ folder: Prompts by organised by category (e.g., general, coding, writing).
- templates/ folder: Base prompt template that includes YAML front matter for metadata.
- scripts/ folder (phase-2): Add automation scripts to process or update prompts.
- data/ folder (phase-2):  Store any JSON or CSV files if you plan to aggregate metadata or stats.
- GitHub Pages (phase-2): Build a web interface for the library, can use GitHub Pages to serve the Markdown files as a website. test out Tools like Jekyll or MkDocs can turn Markdown into a static site.
