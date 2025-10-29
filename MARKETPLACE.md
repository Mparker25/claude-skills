# Claude Startup Starter Kit - Marketplace Guide

> **Complete AI-powered startup toolkit** with 10 domain expert agents coordinating 42 specialized skills and 97 automation tools.

This is a Claude Code plugin marketplace featuring **domain expert agents** that intelligently coordinate specialized skills across marketing, engineering, product, compliance, and leadership domains. Think of it as hiring an AI-powered executive team for your startup.

> **Fork Notice:** This is a professionally maintained fork of the [original Claude Skills Library](https://github.com/alirezarezvani/claude-skills) by Alireza Rezvani (MIT License). Enhanced and maintained by Malik Bernard Parker.

## Quick Start

### 1. Add the Marketplace

```bash
# Add via GitHub (recommended)
/plugin marketplace add Mparker25/claude-skills
```

### 2. Install Domain Toolkits

```bash
# Install specific toolkits (includes agent + skills)
/plugin install marketing@mparker-claude-skills
/plugin install core-engineering@mparker-claude-skills
/plugin install product-management@mparker-claude-skills
```

### 3. Use Your Domain Agents

```bash
# Invoke agents to coordinate complex workflows
@marketing-strategist launch our new SaaS product
@engineering-lead review our microservices architecture
@product-lead prioritize Q2 roadmap with RICE framework
```

**That's it!** Each plugin includes a domain expert agent that coordinates multiple skills automatically.

## Available Plugin Collections

### 1. Marketing Toolkit (3 skills + 1 agent)
**Install:** `/plugin install marketing@mparker-claude-skills`

Complete marketing toolkit with **Marketing Strategist agent** (`@marketing-strategist`) coordinating content creation, demand generation, and product marketing strategy.

**🤖 Domain Agent:**
- **@marketing-strategist**: CMO-level strategic coordination of all marketing activities

**📚 Included Skills:**
- **content-creator**: SEO-optimized content with brand voice analysis
- **marketing-demand-acquisition**: Lead generation and acquisition strategies
- **marketing-strategy-pmm**: Product marketing and go-to-market planning

**💡 Example Workflows:**
```bash
# Product launch (agent coordinates all 3 skills)
@marketing-strategist launch our new SaaS product

# Content strategy
@marketing-strategist build Q1 content strategy for our blog

# Demand generation
@marketing-strategist setup paid campaigns with $50k budget
```

**🛠️ Python Tools:** `brand_voice_analyzer.py`, `seo_optimizer.py`, `cac_calculator.py`

---

### 2. Executive Advisory Toolkit (2 skills + 1 agent)
**Install:** `/plugin install executive-advisory@mparker-claude-skills`

Strategic leadership combining CEO and CTO expertise with **Executive Advisor agent** (`@executive-advisor`) for board-level decision-making.

**🤖 Domain Agent:**
- **@executive-advisor**: Combined CEO + CTO strategic advisory for startups

**📚 Included Skills:**
- **ceo-advisor**: Strategic planning and business decision frameworks
- **cto-advisor**: Technical leadership and engineering strategy

**💡 Example Workflows:**
```bash
# Strategic planning
@executive-advisor set company OKRs for Q2 2025

# Architecture decisions
@executive-advisor should we use microservices or monolith?

# Board preparation
@executive-advisor prepare Series A board presentation
```

**🛠️ Python Tools:** `strategy_analyzer.py`, `financial_scenario_modeler.py`, `tech_debt_analyzer.py`, `team_scaling_calculator.py`

---

### 3. Product Management Toolkit (3 skills + 1 agent)
**Install:** `/plugin install product-management@mparker-claude-skills`

Complete product toolkit with **Product Lead agent** (`@product-lead`) coordinating RICE prioritization, agile delivery, and strategic planning.

**🤖 Domain Agent:**
- **@product-lead**: Head of Product with RICE, OKRs, and sprint planning expertise

**📚 Included Skills:**
- **product-manager-toolkit**: RICE prioritization, customer interviews, roadmapping
- **agile-product-owner**: User story generation, sprint planning, backlog management
- **product-strategist**: OKR cascade, strategy frameworks, market analysis

**💡 Example Workflows:**
```bash
# Feature prioritization
@product-lead prioritize Q2 roadmap with RICE framework

# Customer research
@product-lead analyze customer interview transcripts

# Sprint planning
@product-lead plan next 2-week sprint with 30 points capacity
```

**🛠️ Python Tools:** `rice_prioritizer.py`, `customer_interview_analyzer.py`, `user_story_generator.py`, `okr_cascade_generator.py`

---

### 4. UX Design Toolkit (2 skills + 1 agent)
**Install:** `/plugin install ux-design@mparker-claude-skills`

User experience and UI design with **Design Director agent** (`@design-director`) coordinating research and design systems.

**🤖 Domain Agent:**
- **@design-director**: Head of Design combining UX research and UI design expertise

**📚 Included Skills:**
- **ux-researcher-designer**: User research, persona generation, usability testing
- **ui-design-system**: Design tokens, component libraries, style guides

**💡 Example Workflows:**
```bash
# Design system creation
@design-director create design system from brand color #0066CC

# User research
@design-director generate personas from user interviews

# Design tokens
@design-director export design tokens as CSS variables
```

**🛠️ Python Tools:** `persona_generator.py`, `design_token_generator.py`

---

### 5. Project Management Toolkit (6 skills + 1 agent)
**Install:** `/plugin install project-management@mparker-claude-skills`

Complete agile delivery toolkit with **Delivery Manager agent** (`@delivery-manager`) coordinating PM, Scrum, and Atlassian tools.

**🤖 Domain Agent:**
- **@delivery-manager**: VP of Delivery managing agile ceremonies and project operations

**📚 Included Skills:**
- **senior-pm**: Project planning, risk management, stakeholder communication
- **scrum-master**: Sprint facilitation, agile ceremonies, team coaching
- **jira-expert**: Jira administration, workflow optimization, reporting
- **confluence-expert**: Documentation strategy, knowledge management
- **atlassian-admin**: Atlassian suite administration and integration
- **atlassian-templates**: Ready-to-use Jira and Confluence templates

**💡 Example Workflows:**
```bash
# Sprint setup
@delivery-manager setup new sprint in Jira with 2-week timeline

# Agile transformation
@delivery-manager implement Scrum framework for our team

# Documentation
@delivery-manager create Confluence space structure for engineering
```

**🛠️ Python Tools:** None (uses Atlassian MCP Server for direct Jira/Confluence operations)

---

### 6. Core Engineering Toolkit (9 skills + 1 agent)
**Install:** `/plugin install core-engineering@mparker-claude-skills`

Complete engineering team with **Engineering Lead agent** (`@engineering-lead`) coordinating architecture through security.

**🤖 Domain Agent:**
- **@engineering-lead**: VP of Engineering managing architecture, development, QA, DevOps, and security

**📚 Included Skills:**
- **senior-architect**: System design, architecture patterns, technical decision-making
- **senior-frontend**: React, Next.js, TypeScript, modern frontend development
- **senior-backend**: Node.js, APIs, databases, microservices
- **senior-fullstack**: Complete stack development, project scaffolding
- **senior-qa**: Test automation, quality assurance, testing strategies
- **senior-devops**: CI/CD, Docker, Kubernetes, infrastructure automation
- **senior-secops**: Security operations, vulnerability management
- **code-reviewer**: Code review best practices, quality standards
- **senior-security**: Application security, penetration testing, security architecture

**💡 Example Workflows:**
```bash
# Architecture review
@engineering-lead review our microservices architecture

# Code quality
@engineering-lead analyze code quality and security

# CI/CD setup
@engineering-lead setup CI/CD pipeline for Next.js app
```

**🛠️ Python Tools:** `project_scaffolder.py`, `code_quality_analyzer.py`, `fullstack_scaffolder.py`, `pr_analyzer.py`

---

### 7. AI/ML/Data Toolkit (5 skills + 1 agent)
**Install:** `/plugin install ai-ml-data-engineering@mparker-claude-skills`

AI/ML and data engineering with **Data Science Lead agent** (`@data-science-lead`) coordinating ML pipelines and deployment.

**🤖 Domain Agent:**
- **@data-science-lead**: Head of AI/ML/Data with MLOps and production expertise

**📚 Included Skills:**
- **senior-data-scientist**: Statistical analysis, experimentation, feature engineering
- **senior-data-engineer**: Data pipelines, ETL/ELT, data quality
- **senior-ml-engineer**: Model deployment, MLOps, production ML systems
- **senior-prompt-engineer**: LLM optimization, RAG systems, AI agents
- **senior-computer-vision**: Object detection, image processing, video analysis

**💡 Example Workflows:**
```bash
# ML pipeline
@data-science-lead build ML model deployment pipeline

# RAG system
@data-science-lead build RAG system for our documentation

# Computer vision
@data-science-lead train object detection model
```

**🛠️ Python Tools:** `experiment_designer.py`, `feature_engineering_pipeline.py`, `statistical_analyzer.py`, `pipeline_orchestrator.py`, `data_quality_validator.py`, `etl_generator.py`, `model_deployment_pipeline.py`, `mlops_setup_tool.py`, `llm_integration_builder.py`, `prompt_optimizer.py`, `rag_system_builder.py`, `agent_orchestrator.py`, `vision_model_trainer.py`, `inference_optimizer.py`, `video_processor.py`

---

### 8. Regulatory Affairs Toolkit (4 skills + 1 agent)
**Install:** `/plugin install regulatory-affairs@mparker-claude-skills`

HealthTech/MedTech compliance with **Regulatory Director agent** (`@regulatory-director`) coordinating MDR, FDA, and risk management.

**🤖 Domain Agent:**
- **@regulatory-director**: Head of Regulatory Affairs for medical device market access

**📚 Included Skills:**
- **regulatory-affairs-head**: Regulatory strategy, submissions, compliance oversight
- **mdr-745-specialist**: EU MDR 2017/745 compliance and implementation
- **fda-consultant-specialist**: FDA 510(k), PMA, quality system regulations
- **risk-management-specialist**: ISO 14971 risk management process

**💡 Example Workflows:**
```bash
# MDR compliance
@regulatory-director prepare EU MDR certification

# FDA submission
@regulatory-director prepare 510(k) submission package

# Risk management
@regulatory-director conduct ISO 14971 risk analysis
```

**🛠️ Python Tools:** `regulatory_pathway_analyzer.py`, `submission_timeline_tracker.py`, `risk_analysis_tool.py`

---

### 9. Quality Management Toolkit (5 skills + 1 agent)
**Install:** `/plugin install quality-management@mparker-claude-skills`

Quality systems with **Quality Director agent** (`@quality-director`) coordinating ISO 13485, CAPA, and ISO 27001.

**🤖 Domain Agent:**
- **@quality-director**: Head of Quality managing QMS, CAPA, and information security

**📚 Included Skills:**
- **quality-manager-qmr**: Quality management representative role
- **quality-manager-qms-iso13485**: ISO 13485 QMS implementation
- **capa-officer**: Corrective and preventive action management
- **quality-documentation-manager**: Document control and management
- **information-security-manager-iso27001**: ISO 27001 ISMS implementation

**💡 Example Workflows:**
```bash
# QMS setup
@quality-director setup ISO 13485 quality management system

# CAPA management
@quality-director investigate audit nonconformance

# ISMS setup
@quality-director implement ISO 27001 information security
```

**🛠️ Python Tools:** `qms_effectiveness_monitor.py`, `capa_tracker.py`, `document_version_controller.py`

---

### 10. Audit & Compliance Toolkit (3 skills + 1 agent)
**Install:** `/plugin install audit-compliance@mparker-claude-skills`

Audit and compliance with **Compliance Officer agent** (`@compliance-officer`) coordinating QMS, ISMS, and GDPR audits.

**🤖 Domain Agent:**
- **@compliance-officer**: Chief Compliance Officer managing internal audits and GDPR compliance

**📚 Included Skills:**
- **qms-audit-expert**: Quality management system auditing (ISO 13485)
- **isms-audit-expert**: Information security management system auditing (ISO 27001)
- **gdpr-dsgvo-expert**: GDPR/DSGVO compliance and data protection

**💡 Example Workflows:**
```bash
# Internal QMS audit
@compliance-officer conduct internal QMS audit

# ISMS audit
@compliance-officer audit information security controls

# GDPR assessment
@compliance-officer assess GDPR compliance
```

**🛠️ Python Tools:** `gdpr_compliance_checker.py`, `dpia_generator.py`, `audit_checklist_generator.py`

---

## Team Configuration

Configure automatic marketplace installation for team projects by adding to `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "mparker-claude-skills": {
      "source": {
        "source": "github",
        "repo": "Mparker25/claude-skills"
      }
    }
  },
  "enabledPlugins": [
    "marketing",
    "core-engineering",
    "product-management"
  ]
}
```

When team members trust the repository folder, Claude Code automatically installs the marketplace and specified plugins.

## Skill Structure

Each skill includes:

- **SKILL.md**: Master documentation with workflows and usage examples
- **scripts/**: Python CLI tools for algorithmic analysis (2-3 per skill)
- **references/**: Expert knowledge bases with frameworks and best practices
- **assets/**: User-facing templates and checklists (where applicable)

## Python Tools

97 production-ready Python automation tools are included across all skills:

### Running Tools

```bash
# Marketing tools
python marketing-skill/content-creator/scripts/brand_voice_analyzer.py content.txt
python marketing-skill/content-creator/scripts/seo_optimizer.py article.md "keyword"

# Product tools
python product-team/product-manager-toolkit/scripts/rice_prioritizer.py features.csv
python product-team/agile-product-owner/scripts/user_story_generator.py sprint 30

# Engineering tools
python engineering-team/senior-fullstack/scripts/project_scaffolder.py my-app --type nextjs-graphql
python engineering-team/senior-fullstack/scripts/code_quality_analyzer.py /path/to/project

# Data/ML tools
python engineering-team/senior-data-scientist/scripts/experiment_designer.py
python engineering-team/senior-ml-engineer/scripts/model_deployment_pipeline.py
```

## Troubleshooting

### Marketplace not loading

**Issue:** Can't add marketplace or see plugins

**Solutions:**
- Verify repository URL is accessible
- Check `.claude-plugin/marketplace.json` exists
- Ensure you have access to private repositories (if applicable)
- Try adding with full git URL instead of shorthand

### Plugin installation fails

**Issue:** Marketplace appears but plugin won't install

**Solutions:**
- Verify skill paths in marketplace.json
- Check that SKILL.md files exist in specified locations
- Try installing from local clone for debugging
- Review Claude Code logs for specific errors

### Skills not appearing in Claude

**Issue:** Plugin installed but skills aren't available

**Solutions:**
- Restart Claude Code session
- Verify plugin is listed in `/plugin list`
- Check that skills are enabled in settings
- Ensure SKILL.md has valid YAML frontmatter

## Contributing

Contributions welcome! Please:

1. Fork the repository
2. Create feature branch for new skills
3. Follow existing skill structure and conventions
4. Test locally before submitting PR
5. Update marketplace.json with new skills

## License

MIT License - see LICENSE file for details.

## Support

- **Issues:** https://github.com/Mparker25/claude-skills/issues
- **Documentation:** See individual SKILL.md files
- **Email:** Malik.Bernard.Parker@gmail.com

---

**Total Skills:** 42 production-ready skills
**Total Tools:** 97 Python automation tools
**Total Plugins:** 10 granular collections
**Domains Covered:** Marketing, Engineering, Product, Compliance, Leadership
