# Hackathon II – Todo App Constitution

This repository implements the Evolution of Todo project for Hackathon II using spec-driven development.

## Rules for Implementation

1. All features must be defined first as Markdown specs in the `specs-history` folder.
2. Code must be generated using Claude Code or a spec-driven LLM workflow based on these specs.
3. I will not manually write or edit the main application logic. Instead, I will refine the specs until the LLM produces correct code.
4. The project must follow clean code practices and be easy to understand and maintain.

## Phase I Scope

1. In-memory Python console application.
2. Features: add, list, update, delete, and toggle complete/incomplete for todo tasks.
3. No database or file storage. Tasks are stored in memory only while the program is running.
