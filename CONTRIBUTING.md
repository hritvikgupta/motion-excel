# Contributing to Motion Excel

Thank you for your interest in contributing to Motion Excel! This document provides guidelines and instructions for contributing to the project.

## Code of Conduct

By participating in this project, you agree to abide by our [Code of Conduct](./CODE_OF_CONDUCT.md). Please read it before contributing.

## How Can I Contribute?

Actual codebase is private and is only invite only please fill out this form and we'll get back to you 
https://docs.google.com/forms/d/e/1FAIpQLSdkDSJsjf-Y4MghZN03eABgQ72UrOFOu4v4zyu5arYt6Gv3Uw/viewform?usp=dialog

### Reporting Bugs

Before creating bug reports, please check the issue list as you might find out that you don't need to create one. When you are creating a bug report, please include as many details as possible:

- **Use a clear and descriptive title**
- **Describe the exact steps to reproduce the problem**
- **Provide specific examples to demonstrate the steps**
- **Describe the behavior you observed after following the steps**
- **Explain which behavior you expected to see instead and why**
- **Include screenshots and animated GIFs if applicable**
- **Include system information** (OS, browser, Node.js version, etc.)

Use the [Bug Report template](./.github/ISSUE_TEMPLATE/bug_report.md) when creating a new issue.

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion, please include:

- **Use a clear and descriptive title**
- **Provide a step-by-step description of the suggested enhancement**
- **Provide specific examples to demonstrate the steps**
- **Describe the current behavior and explain which behavior you expected to see instead**
- **Explain why this enhancement would be useful**

Use the [Feature Request template](./.github/ISSUE_TEMPLATE/feature_request.md) when creating a new issue.

### Pull Requests

- Fill in the required template
- Do not include issue numbers in the PR title
- Include screenshots and animated GIFs in your pull request whenever possible
- Follow the TypeScript and React styleguides
- Include thoughtfully-worded, well-structured tests
- Document new code based on the Documentation Styleguide
- End all files with a newline

## Development Process

### Setting Up Your Development Environment

1. **Fork the repository** on GitHub

2. **Clone your fork** locally:
```bash
git clone https://github.com/YOUR_USERNAME/motion-excel.git
cd motion-excel
```

3. **Add the upstream remote**:
```bash
git remote add upstream https://github.com/hritvikgupta/motion-excel.git
```

4. **Install dependencies**:
```bash
npm install
# or
pnpm install
```

5. **Set up environment variables**:
```bash
cp .env.local.example .env.local
# Edit .env.local with your API keys
```

6. **Set up Docker service** (for code execution features):
```bash
cd docker-service
npm install
npm start
```

7. **Run the development server**:
```bash
npm run dev
```

### Making Changes

1. **Create a branch** for your feature or bug fix:
```bash
git checkout -b feature/your-feature-name
# or
git checkout -b fix/your-bug-fix-name
```

2. **Make your changes** following the coding standards below

3. **Test your changes**:
```bash
npm run test  # if tests exist
npm run lint  # check for linting errors
```

4. **Commit your changes**:
```bash
git add .
git commit -m "feat: add your feature description"
```

### Commit Message Guidelines

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

- `feat:` - A new feature
- `fix:` - A bug fix
- `docs:` - Documentation only changes
- `style:` - Changes that do not affect the meaning of the code
- `refactor:` - A code change that neither fixes a bug nor adds a feature
- `perf:` - A code change that improves performance
- `test:` - Adding missing tests or correcting existing tests
- `chore:` - Changes to the build process or auxiliary tools

Examples:
```
feat: add export to PDF functionality
fix: resolve formula calculation error in edge cases
docs: update installation instructions
refactor: improve spreadsheet rendering performance
```

### Coding Standards

#### TypeScript/JavaScript

- Use TypeScript for all new code
- Follow the existing code style
- Use meaningful variable and function names
- Add JSDoc comments for public functions
- Keep functions small and focused
- Avoid deep nesting (max 3 levels)

#### React Components

- Use functional components with hooks
- Keep components small and focused
- Extract reusable logic into custom hooks
- Use TypeScript interfaces for props
- Follow the existing component structure

#### File Naming

- Use PascalCase for component files: `SpreadsheetEditor.tsx`
- Use camelCase for utility files: `formatUtils.ts`
- Use kebab-case for configuration files: `next.config.mjs`

### Testing

- Write tests for new features
- Ensure all tests pass before submitting
- Aim for good test coverage
- Test edge cases and error scenarios

### Documentation

- Update README.md if needed
- Add JSDoc comments for new functions
- Update API documentation if applicable
- Include examples in your documentation

## Submitting Changes

### Before Submitting

- [ ] Code follows the style guidelines
- [ ] Self-review your code
- [ ] Comment complex code sections
- [ ] Update documentation as needed
- [ ] Tests pass locally
- [ ] No new warnings are introduced
- [ ] Code is properly formatted

### Pull Request Process

1. **Update your branch** with the latest changes from upstream:
```bash
git fetch upstream
git rebase upstream/main
```

2. **Push your branch** to your fork:
```bash
git push origin feature/your-feature-name
```

3. **Create a Pull Request** on GitHub:
   - Use a clear and descriptive title
   - Fill out the PR template completely
   - Link to any related issues
   - Include screenshots if applicable
   - Request review from maintainers

4. **Respond to feedback**:
   - Address review comments promptly
   - Make requested changes
   - Keep the discussion focused and constructive

### Review Process

- Maintainers will review your PR
- You may be asked to make changes
- Once approved, a maintainer will merge your PR
- Your contribution will be credited in the project

## Project Structure

```
motion-excel/
├── src/              # Source code
├── public/           # Static assets
├── api/              # API routes
├── docker-service/   # Docker service for code execution
├── docs/             # Documentation
└── tests/            # Test files
```

## Getting Help

If you need help or have questions:

- Open a [GitHub Discussion](https://github.com/hritvikgupta/motion-excel/discussions)
- Join our [Discord community](https://discord.gg/your-server)
- Check existing [Issues](https://github.com/hritvikgupta/motion-excel/issues)

## Recognition

Contributors will be recognized in:
- The project's README.md
- Release notes
- Project documentation

Thank you for contributing to Motion Excel! 🎉
