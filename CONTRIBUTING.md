# Contributing to Trokky

Thank you for your interest in contributing to Trokky! This document provides guidelines and information for contributors.

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- npm 9+
- Git

### Development Setup

1. **Fork the repository** you want to contribute to
2. **Clone your fork**:
   ```bash
   git clone https://github.com/YOUR_USERNAME/REPO_NAME.git
   cd REPO_NAME
   ```
3. **Install dependencies**:
   ```bash
   npm install
   ```
4. **Start development**:
   ```bash
   npm run dev
   ```

## 📋 How to Contribute

### 🐛 Reporting Bugs
- Use the [issue tracker](https://github.com/Trokky/trokky/issues)
- Search existing issues first
- Use the bug report template
- Include reproducible steps

### 💡 Suggesting Features
- Open a [discussion](https://github.com/Trokky/trokky/discussions)
- Describe the use case
- Explain the expected behavior

### 🔧 Code Contributions

1. **Create a feature branch**:
   ```bash
   git checkout -b feature/amazing-feature
   ```

2. **Make your changes**:
   - Follow our coding standards
   - Add tests for new functionality
   - Update documentation

3. **Test your changes**:
   ```bash
   npm test
   npm run type-check
   npm run lint
   ```

4. **Commit your changes**:
   ```bash
   git commit -m "feat: add amazing feature"
   ```

5. **Push and create PR**:
   ```bash
   git push origin feature/amazing-feature
   ```

## 📝 Code Standards

### TypeScript
- Use TypeScript for all new code
- Follow existing patterns
- Add proper type annotations

### Testing
- Write tests for new features
- Maintain existing test coverage
- Use Jest for testing

### Documentation
- Update README if needed
- Add JSDoc comments
- Update TypeScript types

## 🏗️ Project Structure

### Trokky Pro
- **packages/core** - Core CMS functionality
- **packages/admin** - Admin interface
- **packages/api** - API layer
- **packages/create-project** - CLI tool

### Trokky Classic
- **src/** - Main application code
- **admin/** - Admin interface
- **cli/** - Command line tools

## 🤝 Community Guidelines

- Be respectful and inclusive
- Follow the code of conduct
- Help others learn and grow
- Share knowledge and experience

## 📞 Getting Help

- 💬 [Discord Community](https://discord.gg/trokky)
- 💡 [GitHub Discussions](https://github.com/Trokky/trokky/discussions)
- 📧 Email: contributors@trokky.com

Thank you for contributing to Trokky! 🎉