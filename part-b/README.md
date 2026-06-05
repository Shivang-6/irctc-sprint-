# IRCTC Design Engineering Sprint

![Status](https://img.shields.io/badge/Status-Part%20A%20Complete-success)
![Version](https://img.shields.io/badge/Version-1.0.0-blue)
![License](https://img.shields.io/badge/License-MIT-green)

## 📋 Table of Contents

- [Overview](#overview)
- [Project Background](#project-background)
- [Repository Structure](#repository-structure)
- [Part A Deliverables](#part-a-deliverables)
- [Part B Deliverables](#part-b-deliverables)
- [Methodology](#methodology)
- [Tools Used](#tools-used)
- [How to Run](#how-to-run)
- [Git Workflow](#git-workflow)
- [Contribution Guidelines](#contribution-guidelines)
- [Submission Requirements](#submission-requirements)
- [License](#license)

## 🎯 Overview

This repository contains the deliverables for the **IRCTC Design Engineering Sprint**, a comprehensive product management and UX research project focused on identifying and documenting critical user experience issues in the Indian Railway Catering and Tourism Corporation (IRCTC) online ticketing platform.

### Sprint Structure

- **Part A:** Problem Discovery - Detailed documentation of 6 high-impact user experience issues
- **Part B:** Solution Specifications - Technical specifications, AI feature proposals, and prioritization matrices

### Project Goal

Provide actionable insights for improving the IRCTC platform's usability, reliability, and overall user experience through systematic problem identification and solution planning.

## 📚 Project Background

IRCTC (Indian Railway Catering and Tourism Corporation) is the official online ticketing platform for Indian Railways, serving millions of users daily. Despite its critical importance, the platform suffers from numerous user experience issues that impact booking efficiency, user satisfaction, and system reliability.

This sprint adopts a structured approach to:
- Identify and document critical UX problems through systematic research
- Analyze user flows and break points
- Propose technical solutions with implementation specifications
- Leverage AI capabilities to enhance platform functionality
- Prioritize improvements based on impact and effort

## Repository Structure

```
irctc-sprint/
├── README.md                          # Project overview and documentation
├── part-a/
│   └── PROBLEMS.md                    # Problem discovery documentation
├── part-b/
│   ├── SPECS.md                       # Technical solution specifications
│   ├── AI-FEATURE.md                  # AI-powered feature proposals
│   └── MATRIX.md                      # Prioritization and impact analysis
└── assets/
    └── screenshots/                   # Screenshots supporting problem documentation
```

## 📦 Part A Deliverables

### PROBLEMS.md
A comprehensive problem discovery document containing:

#### Summary
- **Total problems documented:** 6
- **Platform explored:** IRCTC
- **Devices used:** Desktop Chrome and Mobile Chrome

#### Documented Problems

| Problem | Category | Severity | Steps |
|---------|----------|----------|-------|
| Tatkal Booking Crashes at 10:00 AM | System Reliability | Critical | 12 |
| Search Filters Do Not Work Reliably | UX Functionality | High | 15 |
| Seat Selection Resets Randomly | State Management | High | 17 |
| Payment Gateway Timeout During High Traffic | Payment Integration | Critical | 15 |
| PNR Status Not Updating in Real-Time | Data Accuracy | High | 15 |
| Mobile Layout Breaks on Smaller Screens | Responsive Design | High | 17 |

#### Problem Details

**Problem 1: Tatkal Booking Crashes at 10:00 AM**
- System failure during critical booking windows
- 12-step user flow with break point analysis
- Technical failure identification (API, database, load balancer)

**Problem 2: Search Filters Do Not Work Reliably**
- Inconsistent filter application across train search
- 15-step user flow with multiple break points
- Session state and cache failure analysis

**Problem 3: Seat Selection Resets Randomly**
- Seat selection state persistence issues
- 17-step user flow demonstrating reset behavior
- Frontend state management and concurrency issues

**Problem 4: Payment Gateway Timeout During High Traffic**
- Payment integration failures during peak hours
- 15-step user flow with timeout analysis
- Gateway API and transaction lock failures

**Problem 5: PNR Status Not Updating in Real-Time**
- Delayed PNR status updates causing misinformed decisions
- 15-step user flow showing cache invalidation issues
- Database sync and cache TTL problems

**Problem 6: Mobile Layout Breaks on Smaller Screens**
- Responsive design failures on budget smartphones
- 17-step user flow demonstrating layout issues
- CSS media query and touch target failures

#### Documentation Structure
Each problem includes:
- **What is broken** - Detailed description of the issue
- **How I found it** - Discovery methodology (for self-discovered problems)
- **Affected users** - User segments impacted
- **Frequency analysis** - Occurrence rates, peak times, severity metrics
- **Current flow step by step** - Minimum 6-step user journey with break points
- **Where exactly it breaks** - Technical failure analysis (primary/secondary/tertiary)
- **Screenshot description** - Visual documentation of the issue

## 🚀 Part B Deliverables

### SPECS.md
Technical solution specifications for addressing the documented problems:
- Detailed technical requirements for each fix
- Implementation approaches and architecture recommendations
- API specifications and database schema changes
- Frontend component redesign specifications
- Testing and validation criteria

### AI-FEATURE.md
Proposed AI-powered features to enhance IRCTC platform:
- Intelligent recommendation engine for train selection
- Predictive waitlist confirmation system
- Natural language query interface
- Automated customer support chatbot
- Dynamic pricing optimization
- Fraud detection and prevention

### MATRIX.md
Prioritization and impact analysis:
- Problem prioritization matrix (severity vs. effort)
- ROI analysis for proposed solutions
- Risk assessment for implementation
- Timeline and resource allocation recommendations
- Success metrics and KPIs

## 🔬 Methodology

### Research Approach

This project employs a systematic UX research methodology:

1. **Problem Identification**
   - Direct platform exploration and testing
   - User flow analysis across critical booking journeys
   - Cross-device compatibility testing (desktop and mobile)
   - Peak traffic simulation (Tatkal booking windows)

2. **Documentation Standards**
   - Structured problem documentation with consistent format
   - Step-by-step user flow mapping with break points
   - Technical failure analysis at multiple levels
   - Frequency and severity metrics collection

3. **Solution Planning**
   - Technical specification development
   - AI capability assessment and integration planning
   - Prioritization based on impact-effort analysis
   - Implementation timeline and resource allocation

### Testing Protocol

- **Platforms:** Desktop Chrome, Mobile Chrome
- **Devices:** iPhone 13 Pro (390px), Samsung Galaxy S21 (360px), Redmi Note 7 (320px)
- **Time Periods:** Peak hours (10:00 AM - 12:00 PM), Off-peak hours (3:00 PM - 5:00 PM)
- **Test Scenarios:** Tatkal booking, regular booking, PNR tracking, seat selection

## 🛠️ Tools Used

### Research & Documentation
- **Markdown:** Documentation formatting and structure
- **Git:** Version control and collaboration
- **Chrome DevTools:** Browser inspection and debugging
- **Mobile Device Testing:** Cross-device compatibility testing

### Platforms Tested
| Platform | Purpose | Screen Sizes |
|----------|---------|--------------|
| Desktop Chrome | Primary desktop browser testing | 1920x1080, 1366x768 |
| Mobile Chrome | Mobile browser testing | 390px, 360px, 320px |
| Budget Smartphones | Responsive design validation | < 360px width |

### Documentation Tools
- **VS Code:** Code and markdown editing
- **Git:** Version control
- **GitHub:** Repository hosting and collaboration

## 🚀 How to Run

### Quick Start

```bash
# Clone the repository
git clone https://github.com/Nishant804-alt/irctc-sprint.git
cd irctc-sprint

# View Part A deliverables
cat part-a/PROBLEMS.md

# View Part B deliverables (when available)
cat part-b/SPECS.md
cat part-b/AI-FEATURE.md
cat part-b/MATRIX.md
```

### Prerequisites
- Git installed on local machine
- Basic understanding of markdown syntax
- Text editor or IDE (VS Code recommended)

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Nishant804-alt/irctc-sprint.git
   cd irctc-sprint
   ```

2. **Review Part A deliverables**
   ```bash
   # Open problem documentation
   cat part-a/PROBLEMS.md
   # Or open in your preferred markdown viewer
   ```

3. **Review Part B deliverables** (when available)
   ```bash
   # View solution specifications
   cat part-b/SPECS.md
   # View AI feature proposals
   cat part-b/AI-FEATURE.md
   # View prioritization matrix
   cat part-b/MATRIX.md
   ```

4. **View screenshots** (when available)
   ```bash
   # Navigate to screenshots directory
   cd assets/screenshots
   # View supporting screenshots
   ```

### Viewing Markdown Files
| Tool | Method | Shortcut |
|------|--------|----------|
| VS Code | Built-in markdown preview | `Ctrl+Shift+V` |
| GitHub | Automatic rendering | Open file in browser |
| Typora | Dedicated markdown editor | Open file |
| MarkText | Open source markdown editor | Open file |
| Command Line | Basic viewing | `cat` or `less` |

## 📝 Git Workflow

### Branching Strategy
- `main` branch: Main production branch
- Feature branches: Created for each major deliverable (e.g., `part-a-problems`, `part-b-specs`)

### Commit Convention
Use descriptive commit messages following conventional commit format:

```
<type>: <subject>

<body>

<footer>
```

**Types:**
| Type | Description |
|------|-------------|
| `feat` | New feature or deliverable |
| `docs` | Documentation changes |
| `fix` | Bug fixes or corrections |
| `refactor` | Code restructuring |
| `style` | Formatting changes |
| `test` | Test additions or modifications |

**Examples:**
```bash
docs: add comprehensive problem documentation for Part A
feat: complete AI feature proposals for Part B
fix: correct formatting in SPECS.md
```

### Workflow Steps

1. **Create feature branch**
   ```bash
   git checkout -b feature/<branch-name>
   ```

2. **Make changes and commit**
   ```bash
   git add .
   git commit -m "feat: add problem documentation"
   ```

3. **Push to remote**
   ```bash
   git push origin feature/<branch-name>
   ```

4. **Create pull request** (if using GitHub/GitLab)
   - Describe changes in PR description
   - Reference related issues
   - Request review from team members

5. **Merge after approval**
   - Squash commits for clean history
   - Delete feature branch after merge

### Pull Request Guidelines
- Keep PRs focused and small
- Include descriptive title and description
- Link to related issues or deliverables
- Ensure all documentation is updated
- Request review before merging

## 📋 Submission Requirements

### Part A Submission Checklist
- [x] PROBLEMS.md completed with 6 documented problems
- [x] Each problem includes affected users section
- [x] Each problem includes frequency analysis
- [x] Each problem includes minimum 6-step current flow
- [x] Each problem clearly identifies exact failure points
- [x] Professional markdown formatting throughout
- [x] Screenshots documented in description sections
- [ ] Actual screenshot files added to assets/screenshots/ (optional)

### Part B Submission Checklist (To Be Completed)
- [ ] SPECS.md with technical solution specifications
- [ ] AI-FEATURE.md with AI-powered feature proposals
- [ ] MATRIX.md with prioritization and impact analysis
- [ ] All deliverables follow professional markdown formatting
- [ ] Cross-references between Part A problems and Part B solutions
- [ ] Implementation timeline and resource allocation

### Quality Standards
| Standard | Description |
|----------|-------------|
| **Clarity** | All documentation must be clear and concise |
| **Completeness** | All sections must be thoroughly filled |
| **Accuracy** | Technical details must be accurate and realistic |
| **Professionalism** | Maintain professional tone throughout |
| **Consistency** | Use consistent formatting and terminology |
| **Actionability** | Solutions must be implementable and specific |

### Final Submission
1. Ensure all deliverables are complete
2. Verify markdown formatting renders correctly
3. Check all links and references work
4. Commit all changes with descriptive message
5. Push to main branch
6. Create release tag (if applicable)
7. Submit repository link or zip file as required

## 🤝 Contribution Guidelines

### How to Contribute
Contributions are welcome! Please follow these guidelines:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/amazing-feature`)
3. **Commit your changes** (`git commit -m 'feat: add amazing feature'`)
4. **Push to the branch** (`git push origin feature/amazing-feature`)
5. **Open a Pull Request**

### Code of Conduct
- Be respectful and constructive
- Provide clear and detailed commit messages
- Ensure all documentation is updated
- Follow the established commit conventions
- Test changes before submitting

### Reporting Issues
If you find any issues or have suggestions:
1. Check existing issues to avoid duplicates
2. Create a new issue with descriptive title
3. Provide detailed description of the problem
4. Include steps to reproduce (if applicable)
5. Suggest potential solutions (if known)

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 📞 Contact & Support

For questions or clarifications regarding this sprint:
- Review the documentation in each deliverable
- Check git commit history for change rationale
- Refer to project guidelines provided by instructors/mentors

---

**Last Updated:** June 5, 2026  
**Version:** 1.0.0  
**Status:** Part A Complete, Part B In Progress  
**Repository:** https://github.com/Nishant804-alt/irctc-sprint