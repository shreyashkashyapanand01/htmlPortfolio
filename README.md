# Project Documentation — Automated Detailed Summary

Generated using file analysis heuristics. File contents were inspected; summaries below aim to capture purpose, key symbols, and top comments where present.

**Repository path:** `/mnt/data/project_extract/collegeMajorProject1`

----

## `.cursorrules`  — 47.9 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** invokeDeepResearchTool, callGeminiProConfigurable, callRawGeminiAPI, performGoogleSearchLocalized, chunkTextWithTiktoken, loadCursorRulesData, createThought, Q, DR, DP, MR, NL, result, mcp, model, response, geminiResponseDefault, geminiResponseVision, geminiResponseSafe, genAI, geminiResponse, serpApiClient, params, basicSearchResults, localizedResultsGB, encoder, tokens, longText, textChunks, smallerChunks, data, cursorRules, newThought, output, filteredArray, to, entry, and, MyObject, name

- **Top comment / preview:**

```
.cursorrules
```

- **Heuristic summary:** Auxiliary file or asset.

- **Likely responsibilities:**

  - `invokeDeepResearchTool` — referenced or defined in this file.
  - `callGeminiProConfigurable` — referenced or defined in this file.
  - `callRawGeminiAPI` — referenced or defined in this file.
  - `performGoogleSearchLocalized` — referenced or defined in this file.
  - `chunkTextWithTiktoken` — referenced or defined in this file.
  - `loadCursorRulesData` — referenced or defined in this file.

---

## `.env.Example`  — 6.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
-----------------------------------------------------------------------------
GEMINI_API_KEY=
Description: API key used for Google's Gemini models.
Required: Yes (src/deep-research.ts expects this; the app cannot run without it)
How to obtain: From Google AI Studio/Google Cloud project with Generative AI access.
Example format: AIza... (never commit a real key)
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/HEAD`  — 0.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
ref: refs/heads/main
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/config`  — 0.3 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
[core]
	repositoryformatversion = 0
	filemode = false
	bare = false
	logallrefupdates = true
	symlinks = false
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/description`  — 0.1 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
Unnamed repository; edit this file 'description' to name the repository.
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/applypatch-msg.sample`  — 0.5 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh

An example hook script to check the commit log message taken by
applypatch from an e-mail message.

The hook should exit with non-zero status after issuing an
appropriate message if it wants to stop the commit.  The hook is
allowed to edit the commit message file.

To enable this hook, rename this file to "applypatch-msg".
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/commit-msg.sample`  — 0.9 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh

An example hook script to check the commit log message.
Called by "git commit" with one argument, the name of the file
that has the commit message.  The hook should exit with non-zero
status after issuing an appropriate message if it wants to stop the
commit.  The hook is allowed to edit the commit message file.

To enable this hook, rename this file to "commit-msg".
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/fsmonitor-watchman.sample`  — 4.6 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** version

- **Top comment / preview:**

```
!/usr/bin/perl
```

- **Heuristic summary:** Auxiliary file or asset.

- **Likely responsibilities:**

  - `version` — referenced or defined in this file.

---

## `.git/hooks/post-update.sample`  — 0.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh

An example hook script to prepare a packed repository for use over
dumb transports.

To enable this hook, rename this file to "post-update".
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/pre-applypatch.sample`  — 0.4 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh

An example hook script to verify what is about to be committed
by applypatch from an e-mail message.

The hook should exit with non-zero status after issuing an
appropriate message if it wants to stop the commit.

To enable this hook, rename this file to "pre-applypatch".
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/pre-commit.sample`  — 1.6 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh

An example hook script to verify what is about to be committed.
Called by "git commit" with no arguments.  The hook should
exit with non-zero status after issuing an appropriate message if
it wants to stop the commit.

To enable this hook, rename this file to "pre-commit".
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/pre-merge-commit.sample`  — 0.4 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh

An example hook script to verify what is about to be committed.
Called by "git merge" with no arguments.  The hook should
exit with non-zero status after issuing an appropriate message to
stderr if it wants to stop the merge commit.

To enable this hook, rename this file to "pre-merge-commit".
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/pre-push.sample`  — 1.3 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/pre-rebase.sample`  — 4.8 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh

Copyright (c) 2006, 2008 Junio C Hamano

The "pre-rebase" hook is run just before "git rebase" starts doing
its job, and can prevent the command from running by exiting with
non-zero status.

The hook is called with the following parameters:

$1 -- the upstream the series was forked from.
$2 -- the branch being rebased (or empty when rebasing the current branch).

This sample shows how to prevent topic branches that are already
merged to 'next' branch from getting rebased, because allowing it
would result in rebasing already published history.
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/pre-receive.sample`  — 0.5 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh

An example hook script to make use of push options.
The example simply echoes all push options that start with 'echoback='
and rejects all pushes when the "reject" push option is used.

To enable this hook, rename this file to "pre-receive".
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/prepare-commit-msg.sample`  — 1.5 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh

An example hook script to prepare the commit log message.
Called by "git commit" with the name of the file that has the
commit message, followed by the description of the commit
message's source.  The hook's purpose is to edit the commit
message file.  If the hook fails with a non-zero status,
the commit is aborted.

To enable this hook, rename this file to "prepare-commit-msg".
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/push-to-checkout.sample`  — 2.7 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/sendemail-validate.sample`  — 2.3 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/hooks/update.sample`  — 3.6 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
!/bin/sh

An example hook script to block unannotated tags from entering.
Called by "git receive-pack" with arguments: refname sha1-old sha1-new

To enable this hook, rename this file to "update".

Config
------
hooks.allowunannotated
This boolean sets whether unannotated tags will be allowed into the
repository.  By default they won't be.
hooks.allowdeletetag
This boolean sets whether deleting tags will be allowed in the
repository.  By default they won't be.
hooks.allowmodifytag
This boolean sets whether a tag may be modified after creation. By default
it won't be.
hooks.allowdeletebranch
This boolean sets whether deleting branches will be allowed in the
repository.  By default they won't be.
hooks.denycreatebranch
This boolean sets whether remotely creating branches will be denied
in th
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/index`  — 5.6 KB

- **Text file:** No

- **Detected symbols/functions/classes:** None detected

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/info/exclude`  — 0.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
git ls-files --others --exclude-from=.git/info/exclude
Lines that start with '#' are comments.
For a project mostly in C, the following would be a good set of
exclude patterns (uncomment them if you want to use them):
.[oa]
~
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/logs/HEAD`  — 0.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
0000000000000000000000000000000000000000 7a6dd3e49e6d69ff297a6b78b7c60a2dd1d5f21e shreyashkashyapanand01 <shreyashkashyapanand01@gmail.com> 1763587015 +0530	clone: from https://github.com/shreyashkashyapanand01/collegeMajorProject1.git
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/logs/refs/heads/main`  — 0.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
0000000000000000000000000000000000000000 7a6dd3e49e6d69ff297a6b78b7c60a2dd1d5f21e shreyashkashyapanand01 <shreyashkashyapanand01@gmail.com> 1763587015 +0530	clone: from https://github.com/shreyashkashyapanand01/collegeMajorProject1.git
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/logs/refs/remotes/origin/HEAD`  — 0.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
0000000000000000000000000000000000000000 7a6dd3e49e6d69ff297a6b78b7c60a2dd1d5f21e shreyashkashyapanand01 <shreyashkashyapanand01@gmail.com> 1763587015 +0530	clone: from https://github.com/shreyashkashyapanand01/collegeMajorProject1.git
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/objects/pack/pack-e40406e1442fb2f7b800058fcd0f544cb147f042.idx`  — 4.5 KB

- **Text file:** No

- **Detected symbols/functions/classes:** None detected

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/objects/pack/pack-e40406e1442fb2f7b800058fcd0f544cb147f042.pack`  — 1590.8 KB

- **Text file:** No

- **Detected symbols/functions/classes:** None detected

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/objects/pack/pack-e40406e1442fb2f7b800058fcd0f544cb147f042.rev`  — 0.6 KB

- **Text file:** No

- **Detected symbols/functions/classes:** None detected

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/packed-refs`  — 0.1 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
pack-refs with: peeled fully-peeled sorted
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/refs/heads/main`  — 0.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
7a6dd3e49e6d69ff297a6b78b7c60a2dd1d5f21e
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.git/refs/remotes/origin/HEAD`  — 0.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
ref: refs/remotes/origin/main
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.gitignore`  — 0.8 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
See https://help.github.com/articles/ignoring-files/ for more about ignoring files.
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.prettierignore`  — 0.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
.hbs
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.specstory/.gitignore`  — 0.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
SpecStory explanation file
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `.windsurf/rules/00-critical-code-practices.md`  — 0.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
---
trigger: manual
glob:
description:
---
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.


---

## `.windsurf/rules/01-project.md`  — 4.5 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** client, modelId, model, response, json, toolDefs, toolModel

- **Top comment / preview:**

```
Deep Research MCP Server – Rules for Contributors
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.

- **Likely responsibilities:**

  - `client` — referenced or defined in this file.
  - `modelId` — referenced or defined in this file.
  - `model` — referenced or defined in this file.
  - `response` — referenced or defined in this file.
  - `json` — referenced or defined in this file.
  - `toolDefs` — referenced or defined in this file.

---

## `.windsurf/rules/02-chunking-and-splitting-rules.md`  — 1.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
Chunking and Text Splitting Rules
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.


---

## `.windsurf/rules/03-mcp-server.md`  — 8.1 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** server, transport, result, report, for

- **Top comment / preview:**

```
MCP Server Rules (src/mcp-server.ts)
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.

- **Likely responsibilities:**

  - `server` — referenced or defined in this file.
  - `transport` — referenced or defined in this file.
  - `result` — referenced or defined in this file.
  - `report` — referenced or defined in this file.
  - `for` — referenced or defined in this file.

---

## `.windsurf/rules/04-gemini-structured-output-rules.md`  — 0.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
---
trigger: manual
glob:
description:
---
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.


---

## `.windsurf/rules/05-google-search-grounding-rules.md`  — 0.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
---
trigger: manual
glob:
description:
---
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.


---

## `Dockerfile`  — 0.1 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
FROM node:18-alpine
WORKDIR /app
COPY . .
COPY package.json ./
COPY .env.local ./.env.local
RUN npm install
```

- **Heuristic summary:** Deployment or CI configuration file.


---

## `LICENSE`  — 1.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
MIT License
Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `README.md`  — 16.6 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** invokeDeepResearchTool, Q, DR, DP, MR, NL, mcp, result

- **Top comment / preview:**

```
Deep Researcher
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.

- **Likely responsibilities:**

  - `invokeDeepResearchTool` — referenced or defined in this file.
  - `Q` — referenced or defined in this file.
  - `DR` — referenced or defined in this file.
  - `DP` — referenced or defined in this file.
  - `MR` — referenced or defined in this file.
  - `NL` — referenced or defined in this file.

---

## `backend/.env.Example`  — 6.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
-----------------------------------------------------------------------------
GEMINI_API_KEY=
Description: API key used for Google's Gemini models.
Required: Yes (src/deep-research.ts expects this; the app cannot run without it)
How to obtain: From Google AI Studio/Google Cloud project with Generative AI access.
Example format: AIza... (never commit a real key)
```

- **Heuristic summary:** Backend server code (likely Node/Express or similar) — handles API, server logic and data.


---

## `backend/server.ts`  — 1.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** __filename, __dirname, app, report, frontendPath, port

- **Top comment / preview:**

```
ESM-safe __dirname support
```

- **Heuristic summary:** Backend server code (likely Node/Express or similar) — handles API, server logic and data.

- **Likely responsibilities:**

  - `__filename` — referenced or defined in this file.
  - `__dirname` — referenced or defined in this file.
  - `app` — referenced or defined in this file.
  - `report` — referenced or defined in this file.
  - `frontendPath` — referenced or defined in this file.
  - `port` — referenced or defined in this file.

---

## `docker-compose.yml`  — 0.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
services:
  deep-research:
    container_name: deep-research
    build: .
    env_file:
      - .env.local
```

- **Heuristic summary:** Deployment or CI configuration file.


---

## `docs-cursorrules/code_snippets_deep_research.cursorrules`  — 5.4 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** testGenerateQueries, testProcessSERP, testWriteReport, runMinimalDeepResearch, researchQuery, serpQueries, searchQuery, mockSerpResult, processingResult, researchPrompt, exampleLearnings, exampleUrls, reportMarkdown, breadth, depth, researchResult

- **Top comment / preview:**

```
@snippet-category(name: "deep-research.ts - Core Logic Snippets") {
  @snippet(name: "Call generateSerpQueries Function", description: "Snippet to call the generateSerpQueries function with a user query") {
    @code(language: "typescript") {
      ```typescript
      import { generateSerpQueries } from './deep-research'; // Adjust path if needed
      async function testGenerateQueries() {
```

- **Heuristic summary:** Auxiliary file or asset.

- **Likely responsibilities:**

  - `testGenerateQueries` — referenced or defined in this file.
  - `testProcessSERP` — referenced or defined in this file.
  - `testWriteReport` — referenced or defined in this file.
  - `runMinimalDeepResearch` — referenced or defined in this file.
  - `researchQuery` — referenced or defined in this file.
  - `serpQueries` — referenced or defined in this file.

---

## `docs/rules/chunking-and-splitting-rules.md`  — 1.1 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
Chunking and Text Splitting Rules
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.


---

## `docs/rules/exa-provider-rules.md`  — 1.7 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** exa, results, contents

- **Top comment / preview:**

```
Exa Provider Rules (Primary Search/Crawl)
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.

- **Likely responsibilities:**

  - `exa` — referenced or defined in this file.
  - `results` — referenced or defined in this file.
  - `contents` — referenced or defined in this file.

---

## `docs/rules/gemini-structured-output-rules.md`  — 1.8 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** response

- **Top comment / preview:**

```
Gemini Structured Output Rules
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.

- **Likely responsibilities:**

  - `response` — referenced or defined in this file.

---

## `docs/rules/google-search-grounding-rules.md`  — 1.3 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
Google Search Grounding Rules
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.


---

## `docs/rules/jest-testing-rules.md`  — 1.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
Testing Rules (Jest + TypeScript ESM)
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.


---

## `docs/rules/mcp-server-rules.md`  — 7.9 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** server, transport, result, report, for

- **Top comment / preview:**

```
MCP Server Rules (src/mcp-server.ts)
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.

- **Likely responsibilities:**

  - `server` — referenced or defined in this file.
  - `transport` — referenced or defined in this file.
  - `result` — referenced or defined in this file.
  - `report` — referenced or defined in this file.
  - `for` — referenced or defined in this file.

---

## `docs/rules/windsurf-core-rules.md`  — 2.7 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
Windsurf Core Rules for This Project
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.


---

## `docs/windsurf-rules.md`  — 4.5 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** client, modelId, model, response, json, toolDefs, toolModel

- **Top comment / preview:**

```
Deep Research MCP Server – Rules for Contributors
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.

- **Likely responsibilities:**

  - `client` — referenced or defined in this file.
  - `modelId` — referenced or defined in this file.
  - `model` — referenced or defined in this file.
  - `response` — referenced or defined in this file.
  - `json` — referenced or defined in this file.
  - `toolDefs` — referenced or defined in this file.

---

## `frontend/.env.Example`  — 6.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
-----------------------------------------------------------------------------
GEMINI_API_KEY=
Description: API key used for Google's Gemini models.
Required: Yes (src/deep-research.ts expects this; the app cannot run without it)
How to obtain: From Google AI Studio/Google Cloud project with Generative AI access.
Example format: AIza... (never commit a real key)
```

- **Heuristic summary:** Frontend application code — UI components, assets, build config.


---

## `frontend/index.html`  — 9.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
<!-- jsPDF for PDF export -->
```

- **Heuristic summary:** Frontend application code — UI components, assets, build config.


---

## `frontend/script.js`  — 5.3 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** startSimulatedProgress, stopSimulatedProgress, updateProgress, downloadMarkdown, downloadPDF, topicEl, depthEl, breadthEl, notesEl, startBtn, clearBtn, outputEl, downloadMd, downloadPdf, progressBar, progressLabel, progressPct, metaInfo, themeCheckbox, knob, body, clamped, blob, url, doc, lines, topic, depth, breadth, notes, res, data, report, safeName

- **Top comment / preview:**

```
frontend script.js — Blue Cyber Tech UI
This file does frontend-only simulated progress, calls /generate-report, and handles downloads + dark mode
```

- **Heuristic summary:** Frontend application code — UI components, assets, build config.

- **Likely responsibilities:**

  - `startSimulatedProgress` — referenced or defined in this file.
  - `stopSimulatedProgress` — referenced or defined in this file.
  - `updateProgress` — referenced or defined in this file.
  - `downloadMarkdown` — referenced or defined in this file.
  - `downloadPDF` — referenced or defined in this file.
  - `topicEl` — referenced or defined in this file.

---

## `output.md`  — 22.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** hierarchy, members, providing, has, acquires, that, non, with

- **Top comment / preview:**

```
Object-Oriented Programming in Java: A Research Report
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.

- **Likely responsibilities:**

  - `hierarchy` — referenced or defined in this file.
  - `members` — referenced or defined in this file.
  - `providing` — referenced or defined in this file.
  - `has` — referenced or defined in this file.
  - `acquires` — referenced or defined in this file.
  - `that` — referenced or defined in this file.

---

## `package-lock.json`  — 399.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Heuristic summary:** Auxiliary file or asset.


---

## `package.json`  — 1.9 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
{
  "name": "deep-research",
  "version": "0.3.0",
  "main": "dist/mcp-server.js",
  "type": "module",
  "scripts": {
```

- **Heuristic summary:** Node project manifest for **deep-research** listing scripts and dependencies (examples: version, main, type, format, tsx, start, build)


---

## `prettier.config.mjs`  — 0.5 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
@type {import('prettier').Config} */
```

- **Heuristic summary:** Auxiliary file or asset.


---

## `report.md`  — 26.1 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** gemini_request, main, gemini_websocket, run, for, and

- **Top comment / preview:**

```
I. Executive Summary**
```

- **Heuristic summary:** Markdown document — likely documentation, README or report.

- **Likely responsibilities:**

  - `gemini_request` — referenced or defined in this file.
  - `main` — referenced or defined in this file.
  - `gemini_websocket` — referenced or defined in this file.
  - `run` — referenced or defined in this file.
  - `for` — referenced or defined in this file.
  - `and` — referenced or defined in this file.

---

## `report2.md`  — 15.8 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Heuristic summary:** Markdown document — likely documentation, README or report.


---

## `screenshots_UI/generated_pdf.png`  — 236.7 KB

- **Text file:** No

- **Detected symbols/functions/classes:** None detected

- **Heuristic summary:** Auxiliary file or asset.


---

## `screenshots_UI/homepage.png`  — 397.0 KB

- **Text file:** No

- **Detected symbols/functions/classes:** None detected

- **Heuristic summary:** Auxiliary file or asset.


---

## `screenshots_UI/terminal.png`  — 145.9 KB

- **Text file:** No

- **Detected symbols/functions/classes:** None detected

- **Heuristic summary:** Auxiliary file or asset.


---

## `src/README.md`  — 0.0 KB

- **Text file:** No

- **Detected symbols/functions/classes:** None detected

- **Heuristic summary:** Markdown document — likely documentation, README or report.


---

## `src/ai/providers.ts`  — 18.7 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** createPrompt, getChunkSize, extractText, extractCitations, SemanticTextSplitter, clampNumber, generateTextEmbedding, baseConfig, hashKey, defaultTools, extractTextFromRaw, generateContentInternal, countTokens, trimPrompt, callGeminiProConfigurable, semanticChunking, adaptivePrompt, generateWithTools, generateBatch, generateBatchWithTools, generateAnalysisPlan, generateFinalFromPlan, API_KEY, client, MODEL, MAX_TOKENS, TEMPERATURE, TOP_P, TOP_K, CANDIDATE_COUNT, THINKING_BUDGET_TOKENS, ENABLE_URL_CONTEXT, ENABLE_GEMINI_GOOGLE_SEARCH, ENABLE_GEMINI_CODE_EXECUTION, ENABLE_GEMINI_FUNCTIONS, ENABLE_PROVIDER_CACHE, PROVIDER_CACHE_MAX, PROVIDER_CACHE_TTL_MS, ai, EMBEDDING_MODEL, values, providerCache, parts, firstText, toolsCombined, configObj, cacheKey, hit, raw, textVal, wrapped, o3MiniModel, o3MiniModel2, researchModel, res, contents, tokenLength, overflowTokens, approxCharsPerToken, sliceLen, normalized, sentences, rc, embs, start, first, next, nextEmb, sim, merged, mergedTokens, withinBudget, effectiveSplitter, baseEmbedding, contextEmbeddings, relevantContext, urlRegex, refRegex, urls, refs, results, i, item, urlBlock, prompt, TextSplitter, EmbedVector, EmbedResponse, Empty, Tool, GenExtra, Part, ContentMsg, ContentArg, GenerateRaw, GenerateWrapped, ResearchResultOutput

- **Top comment / preview:**

```
Environment and client setup
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `createPrompt` — referenced or defined in this file.
  - `getChunkSize` — referenced or defined in this file.
  - `extractText` — referenced or defined in this file.
  - `extractCitations` — referenced or defined in this file.
  - `SemanticTextSplitter` — referenced or defined in this file.
  - `clampNumber` — referenced or defined in this file.

---

## `src/ai/text-splitter.test.ts`  — 2.5 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** text, largeText, specialCharText

- **Top comment / preview:**

```
Test with initial chunkSize
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `text` — referenced or defined in this file.
  - `largeText` — referenced or defined in this file.
  - `specialCharText` — referenced or defined in this file.

---

## `src/ai/text-splitter.ts`  — 5.3 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** RecursiveCharacterTextSplitter, SemanticTextSplitter, TiktokenTextSplitter, target, step, splitRecursive, trimmed, piece, sep, parts, candidate, normalized, enc, ids, slice, TextSplitterParams

- **Top comment / preview:**

```
Pure text splitting utilities (no Gemini here). Providers own all Gemini logic.
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `RecursiveCharacterTextSplitter` — referenced or defined in this file.
  - `SemanticTextSplitter` — referenced or defined in this file.
  - `TiktokenTextSplitter` — referenced or defined in this file.
  - `target` — referenced or defined in this file.
  - `step` — referenced or defined in this file.
  - `splitRecursive` — referenced or defined in this file.

---

## `src/deep-research.ts`  — 33.3 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** validateAcademicInput, validateAcademicOutput, logResearchProgress, cacheSearchResults, generateSerpQueries, processSerpResult, generateOutline, writeReportFromOutline, generateSummary, generateTitle, deepResearch, writeFinalReport, research, processGeminiResponse, conductResearch, output, GEMINI_MODEL, CONCURRENCY_LIMIT, ConcurrencyLimit, SerpQuerySchema, DEFAULT_NUM_QUERIES, serpQueryCache, reportCache, prettyJson, minifiedResultsJson, learningsHash, cachedResult, query, sanitizedLearnings, prompt, finalPrompt, geminiText, rawQueriesJSON, queryValue, q, parsed, createResearchSplitter, contents, resolvedContents, urls, splitter, firstUrl, prompts, batchResults, text, parsedResult, outlinePrompt, json, outline, cleanOutline, cleanLearnings, reportPrompt, body, citations, summaryPrompt, titlePrompt, DEFAULT_DEPTH, DEFAULT_BREADTH, serpQueries, limit, limitedProcessResult, geminiResponseText, geminiResult, result, firecrawlResult, newBreadth, newDepth, processResult, allLearnings, allUrls, nextQuery, deeper, promises, results, processedData, firecrawlResponse, visitedUrlsHash, cachedReport, report, summary, title, finalReport, finalReportContent, researchResult, responseData, citationMatches, citationDensity, recentSources, conflictDisclosures, chunks, limitedChunks, batch, createEmptyResearchResult, isObject, processFirecrawlData, dataRaw, data, metadata, success, error, ResearchResult, ProcessResult, ResearchProgress, researchProgress, DeepResearchOptions, WriteFinalReportParams, ResearchOptions, GeminiItem, GeminiResponse, ProcessedGeminiResponse, FirecrawlResult, to, SearchResponse, SerpQuery

- **Top comment / preview:**

```
Rename your local type to avoid conflict
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `validateAcademicInput` — referenced or defined in this file.
  - `validateAcademicOutput` — referenced or defined in this file.
  - `logResearchProgress` — referenced or defined in this file.
  - `cacheSearchResults` — referenced or defined in this file.
  - `generateSerpQueries` — referenced or defined in this file.
  - `processSerpResult` — referenced or defined in this file.

---

## `src/depp-research1.ts`  — 33.6 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** validateAcademicInput, validateAcademicOutput, logResearchProgress, cacheSearchResults, generateSerpQueries, processSerpResult, generateOutline, writeReportFromOutline, generateSummary, generateTitle, deepResearch, writeFinalReport, research, processGeminiResponse, conductResearch, output, GEMINI_MODEL, CONCURRENCY_LIMIT, ConcurrencyLimit, SerpQuerySchema, DEFAULT_NUM_QUERIES, serpQueryCache, reportCache, prettyJson, minifiedResultsJson, learningsHash, cachedResult, query, sanitizedLearnings, prompt, finalPrompt, geminiText, rawQueriesJSON, queryValue, q, parsed, createResearchSplitter, contents, resolvedContents, urls, splitter, firstUrl, prompts, batchResults, text, parsedResult, outlinePrompt, json, outline, cleanOutline, cleanLearnings, reportPrompt, body, citations, summaryPrompt, titlePrompt, DEFAULT_DEPTH, DEFAULT_BREADTH, serpQueries, limit, limitedProcessResult, geminiResponseText, geminiResult, result, firecrawlResult, newBreadth, newDepth, processResult, allLearnings, allUrls, nextQuery, deeper, promises, results, processedData, firecrawlResponse, visitedUrlsHash, cachedReport, report, summary, title, finalReport, finalReportContent, researchResult, responseData, citationMatches, citationDensity, recentSources, conflictDisclosures, chunks, limitedChunks, batch, createEmptyResearchResult, isObject, processFirecrawlData, dataRaw, data, metadata, success, error, ResearchResult, ProcessResult, ResearchProgress, researchProgress, DeepResearchOptions, WriteFinalReportParams, ResearchOptions, GeminiItem, GeminiResponse, ProcessedGeminiResponse, FirecrawlResult, to, SearchResponse, SerpQuery

- **Top comment / preview:**

```
Rename your local type to avoid conflict
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `validateAcademicInput` — referenced or defined in this file.
  - `validateAcademicOutput` — referenced or defined in this file.
  - `logResearchProgress` — referenced or defined in this file.
  - `cacheSearchResults` — referenced or defined in this file.
  - `generateSerpQueries` — referenced or defined in this file.
  - `processSerpResult` — referenced or defined in this file.

---

## `src/feedback.ts`  — 10.4 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** analyzePastFeedback, calculateFeedbackScore, generateProgressBar, generateFeedback, output, FEEDBACK_CACHE_CONFIG, feedbackCache, FeedbackResponseSchema, DEFAULT_KEYWORDS, analysisProgress, startTime, foundKeyword, analysisTime, baseScore, penalty, filled, learningsHash, cachedFeedback, context, researchResult, analysisText, pastFeedback, geminiPrompt, totalSteps, bar, isValidOutput, FeedbackOptions, FeedbackAnalysis, FeedbackResponse, ProgressBarParams

- **Top comment / preview:**

```
Optimized cache configuration
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `analyzePastFeedback` — referenced or defined in this file.
  - `calculateFeedbackScore` — referenced or defined in this file.
  - `generateProgressBar` — referenced or defined in this file.
  - `generateFeedback` — referenced or defined in this file.
  - `output` — referenced or defined in this file.
  - `FEEDBACK_CACHE_CONFIG` — referenced or defined in this file.

---

## `src/generate-wrapper.ts`  — 1.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** generateReport, __filename, __dirname, researchResult, report

- **Top comment / preview:**

```
1️⃣ Check if key is loaded from server.ts
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `generateReport` — referenced or defined in this file.
  - `__filename` — referenced or defined in this file.
  - `__dirname` — referenced or defined in this file.
  - `researchResult` — referenced or defined in this file.
  - `report` — referenced or defined in this file.

---

## `src/logger.ts`  — 0.7 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** redactIfNeeded, level, pretty, logger, redacted

- **Top comment / preview:**

```
import pino from 'pino';
const level = (process.env.LOG_LEVEL || 'info') as pino.LevelWithSilent;
const pretty = (process.env.LOG_PRETTY || 'false').toLowerCase() === 'true';
export const logger = pino({
  level,
  ...(pretty
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `redactIfNeeded` — referenced or defined in this file.
  - `level` — referenced or defined in this file.
  - `pretty` — referenced or defined in this file.
  - `logger` — referenced or defined in this file.
  - `redacted` — referenced or defined in this file.

---

## `src/mcp-server.ts`  — 6.6 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** hashKey, __dirname, MCP_CACHE_TTL_MS, deepResearchCache, server, cacheKey, cachedResult, result, depthPct, breadthPct, queriesPct, overall, report, errorMessage, transport, name, MCPResearchResult

- **Top comment / preview:**

```
Get the directory name of the current module
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `hashKey` — referenced or defined in this file.
  - `__dirname` — referenced or defined in this file.
  - `MCP_CACHE_TTL_MS` — referenced or defined in this file.
  - `deepResearchCache` — referenced or defined in this file.
  - `server` — referenced or defined in this file.
  - `cacheKey` — referenced or defined in this file.

---

## `src/output-manager.ts`  — 4.8 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** OutputManager, timestamp, metaStr, width, filled, terminalHeight, filename

- **Top comment / preview:**

```
Initialize terminal
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `OutputManager` — referenced or defined in this file.
  - `timestamp` — referenced or defined in this file.
  - `metaStr` — referenced or defined in this file.
  - `width` — referenced or defined in this file.
  - `filled` — referenced or defined in this file.
  - `terminalHeight` — referenced or defined in this file.

---

## `src/progress-manager.ts`  — 7.5 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** ProgressManager, ESC, CLEAR_LINE, CURSOR_TO_LINE, CURSOR_UP, CURSOR_DOWN, DEFAULT_NUMBER_OF_PROGRESS_LINES, width, percent, filled, empty, colorize, bar, pctStr, compact, labelStr, now, first, lastIndex, last, dCompleted, dTimeSec, rate, remaining, etaSec, mm, ss, progressStartLine, depthPct, breadthPct, queriesPct, overall

- **Top comment / preview:**

```
Constants for ANSI escape codes to improve readability
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `ProgressManager` — referenced or defined in this file.
  - `ESC` — referenced or defined in this file.
  - `CLEAR_LINE` — referenced or defined in this file.
  - `CURSOR_TO_LINE` — referenced or defined in this file.
  - `CURSOR_UP` — referenced or defined in this file.
  - `CURSOR_DOWN` — referenced or defined in this file.

---

## `src/prompt.ts`  — 5.8 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** promptCache, systemPrompt, now, hour, researchPhase, instructions, responseFormat, timeContext, serpQueryPromptTemplate, learningPromptTemplate, feedbackPromptTemplate, generateGeminiPrompt, clearPromptCache, validatePromptConsistency, templates, versions, content

- **Top comment / preview:**

```
Simplified cache config (v11 compatible)
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `promptCache` — referenced or defined in this file.
  - `systemPrompt` — referenced or defined in this file.
  - `now` — referenced or defined in this file.
  - `hour` — referenced or defined in this file.
  - `researchPhase` — referenced or defined in this file.
  - `instructions` — referenced or defined in this file.

---

## `src/run.ts`  — 5.1 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** log, askQuestion, run, output, rl, breadthInput, depthInput, feedbackResult, followUpQuestions, answer, combinedQuery, report, reportFilename, is

- **Top comment / preview:**

```
Helper function for consistent logging
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `log` — referenced or defined in this file.
  - `askQuestion` — referenced or defined in this file.
  - `run` — referenced or defined in this file.
  - `output` — referenced or defined in this file.
  - `rl` — referenced or defined in this file.
  - `breadthInput` — referenced or defined in this file.

---

## `src/search/providers.ts`  — 1.4 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** makeExaProviderIfAvailable, ExaProvider, res, results, exa, SearchProvider, SearchHit

- **Top comment / preview:**

```
Exa-only provider module. Firecrawl remains in `src/deep-research.ts`.
Grounding is handled by Gemini configuration in `src/ai/providers.ts`.
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `makeExaProviderIfAvailable` — referenced or defined in this file.
  - `ExaProvider` — referenced or defined in this file.
  - `res` — referenced or defined in this file.
  - `results` — referenced or defined in this file.
  - `exa` — referenced or defined in this file.
  - `SearchProvider` — referenced or defined in this file.

---

## `src/terminal-utils.ts`  — 1.0 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** generateProgressBar, getTerminalDimensions, TERMINAL_CONTROLS, filled, percentage, ProgressBarParams

- **Top comment / preview:**

```
New shared utilities file
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `generateProgressBar` — referenced or defined in this file.
  - `getTerminalDimensions` — referenced or defined in this file.
  - `TERMINAL_CONTROLS` — referenced or defined in this file.
  - `filled` — referenced or defined in this file.
  - `percentage` — referenced or defined in this file.
  - `ProgressBarParams` — referenced or defined in this file.

---

## `src/types.ts`  — 4.1 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** SerpQueriesJsonSchema, OutlineJsonSchema, SectionsJsonSchema, SummaryJsonSchema, TitleJsonSchema, FeedbackResponseJsonSchema, OutlineSchema, SectionsSchema, SummarySchema, ResearchResult, MCPResearchResult, Chunk, SerpQuery, Report, GatherOutput, AnalyzeOutput, SynthesizeOutput, SuperviseVerdict, FullResearchResult, EmbeddingsProvider, LlmJsonClient, EmbeddingVector, Citation, Outline, SectionsJSON, SummaryJSON

- **Top comment / preview:**

```
===========================
JSON Schema (plain objects) for Gemini responses
===========================
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `SerpQueriesJsonSchema` — referenced or defined in this file.
  - `OutlineJsonSchema` — referenced or defined in this file.
  - `SectionsJsonSchema` — referenced or defined in this file.
  - `SummaryJsonSchema` — referenced or defined in this file.
  - `TitleJsonSchema` — referenced or defined in this file.
  - `FeedbackResponseJsonSchema` — referenced or defined in this file.

---

## `src/utils/json.ts`  — 1.8 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** extractJsonFromText, isValidJSON, safeParseJSON, stringifyJSON, jsonRegex, match, jsonString

- **Top comment / preview:**

```
Regex to extract JSON object (non-greedy match)
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `extractJsonFromText` — referenced or defined in this file.
  - `isValidJSON` — referenced or defined in this file.
  - `safeParseJSON` — referenced or defined in this file.
  - `stringifyJSON` — referenced or defined in this file.
  - `jsonRegex` — referenced or defined in this file.
  - `match` — referenced or defined in this file.

---

## `src/utils/sanitize.ts`  — 0.2 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** sanitizeReportContent

- **Top comment / preview:**

```
export function sanitizeReportContent(content: string): string {
  return content
    .replace(/Thinking process:.*?\n\n/gs, '')
    .replace(/Outline:.*?\n\n/gs, '')
    .replace(/Step \d+:.*?\n/g, '')
    .replace(/\[Internal Note:.*?\]/g, '');
```

- **Heuristic summary:** Source code for main application (could be shared code or library).

- **Likely responsibilities:**

  - `sanitizeReportContent` — referenced or defined in this file.

---

## `tsconfig.json`  — 0.8 KB

- **Text file:** Yes

- **Detected symbols/functions/classes:** None detected

- **Top comment / preview:**

```
{
  "$schema": "https://json.schemastore.org/tsconfig",
  "compilerOptions": {
    "declaration": true,
    "declarationMap": true,
    "esModuleInterop": true,
```

- **Heuristic summary:** Auxiliary file or asset.


---
