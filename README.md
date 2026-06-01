<img width="2752" height="1536" alt="Building_An_AI_Second_Brain" src="https://github.com/user-attachments/assets/d4eafceb-9a0b-4855-80cb-e0f3dbd5792e" />

# Build an AI Second Brain with Claude Code

**Project Link:** [View Project](http://learn.nextwork.org/projects/ai-second-brain-claude-code)

---

---

## Introducing Today's Project!

In this project, I'm going to build a second brain using Claude Code and Obsidian to run oof the Andre Kapathy methodology. I will be learning about wikis, indexing and different queries to create my wn personal knowledge base for an LLM.

### Key tools and concepts

Obsidian: A free note-taking app that uses plain Markdown files and provides a visual Graph View to see connections between ideas.

Claude Code: A command-line AI agent that can read, create, and edit files directly on your computer, acting as the "wiki maintainer."

Obsidian Web Clipper (Optional): A browser extension for saving web pages directly into the vault.

Concepts:

The Vault Architecture: The fundamental principle of separating a raw/ folder (your untouched source material) from a wiki/ folder (AI-compiled knowledge). This is called the "load-bearing rule" because keeping them separate ensures your original sources are never modified.

LLM Wiki Pattern: Andrej Karpathy's methodology of using an LLM as a "programmer" and Obsidian as the "IDE" for a knowledge base.

Schema-Driven Behavior: How a CLAUDE.md file acts as a constitution that the AI reads every session, defining project structure, page conventions.

Slash Commands as Primitives:

Knowledge Synthesis:

### Challenges and wins

The project is estimated to take 60 minutes. From the tutorial, you would have spent this time on:

Installing and setting up both Obsidian and Claude Code.

Scaffolding the raw/ and wiki/ vault architecture.

Defining your CLAUDE.md schema and slash commands.

Exporting your existing data from other apps and converting it to Markdown.

Running your first /ingest cycle and exploring the compiled wiki and Graph View.

### Why I did this project

I did this project today to learn how to build an AI Second Brain with Claude Code Another skill I want to learn is automating the ingest so I don't have to move files manually.

---

## Installing Obsidian and Claude Code

In this step, I'm installing Obsidian and creating our vault, and then I will install Claude code to then sort things out later on in the project.

![Image](http://learn.nextwork.org/radiant_blue_innocent_pawpaw/uploads/ai-second-brain-claude-code_qw9n3t5y)

### Verifying my Claude Code install

I installed Claude Code version 2.1.158 

---

## Building the Vault Architecture

In this step I am going to get Claude code to scaffold our vault's folder structure, and we will also be verifying the new folders appear in Obsidian. We are in particular going to pay attention to the raw and the wiki folders. 

![Image](http://learn.nextwork.org/radiant_blue_innocent_pawpaw/uploads/ai-second-brain-claude-code_v2b7n4p2)

### Inside the wiki/ folder

I counted 6 subfolders(well, it was actually four subfolders and two files). 

![Image](http://learn.nextwork.org/radiant_blue_innocent_pawpaw/uploads/ai-second-brain-claude-code_v2d1s6t4)

---

## Configuring CLAUDE.md and Slash Commands

In this step, I'm creating a CLAUDE.md file to load into context every single time that i open a claude session within this project, it will understand:
-the project structure
-the domain context
-the style guide
-the page conventions


![Image](http://learn.nextwork.org/radiant_blue_innocent_pawpaw/uploads/ai-second-brain-claude-code_v3n8q1w6)

### The four slash command workflows

The four sections in my CLAUDE.md are ingest, query, log, and lint. Each one insturcts claude to perform different operatioons that i will cover later on in this project. In the screenshot, we actually cant see our claude commands as they are in a hidden claude folder.

![Image](http://learn.nextwork.org/radiant_blue_innocent_pawpaw/uploads/ai-second-brain-claude-code_p6x2m9k4)

### Scaffolding the slash commands

 .claude/commands/ are real Claude Code slash commands: typing /ingest at the start of a message runs the file as a prompt, with $ARGUMENTS filled in from anything you type after the command. They tab-complete, they're shareable via Git, and they don't conflict with Claude Code's parser.

![Image](http://learn.nextwork.org/radiant_blue_innocent_pawpaw/uploads/ai-second-brain-claude-code_a9c4e7g1)

---

## Converting Source Notes Into the raw/ Folder

In this step, I'm going to what in my notes and conversations from different tools? Convert the JSON exports into markdown becuase thats's the only format that obsidian can read, and then we're going to verify files in Obsidian. 

![Image](http://learn.nextwork.org/radiant_blue_innocent_pawpaw/uploads/ai-second-brain-claude-code_k8n4y1q3)

### How many files Claude Code converted

I converted 42 conversations from Claude.ai. The script created 42 markdown files which were converted from JSON

### Checking the converted files in Obsidian

I verified that the converted files have YAML front matter. The frontmatter includes source, date, and topic.

---

## Running the First Ingest Cycle

In this step I am to create or run the /ingest command to process ourraw sources. I'm going to explore the wiki pages that claude code has complied, and i'll be able to view this all in my obsididan knowledge graph.

![Image](http://learn.nextwork.org/radiant_blue_innocent_pawpaw/uploads/ai-second-brain-claude-code_p3r8w5n1)

### The pages Claude Code created

After the ingest, index.md lists the different connections, concepts, and tags so that we can see how these ideas get linked to other ideas.

### Exploring a wiki page

I explored the page mobility page and it told me that i was focusing [[threat-modelling]], [[maestro-framework]], [[ai-agent-governance]], [[securing-ai-agents-data-governance]], [[risen-framework]], [[ics-security]], [[three-tier-web-architecture]],

![Image](http://learn.nextwork.org/radiant_blue_innocent_pawpaw/uploads/ai-second-brain-claude-code_k9g4z6c2)

---

## Querying and Verifying My Wiki

### How my wiki answered with cited sources

---

## Logging Daily Progress

---

## Secret Mission: Dogfooding /lint and /log

In this project extension, I'm going to test the /query/lint and /log slash commands.

![Image](http://learn.nextwork.org/radiant_blue_innocent_pawpaw/uploads/ai-second-brain-claude-code_b3h7k9r2)

### What /lint found and how Claude fixed it

In this project extension, /lint reported I asked Claude to fix The three inaccurate last-updated dates are trivial one-liners. The 17 broken links need a decision first: should Sources sections use plain text instead of [[]] syntax, or is [[raw-slug]] acceptable as a citation convention?

![Image](http://learn.nextwork.org/radiant_blue_innocent_pawpaw/uploads/ai-second-brain-claude-code_g2j8v5x1)

### Capturing a thought with /log

In this project extension, I captured a thought with /log about nothing No entity matches in the note. Claude also updated nothing as  No wiki pages touched — no entity matches found.

---

---
