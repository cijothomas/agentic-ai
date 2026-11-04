---
theme: default
title: Introduction to Agentic AI
info: KAW Agentic AI course contents
layout: default
class: course cover
transition: slide-left
colorSchema: light
aspectRatio: 16/9
canvasWidth: 1200
fonts:
  sans: Arial
  mono: monospace
  provider: none
drawings:
  persist: false
defaults:
  layout: default
  class: course
---

# Introduction to Agentic AI

<div class="subtitle">Course Overview & Foundations</div>

Welcome to the overview of Agentic AI.

---

# Course Syllabus & Logistics

<div class="subtitle">Learning Goals and Expectations</div>

<div class="columns three cards">
<div>

### Goal

Provide a high-level, less technical overview of agentic AI concepts.

</div>
<div>

### Topics Covered

- Foundations of AI & LLMs
- Prompts & Context
- Passive vs. Active AI Agents
- Tools & RAG
- Search Mechanisms
- Agent Standards / Protocols
- Frameworks & Architectures

</div>
<div>

### Expectation

Understand the core concepts and how they fit together in the modern AI landscape.

</div>
</div>

---

# Foundations of AI

<div class="subtitle">Machine Learning vs. Traditional Programming</div>

<div class="columns two compact">
<div>

### TRADITIONAL PROGRAMMING

A programmer figures out all the rules to achieve a task (e.g., writing explicit step-by-step instructions for a recipe).

</div>
<div>

### MACHINE LEARNING (ML)

A system that “Learns from Examples”. The ML system learns the rules by observing patterns in data (e.g., learning cooking patterns by observing thousands of recipes).

</div>
</div>

<img class="recipe-diagram" src="/images/programming-vs-ml.png" alt="Comparison of explicit cooking instructions and learning cooking patterns from examples" />

---

# Large Language Models (LLMs)

<div class="subtitle">Principles and Model Training</div>

<div class="columns four cards">
<div>

### What They Are

Powerful Machine Learning models specialized in language tasks.

They understand the context and underlying meaning of words (tokens) and sentences.

</div>
<div>

### Training

Trained on enormous amounts of text data, including books, articles, and Wikipedia.

Designed to recognize complex language patterns and efficiently “guess the next word”.

</div>
<div>

### Cost

Creating an LLM costs millions ($10M to $100M+).

Driven primarily by high computational resource demands and GPU availability needed for training.

</div>
<div>

### Capabilities

Versatile intelligence capable of answering complex questions.

Can autonomously write cohesive text, generate creative content, and build computer code.

</div>
</div>

---

# Prompts and Context

<div class="subtitle">Guiding Model Reasoning and Behavior</div>

<div class="columns illustrated">
<div>

### Context

Background information, past chat history, or specific instructions given to the AI model so it understands current requests.

### Prompts

Providing relevant information before asking a question to guide the model's interpretation.

### Examples

- **One Shot Learning:** Showing one example before the question.
- **Many Shot Learning:** Showing multiple examples.

<div class="callout">

### Key Benefit

The simplest and cheapest method for customizing LLM responses without retraining.

</div>
</div>
<div class="image-column">
<img src="/images/prompts-and-context.jpg" alt="Structured prompts and context data feeding an AI model" />
</div>
</div>

---

# What is an AI Agent?

<div class="subtitle">Transitioning from Passive LLMs to Active Systems</div>

<div class="columns illustrated">
<div>
<div class="columns two cards short">
<div>

### Passive AI

AI models by themselves can answer questions but cannot take actions on their own.

</div>
<div>

### Active Agents

Software that uses smart AI models to automate tasks.

</div>
</div>
<div class="callout agent-steps">

### How It Works

1. Agents can actively perform tasks on computers.
2. Agents give the AI model a list of tools or actions it is allowed to use.
3. The AI model decides which action to take and asks the agent to run it.

</div>
</div>
<div class="diagram-panel">

### Agent Architecture Loop

<img src="/images/agent-loop.png" alt="An agent asks the LLM and uses tools" />
</div>
</div>

---

# Equipping Agents with Tools

<div class="subtitle">Interacting with External Systems</div>

<div class="columns illustrated roomy">
<div>

### Tools

Special software add-ons (calculators, web search, database connections) that let an AI agent interact with the outside world.

### Purpose

Allows agents to get accurate, up-to-date facts or perform actions.

### Example

Instead of guessing a math problem, an agent sends the equation to a calculator tool for the exact answer.

</div>
<div class="image-column">
<img src="/images/agent-tools.jpg" alt="An AI agent connected to a calculator, web search, and a database" />
</div>
</div>

---

# Retrieval-Augmented Generation (RAG)

<div class="subtitle">Grounding AI in Knowledge</div>

<div class="columns three cards">
<div>

### Step 1

## Document Search

**RAG Technique:** The system looks up relevant facts in private files or domain documents first before generating output.

</div>
<div>

### Step 2

## Context Retrieval

**Goal:** Enables the AI model to construct an accurate, well-sourced answer based strictly on specific, provided information.

</div>
<div>

### Step 3

## Grounded Generation

**Example:** Searching a company handbook for a “vacation policy” and providing that text to the AI to construct a direct answer.

</div>
</div>

---

# Search & Retrieval Mechanisms

<div class="subtitle">Embeddings, Vector DBs, and Hybrid Search</div>

<div class="columns two quadrants">
<div>

### Sentence Embeddings

Converting text into lists of numbers (vectors) representing core meaning, allowing systems to find phrases with similar meanings.

</div>
<div>

### Vector DB

A database built to find information based on similar concepts rather than exact word matches.

</div>
<div>

### Inverted Index

A traditional search index mapping specific keywords directly to exact pages.

</div>
<div>

### Hybrid Search

Combining meaning-based search (vector) with exact keyword search (inverted index) for optimal accuracy.

</div>
</div>

---

# Agent Standards & Protocols

<div class="subtitle">MCP, A2A, A2UI, and AGENTS.md</div>

<p class="protocol-intro"><strong>Protocols:</strong> Shared standards enabling different AI systems to communicate smoothly.</p>

<div class="columns four cards protocols">
<div>

## MCP

### Model Context Protocol

A universal connector standard for plugging AI models into external tools.

</div>
<div>

## A2A

### Agent-to-Agent

Rules letting different AI agents talk, hand off tasks, and collaborate.

</div>
<div>

## A2UI

### Agent-to-User Interface

An open standard for agents to automatically build and display interactive visuals (buttons, forms).

</div>
<div>

## AGENTS.md

### Codebase Rules

A rule file giving coding agents specific instructions and boundaries within a codebase.

</div>
</div>

---

# Frameworks & Developer Toolkits

<div class="subtitle">LangChain, ADK, and Lightweight Kits</div>

<div class="columns three cards">
<div>

### LANGCHAIN

A widely-used toolset helping developers connect AI models to external data sources, prompts, and tools in structured steps.

</div>
<div>

### ADK (AGENT DEVELOPMENT KIT)

Google's toolkit for creating, testing, and running production-ready multi-agent systems.

</div>
<div>

### PI (LIGHTWEIGHT KITS)

Minimal toolkits designed to build small, fast, highly focused AI agents with few dependencies.

</div>
</div>

---

# Advanced Agent Architecture

<div class="subtitle">Sub-Agents, Memory, and Context Compaction</div>

<div class="columns two quadrants">
<div>

### Sub-agents

Helper agents spawned by a main AI agent to handle small, focused tasks separately.

</div>
<div>

### Memory

How an agent retains short-term facts for the immediate conversation and long-term knowledge across interactions.

</div>
<div>

### Context Compaction

Cleaning up or summarizing long chat histories so the AI stays focused and within memory limits.

</div>
<div>

### Prompt Caching

Saving and reusing initial instructions so the AI doesn't re-process identical content, saving time and money.

</div>
</div>
