# AI Agent: Gmail-to-LinkedIn Content Pipeline

## Executive Summary
This agent automates the extraction of insights from incoming emails, processes them using LLMs, and prepares social media drafts. It eliminates 5+ hours of manual drafting per week.

## The Stack
* *Orchestration:* Make.com
* *Intelligence:* Llama 3 via Groq (Low-latency inference)
* *Trigger:* Gmail API
* *Storage:* Notion (Content Calendar)

## Logic Flow
1. *Watch:* Monitors Gmail for specific labels/keywords.
2. *Filter:* Extracts body text and cleans HTML.
3. *Transform:* Groq rewrites the core insight into a LinkedIn-optimized post.
4. *Load:* Appends the draft to a Notion database for final review.
