# Motion Excel

**An AI-Powered Spreadsheet Application Built with CopilotKit**

Motion Excel is a modern, intelligent spreadsheet application that combines the power of Excel-like functionality with AI assistance. Built using Next.js, CopilotKit, and cutting-edge web technologies, it enables users to create, edit, and manage spreadsheets with natural language commands and AI-powered features.

---

## **Table of contents**

- 🌈 [Highlights](#-highlights)
- ✨ [Features](#-features)
- 🚀 [Getting Started](#-getting-started)
- 📖 [Documentation](#-documentation)
- 🔍 [Architecture](#-architecture)
- 🌐 [Internationalization](#-internationalization)
- 🔮 [Showcase](#-showcase)
- 💬 [Community](#-community)
- 🤝 [Contribution](#-contribution)
- 🔒 [Security](#-security)
- 📄 [License](#-license)

---

## 🌈 **Highlights**

- 🤖 **AI-Powered**: Motion Excel integrates CopilotKit to provide intelligent assistance, allowing you to build spreadsheets using natural language commands.
- 📊 **Excel-Like Functionality**: Full-featured spreadsheet with formulas, formatting, data validation, and more.
- ⚡ **High Performance**: Built with modern web technologies for fast, responsive performance.
- 🔌 **Extensible**: Plugin architecture makes it easy to extend functionality and customize the experience.
- 🌐 **Web-Based**: Runs entirely in the browser with no installation required.
- 🎨 **Modern UI**: Clean, intuitive interface designed for productivity.
- 🔄 **Real-Time Collaboration**: Support for collaborative editing (coming soon).

---

## ✨ **Features**

### Core Spreadsheet Features

- **📊 Spreadsheet Operations**
  - Create, edit, and manage multiple spreadsheets
  - Support for formulas and functions
  - Cell formatting (bold, italic, underline, colors)
  - Data validation and input constraints
  - Row and column manipulation
  - Copy, paste, and cell operations

- **🤖 AI Copilot Integration**
  - Natural language commands to build spreadsheets
  - Intelligent formula suggestions
  - Data analysis assistance
  - Automated spreadsheet generation
  - Research agent integration for data gathering

- **💾 Import & Export**
  - Import from XLSX files
  - Export to XLSX format
  - Export to PDF (coming soon)
  - Print functionality

- **🔍 Advanced Features**
  - Web search integration via research agents
  - Code execution support (Python, SQL)
  - Data visualization capabilities
  - Conditional formatting (coming soon)
  - Charts and graphs (coming soon)

### Technical Features

- **⚙️ Technology Stack**
  - Built with Next.js 15 and React 18
  - TypeScript for type safety
  - CopilotKit for AI integration
  - Multiple spreadsheet libraries support (Handsontable, ReactGrid, Syncfusion)
  - Docker service for code execution
  - WebSocket support for real-time features

- **🔌 Extensibility**
  - Plugin architecture
  - Customizable UI components
  - API for third-party integrations
  - Webhook support

---

## 🚀 **Getting Started**

### Prerequisites

- Node.js 18+ and npm/pnpm
- Docker (for code execution features)
- API keys for AI services (optional but recommended)

### Installation

1. **Clone the repository:**

```bash
git clone https://github.com/hritvikgupta/motion-excel.git
cd motion-excel
```

2. **Install dependencies:**

```bash
npm install
# or
pnpm install
```

3. **Set up environment variables:**

Copy `.env.local.example` to `.env.local` and populate the required variables:

```bash
cp .env.local.example .env.local
```

**Required Environment Variables:**

- `PARALLEL_API_KEY` - For Parallel FindAll API (dataset/table creation from web)
- `PERPLEXITY_API_KEY` - For Perplexity API (general web search queries)
- `DOCKER_SERVICE_URL` - URL for Docker service (default: `http://localhost:3001`)

Get your API keys:
- Parallel: https://platform.parallel.ai/settings?tab=api-keys
- Perplexity: https://www.perplexity.ai/settings/account

4. **Set up Docker Service (Required for Code Execution):**

The Docker service runs separately and manages code execution containers.

**Option A: Local Development**

```bash
cd docker-service
npm install
npm start
```

The service will run on `http://localhost:3001` by default.

**Option B: AWS/Production Deployment**

Deploy the Docker service to AWS EC2, ECS, or your server and set `DOCKER_SERVICE_URL` accordingly.

5. **Run the development server:**

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Quick Start Example

Once the app is running, try asking the AI copilot:

> "Create a budget spreadsheet for monthly expenses"

The AI will automatically generate a spreadsheet with the requested structure and formulas.

---

## 📖 **Documentation**

- [Official Documentation](https://docs.copilotkit.ai) - Learn about CopilotKit features and API
- [Tutorial: Building an AI-Powered Spreadsheet](https://dev.to/copilotkit/build-an-ai-powered-spreadsheet-app-nextjs-langchain-copilotkit-109d) - Step-by-step guide
- [API Reference](./docs/API.md) - Complete API documentation (coming soon)
- [Architecture Guide](./docs/ARCHITECTURE.md) - Technical architecture details (coming soon)

---

## 🔍 **Architecture**

### Key Components

1. **Frontend (`/src`)**
   - Next.js application with React components
   - CopilotKit integration for AI features
   - Multiple spreadsheet library integrations

2. **API Routes (`/api`)**
   - `/api/copilotkit/route.ts` - Main CopilotKit API endpoint
   - `/api/copilotkit/tavily.ts` - Research agent integration

3. **Docker Service**
   - Separate service for code execution
   - Python and SQL execution in isolated containers
   - Container management and cleanup

### Key Integration Points

- `useCopilotReadable` - Makes frontend application context accessible to the Copilot engine
- `updateSpreadsheet`, `appendToSpreadsheet`, `createSpreadsheet` - Application interaction hooks for agents

---

## 🌐 **Internationalization**

Motion Excel is designed to support multiple languages. Currently available in:

- English (default)
- More languages coming soon

---

## 🔮 **Showcase**

### Live Demo

Try Motion Excel in action:

[**🚀 Run Live Demo**](https://spreadsheet-demo-tau.vercel.app/)

### Example Use Cases

- **Budget Planning**: Create comprehensive budget spreadsheets with automatic calculations
- **Data Analysis**: Analyze datasets with AI-powered insights
- **Project Management**: Track projects with custom spreadsheet templates
- **Financial Modeling**: Build financial models with complex formulas

---

## 💬 **Community**

Motion Excel is an inclusive and welcoming project. We encourage community participation and contributions.

### Get Involved

- **GitHub Discussions**: Share ideas and ask questions
- **Discord**: Join our community for real-time discussions
- **Stack Overflow**: Tag questions with `motion-excel`
- **Twitter/X**: Follow [@motionexcel](https://twitter.com/motionexcel) for updates

### Code of Conduct

Please read our [Code of Conduct](./CODE_OF_CONDUCT.md) before participating in the community.

---

## 🤝 **Contribution**

We welcome contributions! Motion Excel is open to contributions from the community.

### How to Contribute

1. **Report Issues**: Found a bug or have a feature request? Please [open an issue](https://github.com/hritvikgupta/motion-excel/issues)
2. **Submit Pull Requests**: Want to contribute code? Please read our [Contributing Guide](./CONTRIBUTING.md) first
3. **Improve Documentation**: Help us improve our documentation

### Contribution Guidelines

If you would like to contribute code to Motion Excel, please refer to the [Contributing Guide](./CONTRIBUTING.md). It will guide you through:

- Setting up the development environment
- Coding standards and best practices
- Testing requirements
- Submitting pull requests

---

## 🔒 **Security**

Motion Excel is committed to maintaining a secure codebase. We follow best practices for security and regularly update our dependencies.

### Reporting Security Issues

If you discover a security vulnerability, please refer to our [Security Policy](./SECURITY.md) for information on how to report it responsibly.

**Please do not** report security vulnerabilities through public GitHub issues.

---

## 📄 **License**

Motion Excel is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.

---

## 🙏 **Acknowledgments**

- [CopilotKit](https://github.com/CopilotKit/CopilotKit) - For the amazing AI integration framework
- [Next.js](https://nextjs.org/) - For the powerful React framework
- All contributors and users of Motion Excel

---

## 📞 **Contact**

- **GitHub**: [@hritvikgupta](https://github.com/hritvikgupta)
- **Issues**: [GitHub Issues](https://github.com/hritvikgupta/motion-excel/issues)
- **Email**: [Your email here]

---

<div align="center">

**Made with ❤️ by the Motion Excel team**

[⭐ Star us on GitHub](https://github.com/hritvikgupta/motion-excel) | [📖 Documentation](./docs) | [💬 Discord](https://discord.gg/your-server) | [🐦 Twitter](https://twitter.com/motionexcel)

</div>
