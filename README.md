[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/teched2026-JW262)](https://api.reuse.software/info/github.com/SAP-samples/teched2026-JW262)

# JW262 | OData to outcomes — Build AI-enabled SAP Fiori apps using SAP Fiori elements

## Overview

In this hands-on tutorial you will build an SAP Fiori elements application end-to-end with the help of SAP's AI developer tooling. Starting from your data model, you will create the OData service using **SAP Cloud Application Programming Model (CAP)** and generate and refine the SAP Fiori elements UI on top of it, covering the full-stack story from service to user interface.

Throughout the exercises you work inside **SAP Business Application Studio (SBAS)**, using its **AI Chat** (powered by GitHub Copilot) with an Anthropic Claude Sonnet/Opus large language model (LLM) as your AI coding assistant. The AI is guided by **MCP servers by SAP**, namely the MCP server for CAP and the MCP server for SAP Fiori, together with a set of **skills dedicated to SAP Fiori development** that encode best practices for building Fiori elements apps.

You will gain comprehensive knowledge of AI-assisted full-stack development, and learn how to kickstart your SAP Fiori elements application development.

## Using AI during App Development

When developing SAP Fiori applications with LLMs, you may encounter situations where a prompt is not executed as intended, or technical errors occur when calling MCP server tools. Knowing how to approach these issues systematically can save time and prevent disruption. SBAS AI Chat and the chosen LLM are powerful assistants for problem resolution.

### General steps in case of issues:

[Detailed steps and examples of resolving common issues](./exercises/troubleshoot/)

1. Verify connectivity:
    - Check if your machine has network access.
    - Confirm that the MCP server is up and running.

2. Approach errors systematically
    - Pause before panicking
        - Use natural pauses when the client asks for approval to inspect the current results and chat history.    
        - Stop execution with the "Cancel" button. You can always proceed from there with a new prompt
    - Identify the source: Check if the issue is:
        - CDS compiler error
        - SQLite/database error
        - Console/browser runtime error

3. Using the LLM to solve an issue
    - The LLM occasionally makes mistakes, or forgets required steps leading to error situations
    - But the LLM can read the terminal output and react to API responses, and correct errors visible there
    - Other issues, like from browser console output, can be resolved by copy-pasting the full error message into the chat and ask for a fix in a prompt
    - LLM works best when exact messages are provided rather than manual descriptions.

4. Use Restore Points if Needed
    - If a solution strategy does not work, you can always restore the files and chat to a previous checkpoint using GitHub Copilot’s restore functionality.

5. Don’t be afraid to retry an exercise or step after restoring to a checkpoint.

## Exercises

Begin your exercises here. At the end of each section, there is a link to continue to the next section.

- [Getting Started - Set up your AI Development Environment](./exercises/ex0/)

- [Exercise 1 - Create CAP Project and Fiori List Report App based on Image](./exercises/ex1.0/)
    - [Exercise 1.1 Enable automatic data loading in List Report](./exercises/ex1.1/)
    - [Exercise 1.2 Add new column destination to list report table](./exercises/ex1.2/)
    - [Exercise 1.3 Add Analytical chart to list report page](./exercises/ex1.3/)

- [Exercise 2 - Modify travel object page based on Image](./exercises/ex2.0/)
    - [Exercise 2.1 Add Custom Section with RichTextEditor Building Block](./exercises/ex2.1/)

- [Exercise 3 - Add Object Page for Booking Details](./exercises/ex3.0/)
