[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/teched2026-JW262)](https://api.reuse.software/info/github.com/SAP-samples/teched2026-JW262)

# JW262 | OData to outcomes — Build AI-enabled SAP Fiori apps using SAP Fiori elements

## Overview

In this hands-on tutorial you will experience the complete journey of an AI-assisted SAP Fiori elements application: first you build one with the help of SAP's AI developer tooling, and then you use a ready-to-run application in which AI assists the business user at runtime.

In the build part, you start from your data model, create the OData service using SAP Cloud Application Programming Model (CAP), and generate and refine the SAP Fiori elements UI on top of it, covering the full-stack story from service to user interface. You work inside SAP Business Application Studio (SBAS), using its AI Chat (powered by GitHub Copilot) with an Anthropic Claude Sonnet/Opus large language model (LLM) as your AI coding assistant. The AI is guided by MCP servers by SAP, namely the MCP server for CAP and the MCP server for SAP Fiori, together with a set of skills dedicated to SAP Fiori development that encode best practices for building Fiori elements apps.

In the runtime part, you switch perspective from developer to end user and explore a Fiori elements travel application on SAP S/4HANA Cloud that has AI built directly into the running app, assisting you while you work with travel data.

You will gain comprehensive knowledge of AI-assisted full-stack development, and see first-hand how AI enriches both the building and the using of SAP Fiori elements applications.

The tutorial is organized in two parts:

- **Part 1 - Develop with AI (build time).** In exercises 1 to 3 you build the SAP Fiori elements travel application end-to-end inside SBAS, using AI Chat, the MCP servers by SAP, and the SAP Fiori development skills as your AI-assisted toolchain.
- **Part 2 - Use an AI-enabled app (runtime).** In exercise 4 you switch perspective from developer to end user and explore a ready-to-run SAP Fiori elements travel application on SAP S/4HANA Cloud. Here the AI is built into the running app itself, assisting the business user directly while working with travel data.

Together, the two parts show the complete picture: how AI accelerates building a Fiori elements app, and how AI enriches the experience of using one.

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

### Part 1 - Build an SAP Fiori elements app with AI

- [Exercise 1.0 - Set up your AI Development Environment](./exercises/ex1.0/)
    - [Exercise 1.1 - Create a CAP project and SAP Fiori app from an image](./exercises/ex1.1/)
    - [Exercise 1.2 - Enable automatic data loading in List Report](./exercises/ex1.2/)
    - [Exercise 1.3 - Add destination column to List Report table](./exercises/ex1.3/)
    - [Exercise 1.4 - Add an analytical column chart to the List Report](./exercises/ex1.4/)

- [Exercise 2.0 - Modify travel object page based on image](./exercises/ex2.0/)
    - [Exercise 2.1 - Add Custom Section with RichTextEditor Building Block](./exercises/ex2.1/)
    
- [Exercise 3.0 - Add Object Page for Booking Details](./exercises/ex3.0/)

### Part 2 - Explore an AI-enabled SAP Fiori elements app

- [Exercise 4.0 - Set up for Part 2: open the AI-enabled Travel app](./exercises/ex4.0/)
    - [Exercise 4.1 - AI-assisted easy filter](./exercises/ex4.1/)
    - [Exercise 4.2 - AI-assisted easy fill](./exercises/ex4.2/)
    - [Exercise 4.3 - AI-assisted error explanation](./exercises/ex4.3/)
    - [Exercise 4.4 - AI-assisted smart summarization](./exercises/ex4.4/)

## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## Contributing

Please read the [CONTRIBUTING.md](./CONTRIBUTING.md) to understand the contribution guidelines.

## Code of Conduct

Please read the [SAP Open Source Code of Conduct](https://github.com/SAP-samples/.github/blob/main/CODE_OF_CONDUCT.md).

## License

Copyright (c) 2026 SAP SE or an SAP affiliate company and teched2026-JW262 contributors. Please see our [LICENSE](LICENSE) for copyright and license information. Detailed information including third-party components and their licensing/copyright information is available [via the REUSE tool](https://api.reuse.software/info/github.com/SAP-samples/teched2026-JW262).
