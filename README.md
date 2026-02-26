Turning VS Code into a Local Agentic AI Assistant
Overview

This project explains how to convert Visual Studio Code into a powerful local AI coding assistant using:

Continue.dev extension

Ollama (running locally)

Multiple local AI models

The goal is simple:
Create a fully offline, intelligent development environment where AI can:

Explain your source code

Complete your code in real time

Search across your project intelligently

Help with debugging and understanding logic

All of this runs entirely on your local machine — no external APIs required.

We combine three key components:

1. VS Code

Your main development environment.

2. Continue.dev Extension

This extension brings an AI chat interface directly into VS Code and allows it to act like an agent.

3. Ollama

Ollama runs large language models (LLMs) locally on your machine.

The Three Models We Use

To make the AI effective, we use three different types of models — each with a specific responsibility.

1️⃣ Text Model (Main Chat Model)

This is the primary AI brain.

It helps with:

Explaining source code

Answering technical questions

Debugging issues

Reviewing code

Suggesting improvements

Whenever you ask something in chat, this model generates the response.

2️⃣ Auto-Completion Model

This model focuses on speed.

It helps with:

Completing functions

Writing boilerplate code

Suggesting inline code

Improving development speed

It runs lightweight and fast so that suggestions feel real-time.

3️⃣ Embedding Model

This model is responsible for understanding your entire project.

It:

Indexes your source code

Converts files into vector format

Enables semantic search

Helps the chat model retrieve relevant context

This is what makes the system “smart” about your project instead of giving generic answers.

Installation Steps
Step 1: Install VS Code

Install the latest version of VS Code.

Step 2: Install Continue.dev Extension

Open VS Code

Go to Extensions (Ctrl + Shift + X)

Search for Continue.dev

Install it

Step 3: Install Ollama

After installing Ollama, verify:

ollama --version