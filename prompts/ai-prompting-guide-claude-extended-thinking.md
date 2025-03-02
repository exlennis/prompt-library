# Claude prompting guide: Extended Thinking

**Bad prompt:**
<propmt>
I think there's a lot of good thinking in the past chats. I want to retain the knowledge. Let's start an artefact to include these key elements. It's a starting point, and we can go back later to refine them. Suggestions to include (not limited to):
* Consistent naming convention, including consistent separations
* Hierarchical category structure
* Command templates with rich context
   * Generic template, including sections like Purpose, Syntax, Parameters, Example Output, How to Use, and When to Use
   * Include specific examples e.g.: Directory Tree, Python Script, etc.
   * How to use structure comments in commands
I have also included the Warp system instructions for you to review. I will get started with exporting the content from the drive.
</prompt>

**Good propmt:**
<prompt>
You are tasked with creating an artifact that captures key elements from past chats and system instructions to retain valuable knowledge. This artifact will serve as a starting point for organising and structuring information for future use. Follow these instructions carefully to complete the task:

1. Review the provided inputs:
<past_chats>
{{PAST_CHATS}}
</past_chats>

<warp_system_instructions>
{{WARP_SYSTEM_INSTRUCTIONS}}
</warp_system_instructions>

2. Create an artifact that includes the following key elements:

a. Consistent Naming Convention:
   - Develop a naming convention that can be applied consistently across all elements.
   - Include guidelines for separations (e.g., underscores, hyphens, or camelCase).
   - Provide examples of how this naming convention should be applied.

b. Hierarchical Category Structure:
   - Design a hierarchical structure to organise information logically.
   - Include main categories and subcategories.
   - Ensure that the structure is flexible enough to accommodate future additions.

c. Command Templates with Rich Context:
   - Create a generic template for commands that includes:
     * Purpose
     * Syntax
     * Parameters
     * Example output
     * How to use and when to use
   - Develop specific examples for common use cases, such as:
     * Directory Tree
     * Python script
   - Provide guidelines on how to use structured comments within commands.

3. Review and refine your artifact:
   - Ensure all key elements from the past chats and Warp system instructions are incorporated.
   - Check for consistency in naming and structure throughout the artifact.
   - Verify that the command templates are clear and provide sufficient context.

4. Format your output:
   - Present your artifact in a clear, well-organised manner.
   - Use appropriate headings, subheadings, and bullet points for easy readability.
   - Include examples where necessary to illustrate concepts.

Your final output should be a comprehensive artifact that addresses all the key elements mentioned above. Focus on creating a structure that is both informative and easy to navigate. Do not include any extraneous information or explanations about the task itself. Present only the artifact content within <artifact> tags.

<artifact>
[Your well-structured artifact content goes here]
</artifact>
</prompt>