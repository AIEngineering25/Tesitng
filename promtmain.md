You are a Principal AI Architect and GitHub Copilot Agent Engineer.

Create a production-grade VS Code GitHub Copilot Custom Agent system for an enterprise QA automation intelligence platform.

The agent system must NOT be a single monolithic agent.

Design a modular multi-agent architecture using multiple markdown based Copilot custom agents.

Create:

1. Master Orchestrator Agent

Responsible for:
- Understanding user intent
- Delegating tasks
- Managing workflow between agents
- Maintaining project state


2. Project Knowledge Mining Agent

Responsibilities:
- Read BA documents
- DFS documents
- BRD
- FRD
- SRS
- QA documents
- Existing test cases
- Jira exports
- Automation scripts

Convert them into optimized machine-readable knowledge.

Create:
- JSON schemas
- metadata indexes
- embeddings
- knowledge graph structure


3. Knowledge Optimization Agent

Implement hybrid RAG architecture:

- Vector database
- Knowledge graph
- Metadata search

Optimize:
- token consumption
- retrieval accuracy
- context compression

Use:
- semantic chunking
- embeddings
- entity extraction
- relationship mapping


4. Test Case Generation Agent

Input:
- user stories
- bugs
- requirements
- acceptance criteria

Generate professional QA test cases covering:

- positive scenarios
- negative scenarios
- edge cases
- boundary testing
- regression scenarios
- security scenarios
- API scenarios
- database validations


Store internally in JSON.

Create converters for:

- Excel
- Word
- PDF


5. Test Documentation Agent

Analyze existing project test case templates.

Extract:

- formatting
- colors
- fonts
- layouts
- structures

Create reusable Python generators.

Improve templates professionally while maintaining project standards.


6. Playwright Automation Agent

Automatically:

- convert test cases into automation scripts
- maintain page object model
- execute tests
- capture screenshots
- capture videos
- generate reports


7. Jira Defect Agent

For failed automation:

Generate Jira-ready bug templates containing:

- summary
- description
- environment
- reproduction steps
- expected result
- actual result
- evidence


8. Learning Optimization Agent

Maintain controlled learning database.

Store:

- successful automation patterns
- locator strategies
- common failures
- reusable components

Improve future generation accuracy.


Technical Requirements:

Architecture:

.github/
  copilot/
    agents/
    instructions/
    workflows/


Use markdown files only for Copilot agent definitions.

Create Python utilities where required.

Use a single reusable virtual environment.

Never reinstall dependencies unnecessarily.

Create:

- folder structure
- all agent markdown files
- instruction files
- workflow files
- JSON schemas
- Python utility placeholders
- README explaining usage


Follow enterprise software engineering standards.

Optimize everything for:
- minimum LLM tokens
- maximum retrieval accuracy
- maintainability
- scalability
- security


Act as a senior AI engineer designing this for a large enterprise QA organization.