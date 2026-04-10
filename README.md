# AI Career & Learning Assistant

An agentic AI integration for resume tracking, technical skill assessment, communication skill development, and personalized learning roadmap generation.

## 🚀 Overview

This project integrates an intelligent AI assistant into an existing resume and skill-tracking website. The assistant helps users:

- Practice vocabulary through dynamic MCQ generation
- Analyze overall performance across technical and communication skills
- Generate personalized learning roadmaps
- Discover domain-relevant courses and resources

## ✨ Features

### 1. Vocabulary MCQs
- Generates context-aware multiple-choice questions based on user's specialization
- Each question includes 4 options, correct answer, and explanation
- JSON output format for easy integration

### 2. Overall Performance Analysis
- Aggregates data from:
  - Technical marks (programming languages, tech skills)
  - Online judge performance (LeetCode, Wager, Codilo)
  - Vocabulary chapter-wise marks
  - Mock interview scores
- Provides strengths, weaknesses, and trend analysis
- Actionable insights for improvement

### 3. Personalized Roadmap Generation
- Creates step-by-step learning paths based on:
  - User's specialization
  - Current skill levels
  - Career goals
- Includes:
  - Foundational topics to revise
  - Priority-ordered new topics
  - Practice milestones (problems/week)
  - Mock interview frequency
  - Estimated completion timeline

### 4. Domain-Specific Resource Recommendations
- Suggests 5-7 high-quality resources per domain
- Platforms: Coursera, YouTube, documentation, books
- Includes difficulty level, time estimate, and relevance explanation

## 🛠️ Tech Stack

- **Orchestration**: n8n (workflow automation)
- **AI Model**: OpenAI / Anthropic / Ollama (LLM of choice)
- **Data Sources**: 
  - Resume database
  - Skill tracking system
  - Online judge APIs (LeetCode, Wager, Codilo)
  - Mock interview records
- **Output Formats**: JSON (MCQs), Markdown (analysis & roadmaps)

## 📋 Prerequisites

- n8n instance (self-hosted or cloud)
- API key for your chosen LLM provider
- Access to user database with schema containing:
  - Resume fields (name, specialization, projects, internships, certifications, languages)
  - Technical skills (programming languages, Coursera courses, marks, LeetCode stats)
  - Communication skills (vocabulary marks, mock interview scores)

## 🔧 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/ai-career-assistant.git
cd ai-career-assistant
