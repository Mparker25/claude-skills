# Domain Expert Agents Guide

> **Complete guide to the 10 domain expert agents** in the Claude Startup Starter Kit

## What are Domain Agents?

Domain expert agents are AI specialists that coordinate multiple skills within their area of expertise. Instead of manually selecting and sequencing individual skills, you work with agents who intelligently choose the right tools and workflows for your goals.

**Think of agents as hiring an executive team:**
- @marketing-strategist = Chief Marketing Officer
- @executive-advisor = CEO + CTO Board Advisors
- @product-lead = Head of Product
- @design-director = Head of Design
- @delivery-manager = VP of Delivery
- @engineering-lead = VP of Engineering
- @data-science-lead = Head of AI/ML/Data
- @regulatory-director = Head of Regulatory Affairs
- @quality-director = Head of Quality
- @compliance-officer = Chief Compliance Officer

## Why Use Agents Instead of Individual Skills?

### Traditional Approach (Manual)
```bash
# You need to:
1. Know which skills exist
2. Understand which skill does what
3. Manually select the right skill
4. Chain multiple skills together
5. Coordinate the workflow yourself
```

### Agent Approach (Intelligent)
```bash
# Agent handles everything:
@marketing-strategist launch our new SaaS product

→ Agent automatically:
  - Chooses product marketing for positioning
  - Uses content creator for launch content
  - Applies demand generation for campaigns
  - Coordinates all workflows intelligently
```

**Result:** You get expert coordination without needing to know the implementation details.

---

## The 10 Domain Expert Agents

### 1. Marketing Strategist (@marketing-strategist)

**Role:** Chief Marketing Officer for your startup

**Coordinates:**
- content-creator (SEO, brand voice, content frameworks)
- marketing-demand-acquisition (paid campaigns, lead gen, CAC optimization)
- marketing-strategy-pmm (product marketing, GTM strategy)

**When to Use:**
- Product launches and go-to-market planning
- Content strategy and editorial calendars
- Demand generation and paid campaigns
- Brand voice analysis and consistency
- SEO optimization across content

**Example Requests:**
```bash
# Product launch
@marketing-strategist launch our new AI analytics platform targeting enterprise customers

# Content strategy
@marketing-strategist build a Q1 2025 content strategy for our blog focusing on developer tutorials

# Demand generation
@marketing-strategist setup paid campaigns with $50k monthly budget targeting B2B SaaS buyers

# Brand voice
@marketing-strategist analyze our website copy for brand voice consistency
```

**What the Agent Does:**
1. Analyzes your request and determines strategy
2. Selects appropriate marketing skills
3. Uses brand_voice_analyzer.py for consistency checks
4. Uses seo_optimizer.py for content optimization
5. Uses cac_calculator.py for campaign planning
6. Coordinates multi-skill workflows automatically

**Python Tools:** `brand_voice_analyzer.py`, `seo_optimizer.py`, `cac_calculator.py`

---

### 2. Executive Advisor (@executive-advisor)

**Role:** Combined CEO and CTO strategic advisory board

**Coordinates:**
- ceo-advisor (strategy, business planning, fundraising)
- cto-advisor (technical architecture, team scaling)

**When to Use:**
- Strategic planning and OKR setting
- Major technical architecture decisions
- Team scaling and organization design
- Fundraising and investor relations
- Build vs buy decisions

**Example Requests:**
```bash
# Strategic planning
@executive-advisor set company OKRs for Q2 2025 given our Series A goals

# Technical decisions
@executive-advisor should we use microservices or monolith for our current stage?

# Team scaling
@executive-advisor plan hiring roadmap to scale from 10 to 30 engineers

# Board prep
@executive-advisor prepare board presentation for Q4 results
```

**What the Agent Does:**
1. Provides dual business + technical perspective
2. Uses strategy_analyzer.py for scenario planning
3. Uses financial_scenario_modeler.py for projections
4. Uses tech_debt_analyzer.py for technical assessment
5. Uses team_scaling_calculator.py for hiring plans
6. Delivers board-level recommendations

**Python Tools:** `strategy_analyzer.py`, `financial_scenario_modeler.py`, `tech_debt_analyzer.py`, `team_scaling_calculator.py`

---

### 3. Product Lead (@product-lead)

**Role:** Head of Product for your startup

**Coordinates:**
- product-manager-toolkit (RICE prioritization, customer interviews)
- agile-product-owner (user stories, sprint planning)
- product-strategist (OKRs, roadmapping)

**When to Use:**
- Feature prioritization and roadmapping
- Customer research and interview analysis
- Sprint planning and backlog management
- OKR cascade from company to product level
- PRD (Product Requirements Document) creation

**Example Requests:**
```bash
# Prioritization
@product-lead prioritize our backlog of 50 features using RICE framework for Q2

# Customer research
@product-lead analyze these 20 customer interview transcripts and extract pain points

# Sprint planning
@product-lead plan next 2-week sprint with 30 story points capacity

# OKRs
@product-lead create product OKRs aligned with company goal of 10x revenue growth
```

**What the Agent Does:**
1. Uses rice_prioritizer.py for quantitative prioritization
2. Uses customer_interview_analyzer.py for research insights
3. Uses user_story_generator.py for INVEST-compliant stories
4. Uses okr_cascade_generator.py for strategic alignment
5. Coordinates entire product development lifecycle

**Python Tools:** `rice_prioritizer.py`, `customer_interview_analyzer.py`, `user_story_generator.py`, `okr_cascade_generator.py`

---

### 4. Design Director (@design-director)

**Role:** Head of Design (UX + UI)

**Coordinates:**
- ux-researcher-designer (user research, personas, journey mapping)
- ui-design-system (design tokens, component libraries)

**When to Use:**
- User research and persona generation
- Design system creation from scratch
- Design token generation and export
- User journey mapping
- Usability testing planning

**Example Requests:**
```bash
# Design system
@design-director create a complete design system from our brand color #0066CC

# User research
@design-director generate user personas from our 30 user interviews

# Design tokens
@design-director export design tokens as CSS variables for our React app

# Journey mapping
@design-director map user journey for our onboarding flow
```

**What the Agent Does:**
1. Uses persona_generator.py for data-driven personas
2. Uses design_token_generator.py for complete token systems
3. Generates colors, typography, spacing, shadows
4. Exports in CSS, JSON, or SCSS formats
5. Creates responsive component libraries

**Python Tools:** `persona_generator.py`, `design_token_generator.py`

---

### 5. Delivery Manager (@delivery-manager)

**Role:** VP of Delivery (Project Management + Agile)

**Coordinates:**
- senior-pm (project planning, risk management)
- scrum-master (sprint facilitation, agile ceremonies)
- jira-expert (Jira administration and optimization)
- confluence-expert (documentation strategy)
- atlassian-admin (Atlassian suite management)
- atlassian-templates (ready-to-use templates)

**When to Use:**
- Sprint planning and retrospectives
- Jira workflow configuration
- Confluence documentation structure
- Agile transformation and coaching
- Project reporting and dashboards

**Example Requests:**
```bash
# Sprint setup
@delivery-manager setup new sprint in Jira with 2-week timeline

# Agile transformation
@delivery-manager implement Scrum framework for our 15-person engineering team

# Documentation
@delivery-manager create Confluence space structure for product documentation

# Reporting
@delivery-manager create executive dashboard in Jira for velocity tracking
```

**What the Agent Does:**
1. Configures Jira projects and workflows
2. Sets up Confluence spaces and templates
3. Manages sprint planning and capacity
4. Facilitates agile ceremonies
5. **Uses Atlassian MCP Server** for direct Jira/Confluence operations

**Python Tools:** None (uses Atlassian MCP Server integration)

---

### 6. Engineering Lead (@engineering-lead)

**Role:** VP of Engineering

**Coordinates:**
- senior-architect (system design, architecture patterns)
- senior-frontend (React, Next.js, TypeScript)
- senior-backend (Node.js, APIs, databases)
- senior-fullstack (complete stack, project scaffolding)
- senior-qa (test automation, quality assurance)
- senior-devops (CI/CD, Docker, Kubernetes)
- senior-secops (security operations)
- code-reviewer (code review best practices)
- senior-security (application security, pentesting)

**When to Use:**
- System architecture design and review
- Full-stack application development
- CI/CD pipeline setup
- Code quality and security audits
- Infrastructure as code
- Pull request reviews

**Example Requests:**
```bash
# Architecture review
@engineering-lead review our microservices architecture for scalability

# Project setup
@engineering-lead scaffold a new Next.js + GraphQL + PostgreSQL project

# Code quality
@engineering-lead analyze code quality and security vulnerabilities in our codebase

# CI/CD
@engineering-lead setup CI/CD pipeline with GitHub Actions and Docker
```

**What the Agent Does:**
1. Uses project_scaffolder.py for rapid project setup
2. Uses code_quality_analyzer.py for comprehensive analysis
3. Uses fullstack_scaffolder.py for boilerplate generation
4. Uses pr_analyzer.py for automated code review
5. Coordinates all engineering disciplines

**Python Tools:** `project_scaffolder.py`, `code_quality_analyzer.py`, `fullstack_scaffolder.py`, `pr_analyzer.py`

---

### 7. Data Science Lead (@data-science-lead)

**Role:** Head of AI/ML/Data

**Coordinates:**
- senior-data-scientist (statistical analysis, experiments, feature engineering)
- senior-data-engineer (data pipelines, ETL, data quality)
- senior-ml-engineer (model deployment, MLOps)
- senior-prompt-engineer (LLM optimization, RAG systems)
- senior-computer-vision (object detection, image/video AI)

**When to Use:**
- A/B test design and analysis
- Data pipeline orchestration
- ML model deployment to production
- LLM prompt optimization
- RAG system development
- Computer vision model training

**Example Requests:**
```bash
# ML pipeline
@data-science-lead build ML model deployment pipeline with monitoring

# RAG system
@data-science-lead build RAG system for our documentation using LangChain

# A/B testing
@data-science-lead design A/B test for new checkout flow with statistical rigor

# Computer vision
@data-science-lead train object detection model for product images
```

**What the Agent Does:**
1. Coordinates 15 Python tools across 5 disciplines
2. Data science: experiment_designer.py, feature_engineering_pipeline.py, statistical_analyzer.py
3. Data engineering: pipeline_orchestrator.py, data_quality_validator.py, etl_generator.py
4. ML engineering: model_deployment_pipeline.py, mlops_setup_tool.py, llm_integration_builder.py
5. Prompt engineering: prompt_optimizer.py, rag_system_builder.py, agent_orchestrator.py
6. Computer vision: vision_model_trainer.py, inference_optimizer.py, video_processor.py

**Python Tools:** 15 specialized tools across data/ML/AI domains

---

### 8. Regulatory Director (@regulatory-director)

**Role:** Head of Regulatory Affairs (HealthTech/MedTech)

**Coordinates:**
- regulatory-affairs-head (regulatory strategy, market access)
- mdr-745-specialist (EU MDR 2017/745 compliance)
- fda-consultant-specialist (FDA 510(k), PMA, QSR)
- risk-management-specialist (ISO 14971 risk management)

**When to Use:**
- EU MDR certification preparation
- FDA regulatory submissions
- Risk management file creation (ISO 14971)
- Post-market surveillance
- Technical file compilation
- Regulatory pathway selection

**Example Requests:**
```bash
# MDR compliance
@regulatory-director prepare EU MDR certification for our Class IIb device

# FDA submission
@regulatory-director prepare 510(k) submission package for Class II device

# Risk management
@regulatory-director conduct ISO 14971 risk analysis for new feature

# Pathway selection
@regulatory-director recommend optimal regulatory pathway for US and EU markets
```

**What the Agent Does:**
1. Expert in EU MDR 2017/745 and FDA regulations
2. Uses regulatory_pathway_analyzer.py for strategy
3. Uses submission_timeline_tracker.py for planning
4. Uses risk_analysis_tool.py for ISO 14971 compliance
5. Coordinates all regulatory activities

**Python Tools:** `regulatory_pathway_analyzer.py`, `submission_timeline_tracker.py`, `risk_analysis_tool.py`

---

### 9. Quality Director (@quality-director)

**Role:** Head of Quality (QMS + ISMS)

**Coordinates:**
- quality-manager-qmr (QMR role, management reviews)
- quality-manager-qms-iso13485 (ISO 13485 QMS)
- capa-officer (corrective and preventive actions)
- quality-documentation-manager (document control)
- information-security-manager-iso27001 (ISO 27001 ISMS)

**When to Use:**
- ISO 13485 QMS implementation
- ISO 27001 ISMS implementation
- CAPA investigation and management
- Management review preparation
- Document control systems
- Internal audit planning

**Example Requests:**
```bash
# QMS setup
@quality-director setup ISO 13485 quality management system from scratch

# CAPA management
@quality-director investigate nonconformance from external audit

# ISMS setup
@quality-director implement ISO 27001 information security management system

# Document control
@quality-director design document control system for regulated environment
```

**What the Agent Does:**
1. Uses qms_effectiveness_monitor.py for performance tracking
2. Uses capa_tracker.py for CAPA lifecycle management
3. Uses document_version_controller.py for document control
4. Expert in ISO 13485 and ISO 27001 standards
5. Coordinates quality and security management

**Python Tools:** `qms_effectiveness_monitor.py`, `capa_tracker.py`, `document_version_controller.py`

---

### 10. Compliance Officer (@compliance-officer)

**Role:** Chief Compliance Officer (Audits + GDPR)

**Coordinates:**
- qms-audit-expert (ISO 13485 internal audits)
- isms-audit-expert (ISO 27001 security audits)
- gdpr-dsgvo-expert (GDPR/DSGVO data protection)

**When to Use:**
- Internal QMS audits
- Internal ISMS audits
- External audit preparation
- GDPR compliance assessment
- Data protection impact assessments (DPIA)
- Audit finding management

**Example Requests:**
```bash
# QMS audit
@compliance-officer conduct internal audit of our design control process

# ISMS audit
@compliance-officer audit information security controls

# GDPR compliance
@compliance-officer assess GDPR compliance for our SaaS product

# DPIA
@compliance-officer generate data protection impact assessment for new feature
```

**What the Agent Does:**
1. Uses gdpr_compliance_checker.py for GDPR assessment
2. Uses dpia_generator.py for privacy impact analysis
3. Uses audit_checklist_generator.py for systematic audits
4. Expert in ISO 13485, ISO 27001, and GDPR
5. Manages complete audit lifecycle

**Python Tools:** `gdpr_compliance_checker.py`, `dpia_generator.py`, `audit_checklist_generator.py`

---

## Agent Architecture

### How Agents Work

1. **Context Understanding**: Agent reads your request and determines intent
2. **Skill Selection**: Agent chooses which skills to use
3. **Tool Execution**: Agent runs Python automation tools
4. **Workflow Coordination**: Agent sequences multiple skills if needed
5. **Result Delivery**: Agent provides comprehensive output

### Agent Specifications

All agents follow the Anthropic subagent specification:

```yaml
---
name: agent-name
description: What the agent does and when to invoke it
tools: Read, Write, Edit, Bash, Grep, Glob
model: sonnet
---
```

**Key Properties:**
- **Manual Invocation**: Agents require explicit `@agent-name` call
- **Tool Access**: All agents have file system access (Read, Write, Edit, Bash, Grep, Glob)
- **Model**: All agents use Claude Sonnet for reliability and speed
- **Stateless**: Each agent invocation is independent

### Agent vs Skill

**Agent:**
- High-level coordinator
- Understands business context
- Makes strategic decisions
- Chooses and sequences skills
- Provides expert guidance

**Skill:**
- Specific implementation
- Focused on execution
- Contains Python tools
- Contains knowledge bases
- Contains templates

**Example:**
```
User: "@marketing-strategist launch our product"

Agent thinks:
1. This needs product positioning → use product marketing skill
2. This needs launch content → use content creator skill
3. This needs distribution → use demand generation skill

Agent executes:
1. Calls product-marketing skill for positioning
2. Calls content-creator skill with seo_optimizer.py
3. Calls demand-acquisition skill with cac_calculator.py

Result: Complete product launch strategy
```

---

## Best Practices

### DO ✅

**Be Specific About Your Goal**
```bash
# Good
@marketing-strategist launch our new AI analytics SaaS targeting enterprise customers in Q1 2025

# Avoid
@marketing-strategist help with marketing
```

**Provide Context**
```bash
# Good
@product-lead prioritize Q2 roadmap with 30 person-weeks capacity, focus on revenue growth

# Avoid
@product-lead prioritize features
```

**Trust Agent Expertise**
```bash
# Good
@engineering-lead review our architecture for scalability concerns

# Avoid
@engineering-lead use the senior-architect skill to review architecture using these specific patterns...
```

**Let Agents Coordinate**
```bash
# Good (single agent coordinates everything)
@marketing-strategist launch our product with content, ads, and SEO

# Avoid (manual coordination)
Use content-creator for blog, then marketing-demand for ads, then...
```

### DON'T ❌

**Don't Micromanage Agents**
- Let agents choose which skills to use
- Agents know their toolkit better than you
- Focus on WHAT you want, not HOW

**Don't Mix Multiple Agents**
```bash
# Avoid
@marketing-strategist and @product-lead work together on launch

# Do instead
@marketing-strategist launch our product (agent coordinates with product knowledge)
```

**Don't Forget Constraints**
```bash
# Avoid
@executive-advisor plan team scaling

# Do instead
@executive-advisor plan team scaling with $2M budget over 6 months
```

---

## Quick Reference

| Agent | Best For | Key Tools |
|-------|----------|-----------|
| @marketing-strategist | Product launches, content, campaigns | brand_voice_analyzer, seo_optimizer, cac_calculator |
| @executive-advisor | Strategic planning, architecture decisions | strategy_analyzer, financial_modeler, tech_debt_analyzer |
| @product-lead | Roadmaps, prioritization, sprint planning | rice_prioritizer, customer_analyzer, story_generator |
| @design-director | Design systems, user research | persona_generator, design_token_generator |
| @delivery-manager | Sprints, Jira, Confluence, agile | Atlassian MCP Server |
| @engineering-lead | Architecture, code quality, CI/CD | project_scaffolder, code_analyzer, pr_analyzer |
| @data-science-lead | ML pipelines, RAG systems, A/B tests | 15 AI/ML/Data tools |
| @regulatory-director | MDR, FDA, risk management | regulatory_analyzer, submission_tracker |
| @quality-director | ISO 13485, ISO 27001, CAPA | qms_monitor, capa_tracker, document_controller |
| @compliance-officer | Audits, GDPR, compliance | gdpr_checker, dpia_generator, audit_checklist |

---

## Getting Started

### 1. Install a Domain Toolkit

```bash
/plugin marketplace add Mparker25/claude-skills
/plugin install marketing@mparker-claude-skills
```

### 2. Invoke the Agent

```bash
@marketing-strategist launch our new SaaS product
```

### 3. Provide Context

The more context you provide, the better the agent can help:
- Your company stage (pre-seed, seed, Series A, etc.)
- Your constraints (budget, timeline, team size)
- Your goals (revenue, users, market share)
- Your audience (B2B, B2C, enterprise, SMB)

### 4. Review and Iterate

Agents provide comprehensive output. Review and ask follow-up questions:
```bash
@marketing-strategist that looks good, now create the Q1 content calendar
```

---

## Support

For questions, issues, or feature requests:
- **GitHub Issues**: https://github.com/Mparker25/claude-skills/issues
- **Documentation**: See README.md and MARKETPLACE.md
- **Individual Skills**: See SKILL.md files in each skill directory

## License

MIT License - See LICENSE file

## Maintainer

**Malik Bernard Parker**
- Email: Malik.Bernard.Parker@gmail.com
- GitHub: [@Mparker25](https://github.com/Mparker25)

---

**Ready to build with your AI executive team?** Install your first toolkit and start with an agent!

```bash
/plugin marketplace add Mparker25/claude-skills
/plugin install marketing@mparker-claude-skills
@marketing-strategist help me launch our product
```
