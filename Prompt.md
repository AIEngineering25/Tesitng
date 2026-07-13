Based on this create a architecture diagram:

QA Copilot
multiple specialized agents.

│
├── Knowledge Agent
│      Reads project documents
│      Builds QA knowledge
│
├── Requirement Agent
│      Understands requirement
│      Extracts business rules
│
├── Test Design Agent
│      Creates test cases
│      Covers edge cases
│
├── Automation Agent
│      Generates automation scripts
│
├── Execution Agent
│      Executes tests
│
├── Evidence Agent
│      Creates screenshots
│      Creates logs
│      Creates execution evidence
│
├── Reporting Agent
│      Summary Report
│      Jira Report
│      Metrics
│
└── Knowledge Update Agent
       Learns from approved documents
       Updates project knowledge


qa-copilot/

│
├── .github/
│   ├── copilot-instructions.md
│   └── prompts/
│
├── agents/
│   ├── knowledge-agent.md
│   ├── requirement-agent.md
│   ├── testcase-agent.md
│   ├── automation-agent.md
│   ├── execution-agent.md
│   ├── evidence-agent.md
│   ├── reporting-agent.md
│   └── learning-agent.md
│
├── prompts/
│   ├── generate-testcase.prompt.md
│   ├── review-testcase.prompt.md
│   ├── jira.prompt.md
│   ├── summary.prompt.md
│   └── automation.prompt.md
│
├── knowledge/
│   ├── vector-db/
│   ├── embeddings/
│   ├── project-summary.json
│   ├── modules.json
│   ├── business-rules.json
│   ├── glossary.json
│   └── testcase-index.json
│
├── templates/
│   ├── testcase-template.xlsx
│   ├── jira-template.docx
│   ├── summary-template.docx
│   ├── evidence-template.docx
│   └── execution-template.xlsx
│
├── automation/
│   ├── playwright/
│   ├── selenium/
│   ├── api/
│   └── mobile/
│
├── reports/
│   ├── summary/
│   ├── jira/
│   ├── evidence/
│   └── execution/
│
├── connectors/
│   ├── sharepoint/
│   ├── confluence/
│   ├── jira/
│   ├── azure-devops/
│   └── github/
│
├── config/
│   ├── project.yaml
│   ├── company.yaml
│   └── qa-settings.yaml
│
└── extension/
    ├── commands.ts
    ├── sidebar.ts
    ├── chat.ts
    └── package.json

chat window, provide a dedicated QA panel. Where use has these options but can also just simply enter like this  e.g  Write tests cases for tis JIRA issue -> then user copy paste text from jira board itself  sample -> JIRA ID ABC-1120 Home Screen footers flickering issue  description: Home screen page footers flickers on 1st time page is loaded or when its reloaded  Steps to reproduces:  Step1 Step 2 Expected behaviour: No flickering  Actual behaviour: flickering 
----------------------------------------------

QA Copilot

📚 Build Knowledge

📄 Generate Test Cases

🤖 Generate Automation

▶ Execute Tests

📸 Generate Evidence

📊 Create Summary

🐞 Generate Jira

🔄 Update Knowledge

----------------------------------------------

Knowledge Status

✔ Indexed

Modules : 28

Requirements : 421

Test Cases : 5,630

Business Rules : 812

Last Updated :
Today 10:15 AM

----------------------------------------------





















You are a Principal AI Engineer, Enterprise Software Architect, Senior QA Architect, and VS Code Extension Expert.

Your responsibility is to design and build an enterprise-grade AI QA Copilot Platform that works inside VS Code using GitHub Copilot Chat as the primary interface.

This is NOT a demo project.

This is NOT a simple prompt engineering project.

This is a production-grade enterprise platform designed for Fortune 500 companies.

Your goal is to design the software exactly like an experienced enterprise architect would.

====================================================

PROJECT NAME

QA Copilot Enterprise

====================================================

MISSION

Automate the Manual Testing SDLC using AI.

The AI should think exactly like an experienced Manual QA Engineer.

It should understand requirements, understand existing project knowledge, generate professional test cases, execute automation, generate evidence, create reports, and continuously improve project knowledge.

IMPORTANT

V1 WILL NOT USE SOURCE CODE.

NO GitHub analysis.

NO AST parsing.

NO code impact analysis.

The AI should behave exactly like a Manual Tester.

Knowledge comes ONLY from functional project documents.

GitHub integration will be implemented in V2.

====================================================

PRIMARY OBJECTIVES

Build a production-ready architecture.

Design reusable components.

Design scalable modules.

Design loosely coupled services.

Design enterprise folder structure.

Design maintainable code.

Design extensible AI agents.

Design reusable prompts.

Design reusable templates.

====================================================

SYSTEM ARCHITECTURE

The system must contain four layers.

----------------------------------------------------

Layer 1

Presentation Layer

----------------------------------------------------

VS Code Extension

GitHub Copilot Chat

Dedicated QA Sidebar

Commands

Settings

Progress Indicators

Status Panel

Knowledge Dashboard

----------------------------------------------------

Layer 2

AI Orchestrator

----------------------------------------------------

The Orchestrator is the brain.

Users NEVER call agents directly.

The Orchestrator receives every request.

Example

Generate test cases for Login enhancement.

The Orchestrator should

Understand intent

Select required agents

Retrieve project knowledge

Maintain conversation context

Pass outputs between agents

Avoid duplicate processing

Handle retries

Log execution

Return final result

Future agents should plug into the orchestrator without changing existing workflows.

====================================================

Layer 3

Specialized AI Agents

Create the following agents.

Knowledge Agent

Responsibilities

Read project documents

Build semantic knowledge

Index knowledge

Retrieve relevant knowledge

Update knowledge

Requirement Agent

Responsibilities

Understand BRD

Understand FRD

Understand User Stories

Extract business rules

Extract validations

Extract workflows

Identify testable scenarios

Test Design Agent

Responsibilities

Generate manual test cases

Positive cases

Negative cases

Boundary tests

Edge cases

Regression suggestions

Data validation

Permission validation

Error validation

Automation Agent

Responsibilities

Generate Playwright automation

Reuse existing scripts

Maintain framework

Organize scripts

Execution Agent

Responsibilities

Execute tests

Collect outputs

Validate results

Handle failures

Evidence Agent

Responsibilities

Capture screenshots

Capture logs

Capture videos

Collect execution evidence

Generate evidence package

Reporting Agent

Responsibilities

Generate summary report

Generate Jira defect report

Generate Jira closure comments

Generate metrics

Generate requirement traceability

Knowledge Update Agent

Responsibilities

Learn ONLY from approved documents

Never hallucinate knowledge

Refresh embeddings

Update semantic search

Update indexes

====================================================

Layer 4

Knowledge Layer

Design an enterprise knowledge engine.

Store

Project Summary

Business Rules

Requirement Index

Modules

Glossary

Existing Test Cases

Previous Defects

Release Notes

Embeddings

Vector Database

Semantic Search

The AI should NEVER load the entire project.

Always retrieve only relevant context.

====================================================

CONNECTORS

Design connectors for

SharePoint

Confluence

Jira

Azure DevOps

Local Folder

PDF

Word

Excel

Markdown

Future

GitHub

GitLab

Bitbucket

====================================================

OUTPUTS

Generate

Professional Test Cases

Automation Scripts

Execution Reports

Evidence Documents

Jira Ready Documents

Summary Reports

Requirement Traceability Matrix

Regression Reports

====================================================

VS CODE SIDEBAR

Create a dedicated QA Sidebar.

It should contain

Build Knowledge

Generate Test Cases

Generate Automation

Execute Tests

Generate Evidence

Generate Summary

Generate Jira

Update Knowledge

Knowledge Status

Indexed

Modules

Requirements

Business Rules

Test Cases

Last Updated

====================================================

PROJECT STRUCTURE

Generate a production-grade folder structure.

Example

.github/

agents/

prompts/

knowledge/

automation/

reports/

templates/

connectors/

config/

extension/

services/

core/

utils/

storage/

api/

tests/

====================================================

ENGINEERING PRINCIPLES

Follow

SOLID

DRY

KISS

Clean Architecture

Domain Driven Design

Dependency Injection

Factory Pattern

Strategy Pattern

Repository Pattern

Adapter Pattern

Orchestrator Pattern

Event Driven Communication

====================================================

AI PRINCIPLES

Every agent should

Have one responsibility

Receive structured input

Produce structured output

Never duplicate work

Never access unrelated knowledge

Always use retrieval

Log reasoning

Return confidence score

====================================================

PROMPTS

Store prompts separately.

Each agent should own its own prompt.

No hardcoded prompts inside code.

====================================================

CONFIGURATION

All settings should be configurable.

Company configuration

Project configuration

AI configuration

Prompt configuration

Export configuration

Automation configuration

====================================================

EXPORTS

Support

Excel

Word

PDF

Markdown

JSON

CSV

====================================================

REPORTING

Generate

Executive Summary

QA Summary

Defect Summary

Requirement Coverage

Automation Coverage

Execution Metrics

====================================================

CODE QUALITY

Write production-ready code.

No shortcuts.

No prototype code.

No TODOs.

No placeholders.

Use meaningful class names.

Use meaningful interfaces.

Use dependency injection.

Write modular code.

====================================================

DOCUMENTATION

Generate

Architecture document

High-Level Design

Low-Level Design

API documentation

Folder documentation

Developer Guide

Installation Guide

Configuration Guide

User Guide

====================================================

FUTURE READY

The architecture must support future additions.

Examples

GitHub Integration

Impact Analysis Agent

Code Knowledge Agent

Regression Intelligence Agent

Risk Prediction Agent

Release Readiness Agent

LLM Provider Switching

Multiple AI Models

MCP Servers

====================================================

EXPECTED OUTPUT

Generate everything step by step.

Do NOT skip architecture.

Start with

1. High-Level Architecture
2. Low-Level Architecture
3. Folder Structure
4. Component Design
5. Class Diagram
6. Database Design
7. Knowledge Engine
8. AI Agent Design
9. Prompt Design
10. VS Code Extension Design
11. APIs
12. Workflows
13. Sequence Diagrams
14. Deployment Architecture
15. Security
16. Logging
17. Monitoring
18. Testing Strategy
19. Documentation
20. Implementation Roadmap

Think like a Principal Engineer building a commercial enterprise product that thousands of QA engineers will use daily.
