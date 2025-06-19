# Technical Requirements

These aren't suggestions. Follow them or get disqualified.

## Tech Stack (Non-Negotiable)

**Frontend**:
- React with Vite (not Create React App, not Next.js)
- React Router V7 in library mode
- TypeScript throughout (zero `any` types allowed)

**Backend**:
- Node.js with Express.js
- PostgreSQL database
- Drizzle ORM (not Prisma, not raw SQL)

**Package Manager**:
- Bun is preferred
- Yarn is acceptable IF you document why Bun doesn't work with your solution
- npm is not acceptable

**Starter Template**:
```bash
git clone git@github.com:AkongaLabs/saas-panda.git your-solution
```
Use it or don't. Your choice.

## Code Quality Standards

### Testing Requirements
- **Critical user flows must be tested**
- We don't care about 100% coverage, we care about the important stuff working
- Include test execution screenshots in your PR
- Tests must actually run and pass

### TypeScript Requirements
- Full typing throughout the codebase
- No `any` types anywhere
- No `@ts-ignore` comments unless absolutely necessary (and documented why)
- Your code should compile without warnings

### Code Documentation
- **Self-documenting code only**
- If we need to ask "what does this do?", you're disqualified
- Use clear variable names, function names, and structure
- Comments should explain WHY, not WHAT

### Architecture Standards
- Keep it simple, stupid (KISS principle)
- Don't overengineer
- Use patterns we can understand without a PhD
- Database migrations should be included and documented

## Submission Requirements

### Mandatory Checklist
Your PR gets auto-rejected if missing any of these:

- [ ] **Complete solution** that addresses all bounty requirements
- [ ] **Working tests** with execution proof
- [ ] **TypeScript compliance** (compiles without errors/warnings)
- [ ] **Package manager compatibility** (Bun preferred, Yarn with justification)
- [ ] **Working demo** (deployed link or comprehensive video)
- [ ] **Setup documentation** (how to run your code)
- [ ] **Self-explanatory code** (no external clarification needed)

### Environment Setup
Your solution must include:
- Clear environment variable documentation
- Database setup instructions
- Migration scripts (if applicable)
- Build and deployment instructions

## Automatic Disqualification

You're out if:
- ❌ Wrong tech stack
- ❌ Code doesn't work as described
- ❌ Missing or failing tests
- ❌ TypeScript errors or warnings
- ❌ Using `any` types
- ❌ Code requires explanation beyond what's self-evident
- ❌ No working demo
- ❌ npm as package manager
- ❌ Late submission
- ❌ PR modified after initial submission

## Build Requirements

Your solution must:
- Build successfully with `bun run build` (or `yarn build` with justification)
- Start with `bun run dev` (or `yarn dev`)
- Run tests with `bun test` (or `yarn test`)
- Include all necessary scripts in package.json

## Performance Expectations

We're not looking for NASA-level optimization, but your code should:
- Load reasonably fast
- Handle expected user loads
- Not have obvious performance bottlenecks
- Use efficient database queries

## Security Basics

- No hardcoded secrets or API keys
- Use environment variables for configuration
- Basic input validation where needed
- Follow standard security practices (we're not expecting security audit level, just common sense)

---

**Bottom Line**: Build working, tested, well-structured code using our stack. First working solution wins.

← [Back to Main README](../README.md) | [Submission Process](SUBMISSION.md) → | [Payment Details](PAYMENT.md) | [FAQ](FAQ.md)