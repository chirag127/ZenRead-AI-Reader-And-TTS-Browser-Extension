# ZenRead: AI-Powered Distraction-Free Reader Browser Extension

ZenRead is an AI-powered browser extension designed to provide a seamless and distraction-free reading experience. It leverages advanced AI, including Google Gemini, to offer features like intelligent content extraction, text-to-speech functionality, and enhanced readability, all while prioritizing user privacy.

## Project Overview

This repository hosts the source code for the ZenRead browser extension. It is built with modern web technologies and integrates cutting-edge AI to transform how you consume online content. As a privacy-focused, open-source project, ZenRead aims to be a reliable and user-centric tool for readers worldwide.

## 🤖 AI Agent Directives

<details>
<summary>View AI Agent Directives</summary>

### 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

### 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**. This repository, `ZenRead-AI-Powered-Distraction-Free-Reader-Browser-Extension`, is a browser extension.

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript) - *This repository's scenario.***
    *   **Stack:** This project leverages **TypeScript 6.x (Strict)**. The build system uses **Vite 7 (Rolldown)**. For native desktop integration and cross-platform capabilities, **Tauri v2.x** is employed. For browser extension development, the **WXT (Web Extension Tooling)** framework is utilized, ensuring compatibility across Chromium-based browsers and Firefox.
    *   **State Management:** Standardized Signals API for efficient and predictable state updates across the extension.
    *   **UI/UX:** **Tailwind CSS v4** for rapid, utility-first styling. **Lit 3.x** for highly performant, framework-agnostic web components.
    *   **Linting/Formatting:** **Biome** is the primary tool for ultra-fast code linting and formatting, ensuring code quality and consistency.
    *   **Testing:** **Vitest** for fast unit and component testing. **Playwright** for comprehensive end-to-end (E2E) testing across different browser environments.
    *   **Architecture:** Feature-Sliced Design (FSD) principles are applied to maintain modularity, scalability, and maintainability.
    *   **AI Integration:** Deeply integrated with **Google Gemini API** (`gemini-3-pro` by default) for intelligent content summarization, extraction, and text-to-speech enhancements. Prioritize modular design, clear API contracts, and robust error handling for all AI model interactions.

### 4. DEVELOPMENT & DEPLOYMENT STANDARDS
*   **Version Control:** Git via GitHub. Branching strategy: Gitflow (main, develop, feature branches).
*   **CI/CD:** GitHub Actions (using `ci.yml`) for automated builds, testing, linting, and deployment pipelines.
*   **Package Management:** npm/yarn for JavaScript dependencies.
*   **Code Quality:** Strict linting and formatting via Biome. Comprehensive testing suite via Vitest and Playwright.
*   **Security:** Adherence to OWASP Top 10 for Web Applications and Browser Extensions. Regular dependency vulnerability scanning. Secrets managed via GitHub Secrets.
*   **API Security:** API keys and sensitive data MUST be securely stored and accessed. Never hardcode credentials. Use environment variables or secure storage mechanisms.

### 5. TESTING PROTOCOL
*   **Unit Tests:** Vitest. Focus on isolated component and function logic.
*   **Integration Tests:** Vitest. Test interactions between modules and services.
*   **End-to-End (E2E) Tests:** Playwright. Simulate user interactions across the full extension lifecycle in a real browser environment.
*   **Test Coverage:** Aim for >85% coverage. Use `codecov.io` for reporting.

### 6. ARCHITECTURE PRINCIPLES
*   **SOLID:** Adhere strictly to Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, and Dependency Inversion principles.
*   **DRY (Don't Repeat Yourself):** Eliminate redundant code through abstraction and modularization.
*   **YAGNI (You Ain't Gonna Need It):** Implement only necessary features; avoid over-engineering.
*   **FSD (Feature-Sliced Design):** Structure the codebase into layers and slices for better maintainability and scalability.
*   **Modular Design:** Ensure components and services are loosely coupled and highly cohesive.

### 7. PRIVACY & SECURITY MANDATES
*   **Data Minimization:** Collect only the data essential for functionality.
*   **Transparency:** Clearly document data collection and usage policies.
*   **Secure AI Integration:** Ensure all interactions with the Gemini API are authenticated and authorized. Sanitize inputs and outputs to prevent prompt injection or data leakage.
*   **Local Processing:** Prioritize client-side processing wherever feasible to minimize data transfer.
*   **No Tracking:** Avoid unnecessary third-party trackers or analytics.

</details>

## 🚀 Getting Started

### Prerequisites

*   Node.js v20+ (or via uv)
*   npm or yarn
*   Google Gemini API Key (for AI features)

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/ZenRead-AI-Powered-Distraction-Free-Reader-Browser-Extension.git
    cd ZenRead-AI-Powered-Distraction-Free-Reader-Browser-Extension
    

2.  **Install Dependencies:**
    bash
    npm install
    # or
    yarn install
    

3.  **Configure Environment Variables:**
    Create a `.env` file in the root directory (ensure it's added to `.gitignore`):
    
    GOOGLE_API_KEY=YOUR_GEMINI_API_KEY
    

### Development

Run the development server for live preview:

bash
# For Vite development server
npm run dev
# or
yarn dev


### Building for Production

Compile the extension for deployment:

bash
# Build for production
npm run build
# or
yarn build


This will generate optimized builds in the `dist` directory, ready for packaging as a browser extension.

## 🛠️ Tech Stack

*   **Language:** TypeScript 6.x (Strict)
*   **Build Tool:** Vite 7 (Rolldown)
*   **Extension Framework:** WXT (Web Extension Tooling)
*   **UI Framework:** Lit 3.x
*   **Styling:** Tailwind CSS v4
*   **State Management:** Signals API
*   **Linting/Formatting:** Biome
*   **Testing:** Vitest (Unit/Component), Playwright (E2E)
*   **AI Integration:** Google Gemini API (`gemini-3-pro`)
*   **Runtime:** Node.js (for build tools), Browser APIs

## 📜 Architecture

ZenRead follows the **Feature-Sliced Design (FSD)** pattern for robust organization and maintainability.

mermaid
graph TD
    subgraph Core
        A[App Entrypoints] --> B(Shared Features)
        B --> C(UI Components)
        C --> D(API Services)
    end

    subgraph Features
        E[Content Extraction] --> B
        E --> C
        E --> D
        F[Text-to-Speech] --> B
        F --> C
        F --> D
        G[Reading Mode] --> B
        G --> C
        G --> D
        H[AI Integration] --> D
    end

    subgraph Pages/Views
        I[Popup UI] --> E
        I --> F
        I --> G
        J[Options Page] --> E
        J --> F
        J --> G
    end

    A --> I
    A --> J


## 🤝 Contributing

Contributions are welcome! Please read our **[CONTRIBUTING.md](https://github.com/chirag127/ZenRead-AI-Powered-Distraction-Free-Reader-Browser-Extension/blob/main/.github/CONTRIBUTING.md)** for details on how to submit pull requests, report bugs, and suggest features.

## ⚖️ License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license. See the **[LICENSE](https://github.com/chirag127/ZenRead-AI-Powered-Distraction-Free-Reader-Browser-Extension/blob/main/LICENSE)** file for more details.

## 🛡️ Security

Security is a top priority. Please refer to our **[SECURITY.md](https://github.com/chirag127/ZenRead-AI-Powered-Distraction-Free-Reader-Browser-Extension/blob/main/.github/SECURITY.md)** for information on reporting vulnerabilities and our security practices.
