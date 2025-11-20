## 📁 SRC Folder – File-by-File Explanation

### 1. deep-research.ts
Core engine of your research agent.

Handles the complete research pipeline.

Generates SERP queries, calls search API.

Summarizes raw results.

Creates Learning, Directions, Deep Dives, Final Report Sections.

Applies your prompt templates, chunking, progress tracking.

Orchestrates:
- search provider  
- LLM provider  
- text splitting  
- batching  
- JSON schema validation  
- section-wise report generation  

This is the main brain of the entire project.

---

### 2. depp-research1.ts
Looks like an older / experimental / backup version of deep-research.ts.

Similar imports and functions.

Likely an early prototype.

Not used in production but kept as reference.

---

### 3. feedback.ts
Generates feedback on the final report:

Reads the generated report.

Uses terminal utilities to print formatted feedback.

Provides improvement suggestions for:
- clarity  
- structure  
- accuracy  

Mainly used after report generation is complete.

---

### 4. generate-wrapper.ts
Wrapper around Gemini API.

Loads GEMINI_API_KEY.

Throws error if key missing.

Creates a Unified API client.

Exposes a helper to run Gemini LLM with:
- prompts  
- safety settings  
- maxTokens  
- temperature  
- JSON / text output  

Used by deep-research.ts and all other files requiring LLM calls.

---

## 🧠 SUPPORTING CORE UTILITIES

### 5. prompt.ts
Contains all your prompt templates:

Templates for:
- SERP Query generation  
- Outline creation  
- Topic deep dives  
- Learnings extraction  
- Report composition  

Also includes time-based greeting logic (Morning/Afternoon/Evening) → used for human-like familiarity inside prompts.

This file defines how the AI behaves during the research.

---

### 6. types.ts
Defines all TypeScript types & JSON Schemas:

- Research progress types  
- Outline schema  
- Section schema  
- Structured result objects  

Ensures your Gemini calls return valid JSON, otherwise validated.

Your entire project depends on these types for safe structured outputs.

---

## 🖥 TERMINAL + OUTPUT HANDLING

### 7. output-manager.ts
Manages all console/terminal interactions:

- Clears screen  
- Writes logs  
- Displays animations  
- Ensures consistent output formatting  

Provides helper wrappers for:
- success  
- error  
- formatted blocks  

Used throughout the research process.

---

### 8. progress-manager.ts
Handles the progress bar & step completion indicators.

Contains ANSI cursor movement controls.

Used to show real-time progress:
- Searching…  
- Generating…  
- Summarizing…  
- Finalizing…  

This makes the CLI look premium-level.

---

### 9. terminal-utils.ts
Provides low-level terminal tools:

- progress bar rendering function  
- cursor movement  
- color codes  
- screen clearing helpers  

output-manager.ts and progress-manager.ts use this internally.

---

### 10. logger.ts
Custom logger that:

- Removes sensitive keys (API keys, tokens)  
- Formats console logs for debugging  
- Works with LLM outputs and search responses  

Used inside many files for clean logs.

---

## 🔎 SEARCH + AI PROVIDERS

### 11. search/providers.ts
Handles online search using Exa Search API:

Prepares search queries.

Calls the API with API key.

Extracts:
- snippets  
- title  
- URL  
- extracted text  

Cleans search output for LLM consumption.

Used heavily by deep-research.ts.

---

### 12. ai/providers.ts
Low-level helpers for AI providers:

- Temperature clamping  
- Token control  

Utility helpers for:
- text completion  
- structured output generation  
- streaming  

Mostly used internally by your Gemini wrapper.

---

### 13. ai/text-splitter.ts
Implements your custom text splitting logic:

Splits text into chunks based on:
- length  
- separators (., ?, newlines)  
- chunk overlap  

Used to:
- chunk SERP results  
- chunk long texts  
- batch Gemini calls  

---

### 14. ai/text-splitter.test.ts
Test file containing unit tests for text splitter logic.

---

## 🧹 UTILITY & HELPER FILES

### 15. utils/json.ts
Safe JSON parsing:

- Avoids crashes if output is malformed.  
- Cleans JSON.  
- Logs JSON errors for debugging.  

Used when validating Gemini structured output.

---

### 16. utils/sanitize.ts
Cleans LLM text:

- Removes markdown artifacts  
- Removes internal model notes  
- Removes extra whitespace  

Makes content clean for report writing.

---

## ⚙️ CORE EXECUTION + SERVER

### 17. run.ts
Your main entry script.

Reads user input (topic, depth, breadth).

Initializes OutputManager.

Calls deep-research.ts.

Gets final report.

Calls feedback generator.

Writes final output to Markdown file.

This is the file you run to start the entire research pipeline.

---

### 18. mcp-server.ts
Implements your Model Context Protocol Server:

Exposes your research agent as an MCP tool.

Enables integration with:
- VSCode  
- Cursor IDE  
- Claude Desktop  

Provides:
- search tools  
- research tools  
- report generation tools  

This makes your system behave like an intelligent "backend" tool for LLM IDEs.
