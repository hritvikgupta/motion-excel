# Motion Excel

**An AI-Powered Spreadsheet Application Built with CopilotKit. Extensible. High-performance. Embedded to your application.**

English | [简体中文](#) | [日本語](#) | [Español](#)

[Official Site](#) | [Documentation](#) | [Online Playground](https://spreadsheet-demo-tau.vercel.app/) | [Blog](#)

![license](https://img.shields.io/badge/license-MIT-green)
![build](https://img.shields.io/badge/build-passing-green)
![stars](https://img.shields.io/badge/stars-0-blue)
![contributors](https://img.shields.io/badge/contributors-1-green)
![forks](https://img.shields.io/badge/forks-0-blue)
![issues](https://img.shields.io/badge/issues-0-orange)
![discord](https://img.shields.io/badge/discord-join-blue)

**Use Motion Excel to build AI-powered spreadsheets with natural language and create intelligent, data-driven applications.**

<div align="center">

https://github.com/user-attachments/assets/992b06ae-be6c-4bd2-ae57-20a793688e78

</div>

---

## **Table of contents**

- 🌈 [Highlights](#-highlights)
- ✨ [Features](#-features)
  - 📊 [Spreadsheet Features](#-spreadsheet-features)
  - 🤖 [AI Copilot Features](#-ai-copilot-features)
  - 🔧 [Technical Features](#-technical-features)
- 🚀 [Getting Started](#-getting-started)
- 📖 [Documentation](#-documentation)
- 🔮 [Showcase](#-showcase)
- 🌐 [Internationalization](#-internationalization)
- 💬 [Community](#-community)
- 🤝 [Contribution](#-contribution)
- ❤️ [Sponsors](#-sponsors)
- 📄 [License](#-license)

---

## 🌈 **Highlights**

- 📈 **Motion Excel is designed to support spreadsheets with AI-powered assistance and natural language commands.**
- 🧙‍♀️ **Motion Excel is isomorphic.** It can run both on browsers and Node.js, with the same API.
- ⚙️ **Motion Excel is easily embeddable**, allowing seamless integration into your applications.
- 🌟 **Motion Excel is powerful**, offering a wide range of features including **formulas, conditional formatting, data validation, filtering, collaborative editing, printing, import & export** and more features on the horizon.
- 🔌 **Motion Excel is highly extensible**, thanks to its **plug-in architecture** that makes it a delight for developers to customize and extend.

---

## ✨ **Features**

### 📊 **Spreadsheet Features**

- **Zen Editor**: Offers a distraction-free editing experience with a clean interface and minimal distractions.
- **Formulas & Functions**: Supports a wide range of Excel-compatible formulas and functions.
- **Cell Formatting**: Full support for cell formatting including bold, italic, underline, colors, and more.
- **Data Validation**: Allows setting input constraints and validation rules for cells.
- **Row & Column Operations**: Insert, delete, resize rows and columns with ease.
- **Copy & Paste**: Standard clipboard operations for cells and ranges.
- **Import & Export** `[1]`: Support for importing and exporting data in XLSX format.
- **Printing** `[1]`: Allows printing a spreadsheet or exporting it to PDF.
- **Charts** `[1]`: Supports various types of charts, including bar charts, line charts, pie charts, scatter plots, and more (coming soon).
- **Collaborative Editing** `[1]`: Supports multiple users editing a spreadsheet simultaneously. File history and recovery are also provided (coming soon).
- **Editing History** `[1]`: Allows users to view and restore previous versions of a spreadsheet (coming soon).

### 🤖 **AI Copilot Features**

- **Natural Language Commands**: Build spreadsheets using plain English commands.
- **Intelligent Formula Suggestions**: AI-powered formula recommendations based on context.
- **Automated Spreadsheet Generation**: Create complete spreadsheets from natural language descriptions.
- **Data Analysis Assistance**: Get AI-powered insights and analysis of your data.
- **Research Agent Integration**: Gather data from the web and integrate it into your spreadsheets.
- **Code Execution**: Execute Python and SQL code directly within the spreadsheet environment.

### 🔧 **Technical Features**

- **Modern Tech Stack**: Built with Next.js 15, React 18, and TypeScript.
- **Multiple Library Support**: Integrates with Handsontable, ReactGrid, and Syncfusion.
- **Docker Service**: Isolated code execution in Docker containers.
- **WebSocket Support**: Real-time features and collaboration support.
- **Plugin Architecture**: Extensible design for custom functionality.
- **API Integration**: RESTful API for third-party integrations.

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

- [CopilotKit Documentation](https://docs.copilotkit.ai/getting-started/quickstart-chatbot) - Learn about CopilotKit features and API
- [Tutorial: Building an AI-Powered Spreadsheet](https://dev.to/copilotkit/build-an-ai-powered-spreadsheet-app-nextjs-langchain-copilotkit-109d) - Step-by-step guide
- [GitHub](https://github.com/CopilotKit/CopilotKit) - Check out the CopilotKit GitHub repository
- [Discord](https://discord.gg/6dffbvGU3D) - Join the CopilotKit Discord community

---

## 🔮 **Showcase**

**Embed Motion Excel in AI products as a data presentation tool.**

<div align="center">

![Showcase](https://github.com/user-attachments/assets/992b06ae-be6c-4bd2-ae57-20a793688e78)

</div>

You can find all the examples in the **[Motion Excel Examples](#)**.

### Example Use Cases

- **Budget Planning**: Create comprehensive budget spreadsheets with automatic calculations
- **Data Analysis**: Analyze datasets with AI-powered insights
- **Project Management**: Track projects with custom spreadsheet templates
- **Financial Modeling**: Build financial models with complex formulas
- **AI-Powered Data Presentation**: Use natural language to create and modify spreadsheets

---

## 🌐 **Internationalization**

Motion Excel is designed to support multiple languages. Currently available in:

- English (default)
- More languages coming soon

---

## 💬 **Community**

Motion Excel is an inclusive and welcoming project. Please read our [Code of Conduct](./CODE_OF_CONDUCT.md) before participating in the community.

**Get Involved:**

- Chat with us and other developers on [Discord](https://discord.gg/your-server).
- Start a discussion on [GitHub Discussions](https://github.com/hritvikgupta/motion-excel/discussions).
- Open a topic on [Stack Overflow](https://stackoverflow.com/questions/tagged/motion-excel) and tag it with `motion-excel`.

You can also find Motion Excel on: [Twitter](https://twitter.com/motionexcel) | [YouTube](#)

---

## 🤝 **Contribution**

We appreciate any kinds of contributing. You can submit [issues or feature requests](https://github.com/hritvikgupta/motion-excel/issues) to us. Please read our [contributing guide](./CONTRIBUTING.md) first.

If you would like to contribute code to Motion Excel, please refer to the [contributing guide](./CONTRIBUTING.md) as well. It would guide you through the process of setting up the development environment and submitting a pull request.

---

## ❤️ **Sponsors**

The growth and development of the Motion Excel project rely on the support of its backers and sponsors. If you are interested in supporting our project, we kindly invite you to consider becoming a sponsor. You can sponsor us through [Open Collective](#).

Thanks to our sponsors, just part of them are listed here because of the space limit, ranking is no particular order:

[![Become a Sponsor](https://img.shields.io/badge/Become%20a%20Sponsor-FF6B6B?style=for-the-badge)](https://opencollective.com/motion-excel)

---

## 📄 **License**

Copyright © 2025 Motion Excel Contributors. All Rights Reserved.

Licensed under the [MIT License](./LICENSE).

---

**Note:** `[1]` These features are provided by the current version of Motion Excel, with more features coming soon.
