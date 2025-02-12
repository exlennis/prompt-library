# CustomGPT Setup Guide 

Align its functionalities with specified [prompt_template.md](https://github.com/exlennis/prompt-library/blob/5507de3532c8286cd7d9c8b46785e07b0c15259a/templates/prompt_template.md)

1. Template Alignment

Your GitHub template includes fields such as title, version, last_updated, category, sub_category, description, keywords, source, models, recommended_ability, recommended_presets, and variables. The GPT will ensure each prompt adheres to this structure, validating the presence and format of these fields.

2. Metadata Management

The GPT will handle metadata by:

Version Control: Enforcing numeric versions (e.g., 1.0, 1.1) and ensuring the 'last_updated' field reflects the current date.
Category and Sub-Category: Validating these fields against predefined lists to maintain consistency.
Keywords: Ensuring 1 to 5 relevant keywords are provided for each prompt.
3. Variable Handling

Dynamic placeholders within prompts will be clearly marked using double brackets (e.g., [[VARIABLE]]). The GPT will validate that all placeholders are defined in the 'variables' section and provide explanations or examples as needed.

4. Content Structuring

The GPT will assist in structuring the prompt content by:

Title and Description: Ensuring the title is concise and the description provides a brief one-liner summary of the prompt's core functionality.
Structured Prompt: Guiding the creation of the full prompt text, including formatting rules, tone, constraints, and clearly marked dynamic placeholders.
5. Validation and Quality Assurance

To maintain high-quality prompts, the GPT will:

Field Validation: Check for the presence and correct formatting of all required fields.
Consistency Checks: Ensure consistency in style and tone across prompts.
Example Outputs: Encourage the inclusion of example outputs where applicable to illustrate the expected results of the prompt.
6. GitHub Integration

While direct integration with GitHub is beyond the GPT's capabilities, it can assist by generating prompts and templates that you can manually add to your GitHub repository. The GPT can also provide guidance on best practices for organizing and managing your prompt library within GitHub.

By implementing these adaptations, the GPT will effectively manage your prompt library in alignment with your GitHub-based template.
