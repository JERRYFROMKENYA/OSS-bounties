# Akong'a Labs OSS Bounties

Welcome to the **Akong'a Labs Open Source Software Bounties Repository**! This repository hosts bounties for development tasks that [Akong'a Labs](https://akongalabs.com) would like to outsource to the open source community instead of building in-house.

## About Akong'a Labs

[Akong'a Labs](https://akongalabs.com) is a technology company focused on building innovative software solutions. We believe in the power of open source collaboration and are excited to work with talented developers from around the world to solve interesting technical challenges.

## How It Works

1. **Bounty Posting**: Akong'a Labs team members, will create GitHub issues describing specific development tasks with associated bounties.

2. **Solution Submission**: Contributors submit solutions by creating Pull Requests to this repository.

3. **Review & Selection**: The first submission that meets all requirements wins the bounty.

4. **Winner Determination**: Winners are determined by Pull Request submission timestamp - first **VALID** submission wins.

### ⚠️ **Payment Requirements Warning**

**BEFORE YOU START:** Payments are ONLY processed via Binance using USDT/USDC cryptocurrency. If you cannot receive payments through Binance, do not participate in bounties. See [Payment Process](#payment-process) section for complete details including 6-month forfeiture policy.

## 🚨 Important Legal Notice

**By opening a Pull Request to this repository, you automatically agree that:**

- Your contributed code becomes **Free and Open Source Software (FOSS)** that anyone can use
- You grant **Akong'a Labs unlimited usage rights** to your code, regardless of whether your submission is selected
- Your code will be licensed under terms that support these usage rights
- This agreement is binding upon PR submission - no exceptions

## Technical Requirements

All submissions **MUST** meet the following technical requirements:

### Required Tech Stack
- **Frontend**: Vanilla React with Vite
- **Routing**: React Router V7 (library mode)  
- **Backend**: Node.js with Express.js
- **Database**: PostgreSQL
- **ORM**: Drizzle ORM
- **Language**: TypeScript with full typing (no `any` types)

### Package Manager Requirements
- **Primary**: All submissions must be compatible with [Bun](https://bun.sh)
- **Exception**: Yarn is acceptable ONLY if you provide clear technical justification for why Bun is incompatible with your solution
- **Documentation**: If using Yarn, you must document the incompatibility reason in your PR description

### Starter Boilerplate
Contributors are encouraged to use the Akong'a Labs [provided starter template](https://github.com/AkongaLabs/saas-panda):

```bash
git clone git@github.com:AkongaLabs/saas-panda.git
```

### Code Quality Standards
- **Testing**: Comprehensive tests for all critical user flows
- **Documentation**: Self-documenting code - if we need to ask questions about your implementation, your submission will be disqualified
- **Type Safety**: Full TypeScript typing throughout the codebase
- **Code Style**: Clean, readable, and maintainable code

## Submission Requirements

To be considered for a bounty, your submission must:

### ✅ Mandatory Checklist
- [ ] **Complete Implementation**: Fully functional solution addressing all requirements in the issue
- [ ] **Comprehensive Testing**: Tests covering all critical user flows with evidence of test execution
- [ ] **TypeScript Compliance**: Fully typed codebase with no `any` types
- [ ] **Bun Compatibility**: Works with Bun package manager (or documented Yarn justification)
- [ ] **Working Demo**: Deployed application or comprehensive video demonstration
- [ ] **Documentation**: Clear setup instructions, API documentation, and architectural decisions
- [ ] **Self-Documenting Code**: Code that explains itself without requiring external clarification

### 📋 Pull Request Requirements
When submitting your PR, you **MUST** follow this template:

#### Required PR Template
```markdown
## Bounty Solution Submission

### Problem Statement
[Briefly describe the problem this bounty addresses]

### Solution Approach
[Explain your technical approach and key decisions]

### Technical Implementation
- **Package Manager**: Bun ✅ / Yarn (with justification)
- **Database Migrations**: [How to run migrations]
- **Environment Setup**: [Required environment variables]
- **Build Process**: [How to build the application]

### Testing Evidence
- **Test Coverage**: [Percentage or description of coverage]
- **Critical Flow Tests**: [List of critical flows tested]
- **Test Execution**: [Screenshot or output of test runs]

### Demo Evidence
- **Live Demo**: [Deployment URL] OR
- **Video Demo**: [Link to video demonstration]
- **Login Credentials**: [If applicable, provide demo credentials]

### Setup Instructions
1. [Step-by-step setup instructions]
2. [Database setup]
3. [Environment configuration]
4. [How to run the application]

### Architectural Decisions
[Document any significant architectural choices made]

### Compatibility Notes
[Any specific compatibility considerations or requirements]

---
**Checklist before submission:**
- [ ] All technical requirements met
- [ ] Comprehensive tests written and passing
- [ ] Working demo available
- [ ] Code is self-documenting
- [ ] Setup instructions are complete
- [ ] @adrianmurage tagged for review
```

#### Submission Process
1. **Use the Template**: Copy the template above into your PR description
2. **Complete All Sections**: Every section must be filled out completely
3. **Tag for Review**: Tag `@adrianmurage` immediately upon PR creation
4. **No Post-Submission Changes**: PRs modified after submission will be automatically disqualified

## Disqualification Criteria

Your submission will be **automatically disqualified** if:

- ❌ Any technical requirement is not met
- ❌ Tests are missing or don't cover critical flows
- ❌ Code requires explanation beyond what's self-evident
- ❌ PR is submitted after the deadline (if specified in the issue)
- ❌ PR is modified after initial submission
- ❌ Missing working demo or deployment
- ❌ Bun incompatibility without proper justification

## Winner Selection Process

- **First Valid Submission Wins**: The first PR that meets ALL requirements wins the bounty
- **Timestamp Matters**: Winner determined by GitHub PR submission timestamp
- **Review Timeline**: Initial review within 48-72 hours of submission
- **Final Decision**: Adrian Murage makes the final selection decision

## AI Development Support

**We strongly encourage the use of AI tools to accelerate your development!** 🤖

This repository includes a comprehensive `.cursorrules` file specifically designed to help AI assistants understand our bounty requirements, coding standards, and development workflow.

### Supported AI Editors

The `.cursorrules` file is optimized for:
- **[Cursor](https://cursor.com)** - AI-first code editor
- **[Zed](https://zed.dev)** - High-performance collaborative editor
- **Other AI-powered editors** that support `.cursorrules` configuration

### What's Included in .cursorrules

Our configuration file provides AI assistants with:
- **Project Context**: Understanding of Akong'a Labs bounty program
- **Technical Requirements**: Complete tech stack specifications (React/Vite + React Router V7 + Node.js/Express + PostgreSQL + Drizzle + TypeScript)
- **Quality Standards**: Testing requirements, code quality expectations, and documentation standards
- **Submission Guidelines**: PR template requirements and review process
- **Complexity Guidelines**: Emphasis on simple, maintainable solutions
- **Common Patterns**: Preferred coding patterns and architectural decisions

### How to Use AI Tools Effectively

#### Getting Started
1. **Open the Repository**: Load this repository in your AI-powered editor
2. **AI Context Loading**: The `.cursorrules` file will automatically provide context to your AI assistant
3. **Ask Informed Questions**: Your AI assistant will understand the bounty requirements and can help you plan your approach

#### AI-Assisted Development Workflow
```bash
# 1. Clone and setup
git clone git@github.com:AkongaLabs/saas-panda.git your-bounty-solution
cd your-bounty-solution

# 2. Use AI to understand requirements
# Ask your AI: "Help me analyze the bounty requirements and plan my approach"

# 3. AI-assisted coding
# Example prompts:
# - "Generate TypeScript interfaces for this bounty's data model"
# - "Create comprehensive tests for the critical user flow described in the bounty"
# - "Help me implement this feature following the tech stack requirements"
```

#### Best AI Prompts for Bounty Development
- **Planning**: "Analyze the bounty requirements and create a development plan"
- **Architecture**: "Design the database schema and API structure for this bounty"
- **Testing**: "Generate comprehensive tests for [specific feature] covering all critical flows"
- **Documentation**: "Help me write self-documenting code and clear setup instructions"
- **Review**: "Review my code against the bounty requirements and quality standards"

### AI Advantages for Bounties

Using AI tools with our `.cursorrules` configuration gives you:
- **Faster Development**: AI understands our patterns and can generate boilerplate quickly
- **Quality Assurance**: AI knows our standards and can help ensure compliance
- **Testing Support**: AI can generate comprehensive test suites for critical flows
- **Documentation**: AI can help create self-documenting code and clear documentation
- **Technical Guidance**: AI understands our tech stack and can provide specific guidance

### AI Development Tips

#### Do's ✅
- **Use AI for boilerplate generation** following our tech stack requirements
- **Ask AI to review your code** against bounty requirements before submission
- **Leverage AI for test generation** to ensure comprehensive coverage
- **Use AI to explain complex code** to ensure it's self-documenting
- **Ask AI for optimization suggestions** within our simplicity guidelines

#### Don'ts ❌
- **Don't rely solely on AI** - understand and review all generated code
- **Don't ignore the bounty requirements** - AI should supplement, not replace careful reading
- **Don't submit code you don't understand** - you must be able to explain your implementation
- **Don't skip testing** - AI-generated code still needs thorough testing

### Getting Help with AI Tools

If you're new to AI-assisted development:
1. **Start Simple**: Begin with basic prompts and gradually get more specific
2. **Iterate**: Refine your prompts based on AI responses
3. **Verify**: Always test and verify AI-generated code
4. **Learn**: Use AI as a learning tool to understand our tech stack better

**Remember**: AI is a powerful accelerator, but the final submission must meet all bounty requirements and be code you fully understand and can maintain.

## Payment Process

### 🚨 **IMPORTANT: Payment Method Requirements**

**Akong'a Labs ONLY processes payments via Binance using USDT or USDC cryptocurrency.** If you cannot receive payments through this method, please do not participate in bounties.

### Supported Payment Methods
- **Platform**: Binance exchange only
- **Currencies**: USDT (Tether) or USDC (USD Coin) only
- **Network**: Will be specified at time of payment
- **No Alternatives**: No other payment methods, platforms, or currencies are supported

### Winner Payment Process

#### 1. Winner Notification (Within 24 hours)
- Winner will be notified via GitHub issue and PR comments
- Payment instructions will be provided immediately
- Winner must respond within 48 hours to begin payment process

#### 2. Payment Information Collection (2-3 business days)
Winner must provide:
- **Valid Binance account email address**
- **Binance UID (User ID)**
- **Preferred currency**: USDT or USDC
- **Preferred network**: (e.g., Ethereum, Binance Smart Chain, Polygon)
- **Confirmation of account verification status**

#### 3. Payment Processing (3-5 business days)
- Payment will be processed within 5 business days of receiving complete information
- Transaction hash will be provided as confirmation
- Winner is responsible for monitoring their Binance account

### ⚠️ Forfeiture Policy

#### Automatic Forfeiture Conditions
Your winnings will be **automatically forfeited** if:
- You do not have a valid, verified Binance account
- You cannot or will not provide required payment information
- You do not respond to payment notifications within specified timeframes
- You refuse to accept payment via USDT/USDC on Binance

#### 6-Month Holding Period
- **Winnings Held**: If you forfeit winnings but may be able to claim later, winnings will be held for exactly **6 months** from the original win date
- **No Extensions**: The 6-month period is absolute with no extensions or exceptions
- **Claiming Process**: During the 6-month period, you may claim winnings by providing valid Binance payment information

#### Final Forfeiture and Donation
- **After 6 Months**: Unclaimed winnings are permanently forfeited
- **OSS Donation**: Forfeited funds will be donated to an open source software repository chosen by [@adrianmurage](https://github.com/adrianmurage)
- **Public Transparency**: All donations will be publicly documented in this repository

### Payment Timeline Summary
- **Winner Notification**: Within 24 hours of selection
- **Information Collection**: 2-3 business days
- **Payment Processing**: 3-5 business days
- **Total Timeline**: 5-8 business days for complete payment
- **Forfeiture Holding**: 6 months maximum
- **Final Forfeiture**: Automatic after 6 months

### Frequently Asked Questions

#### Q: Can I use a different exchange or wallet?
**A: No.** Only Binance accounts are supported. No other exchanges, wallets, or payment methods are accepted.

#### Q: Can I receive payment in Bitcoin or other cryptocurrencies?
**A: No.** Only USDT and USDC are supported.

#### Q: What if I don't have a Binance account?
**A: You can create one before participating, but you must have a verified account to receive payments. Consider this requirement before starting work on any bounty.**

#### Q: What if Binance is not available in my country?
**A: Unfortunately, you will not be able to receive payments and should not participate in bounties.**

#### Q: Can the 6-month holding period be extended?
**A: No.** The 6-month period is absolute with no exceptions.

#### Q: What happens to forfeited funds?
**A: They are donated to open source software projects chosen by [@adrianmurage](https://github.com/adrianmurage), with full public transparency.**

### Before You Start Any Bounty

**✅ Verify you can receive payments by ensuring you have:**
- [ ] Active, verified Binance account
- [ ] Ability to receive USDT or USDC
- [ ] Understanding of cryptocurrency transactions
- [ ] Agreement to the 6-month forfeiture policy

**⚠️ By participating in any bounty, you acknowledge and agree to these payment terms.**

## Communication Guidelines

### Question Protocol
- **Pre-Development Questions**: Ask clarifying questions in the GitHub issue comments BEFORE starting work
- **Technical Questions**: All technical questions must be asked publicly in the bounty issue
- **Process Questions**: Create a new issue with the `question` label for process-related questions
- **No Private Communication**: All communication must be public in GitHub issues - no private messages or emails

### Response Expectations
- **Question Responses**: Expect responses within 24-48 hours during business days
- **Review Updates**: Regular updates on review progress will be posted in your PR
- **Final Decisions**: Winner announcements will be made publicly in the issue and PR

### Communication Standards
- **Be Specific**: Ask detailed, specific questions rather than vague inquiries
- **Provide Context**: Include relevant code snippets or examples when asking technical questions
- **Stay Professional**: Maintain professional communication at all times
- **One Question Per Comment**: Ask one question per comment for clarity

### Prohibited Communication
- ❌ Private messages or emails about bounties
- ❌ Requests for hints or solutions
- ❌ Complaints about judging decisions in public channels
- ❌ Attempts to negotiate requirements after submission

## Quality Assurance

To ensure high-quality submissions:

### Automated Validation
Your submission will be automatically checked for:
- **TypeScript Compilation**: Must compile without errors
- **Test Execution**: All tests must pass
- **Bun Compatibility**: Package installation and build must work with Bun
- **Code Quality**: Linting and formatting standards
- **Security**: Basic security vulnerability checks

### Submission Scoring System
Your submission will be evaluated using this weighted scoring system:

#### Technical Implementation (40 points)
- **Code Quality** (15 points): Clean, readable, maintainable code
- **Architecture** (15 points): Sound architectural decisions and patterns
- **Performance** (10 points): Efficient implementation and optimization

#### Testing Coverage (30 points)
- **Critical Flow Coverage** (20 points): All critical user flows tested
- **Test Quality** (10 points): Well-written, meaningful tests

#### Documentation & Setup (20 points)
- **Code Documentation** (10 points): Self-documenting code with clear comments
- **Setup Instructions** (10 points): Complete, accurate setup documentation

#### User Experience (10 points)
- **Interface Design** (5 points): Intuitive and user-friendly interface
- **Functionality** (5 points): Smooth user flows and error handling

### Minimum Passing Score
- **Total Score Required**: 70/100 points
- **Critical Requirements**: Must score at least 15/20 on Critical Flow Coverage
- **Automatic Disqualification**: Any missing mandatory requirement results in 0 points

### Review Timeline
- **Initial Review**: Within 48-72 hours of submission
- **Technical Evaluation**: 2-3 business days for full technical review
- **Final Decision**: Within 5 business days of submission
- **Winner Notification**: Immediate notification upon decision

## Getting Started

### Pre-Development Checklist
Before starting any bounty:
- [ ] Read the bounty issue completely
- [ ] Understand all technical requirements
- [ ] Review this README thoroughly
- [ ] **Verify payment eligibility**: Confirm you have a verified Binance account and can receive USDT/USDC
- [ ] **Acknowledge forfeiture policy**: Understand the 6-month forfeiture policy for unclaimed winnings
- [ ] Ask clarifying questions in issue comments
- [ ] Confirm you can meet the submission timeline

### Development Process
1. **Browse Open Bounties**: Check the [Issues](../../issues) tab for available bounties
2. **Read Issue Details**: Carefully review all requirements and acceptance criteria
3. **Ask Questions**: Use issue comments for any clarifications BEFORE starting
4. **Clone Starter**: (Optional) Use our starter template for faster setup
   ```bash
   git clone git@github.com:AkongaLabs/saas-panda.git your-bounty-solution
   cd your-bounty-solution
   bun install
   ```
5. **Set Up Development Environment**: 
   - Install Bun: `curl -fsSL https://bun.sh/install | bash`
   - Set up PostgreSQL database
   - Configure environment variables
6. **Develop Solution**: Build your solution meeting all technical requirements
7. **Write Tests**: Ensure comprehensive test coverage of critical flows
8. **Test Thoroughly**: Run all tests and verify they pass
9. **Document Everything**: Create clear documentation and setup instructions
10. **Deploy Demo**: Create a working deployment or video demonstration
11. **Submit PR**: Use the required PR template and tag `@adrianmurage`

### Quick Start Commands
```bash
# Using Bun (preferred)
bun install
bun run dev
bun run test
bun run build

# If using Yarn (with justification)
yarn install
yarn dev
yarn test
yarn build
```

## Repository Structure

```
oss-bounties/
├── .cursorrules          # AI editor configuration
├── .gitignore           # Git ignore rules
└── README.md           # This file
```

Individual bounty solutions should be submitted as separate repositories and linked in PRs to this repository.

---

## Questions?

- **Technical Questions**: Ask in the specific bounty issue
- **Process Questions**: Create a new issue with the `question` label

**Happy coding! 🚀**

---

*This repository is maintained by [Akong'a Labs](https://akongalabs.com). By participating, you agree to our open source licensing terms outlined above.*