# Submission Process

How to submit your bounty solution without screwing it up.

## Before You Submit

**Read the bounty issue completely.** Seriously. Every word. If you submit something that doesn't match what we asked for, you're wasting everyone's time.

**Test everything.** If it doesn't work, don't submit it.

**Have a working demo ready.** Deploy it somewhere or record a video. We need proof it works.

## PR Template (Use This Exactly)

Copy this template into your PR description. Fill out every section. Missing sections = automatic disqualification.

```markdown
## Bounty Solution Submission

### Problem Statement
[Briefly describe what problem this bounty solves]

### Solution Approach
[Explain your technical approach and key decisions]

### Technical Implementation
- **Package Manager**: Bun ✅ / Yarn (explain why not Bun)
- **Database Setup**: [How to set up the database]
- **Environment Variables**: [List all required env vars]
- **Build Process**: [How to build the application]

### Testing Evidence
- **Test Coverage**: [What you tested]
- **Critical Flows Tested**: [List the important user flows you tested]
- **Test Results**: [Screenshot or output of your tests passing]

### Demo Evidence
Choose ONE:
- **Live Demo**: [Deployed URL with any login credentials needed]
- **Video Demo**: [Link to video showing your solution working]

### Setup Instructions
Step-by-step instructions to run your code:
1. [First step]
2. [Second step]
3. [And so on...]

### Database Setup
[How to set up the database, run migrations, seed data if needed]

### Architectural Decisions
[Document any significant choices you made and why]

### Bun/Yarn Justification
[If using Yarn, explain why Bun doesn't work with your solution]

---

**Pre-submission Checklist:**
- [ ] All bounty requirements met
- [ ] Tests written and passing
- [ ] Working demo available
- [ ] Code is self-explanatory
- [ ] Setup instructions complete
- [ ] @adrianmurage tagged for review

**I confirm this submission meets all requirements and is ready for review.**
```

## Submission Steps

1. **Fork this repository** (if you haven't already)
2. **Create your solution** in a new branch
3. **Test everything thoroughly**
4. **Deploy a demo** or record a video
5. **Create PR using the exact template above**
6. **Tag `@adrianmurage`** immediately after creating the PR
7. **Don't touch your PR** after submission

## What Happens Next

**Review Timeline**:
- Initial review: 48-72 hours
- Technical evaluation: 2-3 business days  
- Final decision: Within 5 business days

**Winner Selection**:
- First submission that meets ALL requirements wins
- Winner determined by GitHub PR timestamp
- Decision is final, no appeals

## Common Mistakes That Get You Disqualified

- **Incomplete PR template** - Fill out every section
- **No working demo** - We need proof it works
- **Missing tests** - Critical flows must be tested
- **Code that doesn't work** - Test before submitting
- **Wrong tech stack** - Use exactly what we specified
- **TypeScript errors** - Your code must compile cleanly
- **Modifying PR after submission** - Don't change anything once submitted
- **Not tagging @adrianmurage** - We won't see your PR otherwise

## Questions During Development

**Ask questions in the bounty issue comments BEFORE you start coding.**

- Be specific about what you need clarification on
- Include relevant context or examples
- Ask publicly so others can benefit from the answer
- Don't ask for hints or solutions

**Don't ask questions via**:
- Private messages
- Email
- Other repositories
- Social media

## Post-Submission

**DO NOT**:
- Modify your PR after submission
- Create multiple PRs for the same bounty
- Ask for feedback during review
- Complain about judging decisions

**Review Process**:
- We'll review in submission order
- Feedback will be posted in your PR
- Winner announcement in both PR and original issue
- Payment process starts immediately for winners

---

**Remember**: First working solution wins. No beauty contests, no politics. Just working code that solves the problem.

← [Back to Main README](../README.md) | [Technical Requirements](REQUIREMENTS.md) | [Payment Details](PAYMENT.md) | [FAQ](FAQ.md) →