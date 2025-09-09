# AI Stock Picker Agent 📈🤖

An advanced, multi-agent AI system built with CrewAI to automate stock market research and investment recommendations. This crew identifies trending companies, conducts deep financial analysis, and selects the most promising investment opportunity based on current news and data. It features sophisticated memory systems to track picks over time and avoid duplicate recommendations.

## Overview

This application automates a professional stock research workflow:
1.  **Trend Finder:** Scours the latest news to identify 2-3 currently trending companies in a specified sector using web search tools.
2.  **Financial Researcher:** Performs a comprehensive analysis on each trending company to build a detailed report.
3.  **Stock Picker:** Synthesizes the research to select the single best investment opportunity, provides a detailed rationale, and can send a push notification.
4.  **Manager:** Orchestrates the entire hierarchical process, ensuring tasks are delegated correctly and efficiently.

It's designed for investors, analysts, and fintech enthusiasts who want to leverage AI to augment their market research.

## Features

- **Multi-Agent Workflow:** Specialized AI agents work in sequence, each with a distinct role (finding, researching, picking, managing).
- **Sector-Focused Analysis:** Provides targeted research on user-specified market sectors (e.g., `Technology`, `Healthcare`, `Energy`).
- **Advanced Memory Systems:** Uses Short-Term, Long-Term, and Entity Memory to avoid recommending the same company twice, ensuring fresh insights.
- **Structured Outputs:** Uses Pydantic models to save structured results (trending list, research report) in JSON format.
- **External Tools:** Integrates with `SerperDevTool` for web search and a custom `PushNotificationTool`.
- **CrewAI Framework:** Leverages the powerful CrewAI framework for hierarchical agent orchestration and task management.
