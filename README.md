# Awesome-Web-Developer-Inspection-Devtools

# Awesome Web Developer Inspection & DevTools

> A curated list of top Web Developer Inspection and DevTools platforms — both SaaS/Hosted commercial solutions and open-source alternatives for browser debugging, API testing, and framework inspection.  
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [BrowserStack Developer Tools](#browserstack-developer-tools)
  - [Postman DevTools](#postman-devtools)
  - [Requestly](#requestly)
- [Open-Source Software](#-open-source-software)
  - [Chrome DevTools](#chrome-devtools)
  - [Firefox DevTools](#firefox-devtools)
  - [Safari Web Inspector](#safari-web-inspector)
  - [Edge DevTools](#edge-devtools)
  - [Redux DevTools](#redux-devtools)
  - [React Developer Tools](#react-developer-tools)
  - [Vue Devtools](#vue-devtools)
  - [Hoppscotch](#hoppscotch)
  - [Bruno](#bruno)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Web Developer Inspection and DevTools platforms. These are not open-source but are included as reference points for feature comparison.

### BrowserStack Developer Tools
**Type:** Cloud-based browser and device testing  
BrowserStack provides cloud-hosted real browsers and devices for cross-browser testing and debugging. Its Developer Tools offering includes Live (interactive testing), Automate (Selenium/Playwright/Cypress grid), and App Live for mobile. Integrated debugging lets developers inspect elements, view console logs, and debug network requests on remote browsers without local setup. **Note:** BrowserStack acquired Requestly, whose API client and interceptor remain open-source [citation:8].

### Postman DevTools
**Type:** API development and testing platform  
Postman's desktop and web clients include a DevTools-like console for inspecting API requests, responses, headers, and cookies. Features include request history, environment variables, test scripts, and mock servers. The platform has shifted toward a freemium SaaS model; core API testing is free with limits, while team collaboration and advanced governance require paid plans. Open-source alternatives like Hoppscotch and Bruno provide similar functionality without vendor lock-in.

### Requestly
**Type:** API client and HTTP interceptor  
Requestly (by BrowserStack) provides an open-source API client and HTTP interceptor for modifying headers, redirecting URLs, mocking APIs, and inserting scripts [citation:8]. The interceptor component is open-source, while the broader platform includes team features. It bridges the gap between a browser extension and a full API client, useful for debugging and testing without code changes.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Web Developer Inspection and DevTools. All listed projects offer source code you can use, modify, or build upon.

### Chrome DevTools
**Stack:** JavaScript / C++ (Chromium) | **License:** BSD-3-Clause (Chromium)  
The most widely used browser DevTools, built into Google Chrome and other Chromium-based browsers. Provides Elements (DOM/CSS inspection), Console (JavaScript execution and logging), Sources (debugger with breakpoints), Network (request inspection), Performance (profiling), Memory (heap snapshots), Application (storage inspection), and Lighthouse integration for audits [citation:1]. The DevTools frontend is open-source within the Chromium project, though the browser itself includes proprietary components. The Chrome DevTools Protocol (CDP) is widely used for browser automation and debugging tooling.

### Firefox DevTools
**Stack:** JavaScript / Rust / C++ | **License:** MPL-2.0  
Firefox's built-in developer tools, developed as part of the open-source Firefox codebase under the Mozilla Public License [citation:12]. Offers Inspector, Console, Debugger, Network Monitor, Performance, Memory, Storage, Accessibility Inspector, and Responsive Design Mode. Firefox DevTools is known for its accessibility tooling (contrast checking, accessibility tree inspection) and CSS Grid/Flexbox inspectors. The source is available in the mozilla-central repository.

### Safari Web Inspector
**Stack:** JavaScript / Objective-C / C++ | **License:** Open Source (WebKit)  
Safari's Web Inspector is part of the open-source WebKit project [citation:3]. Provides Elements, Console, Sources, Network, Timelines, Storage, and Audit tabs. The Web Inspector source was open-sourced back into WebKit in 2020 [citation:13]. While Safari itself is proprietary, the Web Inspector tooling is developed in the open WebKit repository. Requires macOS or iOS for full functionality.

### Edge DevTools
**Stack:** JavaScript / C++ (Chromium) | **License:** BSD-3-Clause (Chromium)  
Microsoft Edge is built on Chromium, so its DevTools are largely the same as Chrome DevTools with Microsoft-specific additions . Edge DevTools includes the standard Elements, Console, Sources, and Network panels, plus Microsoft-specific features like 3D View, accessibility testing tools, and integration with VS Code for debugging. The Chromium base is open-source, though Edge includes proprietary Microsoft components. Edge DevTools can be enabled via F12 or the menu .

### Redux DevTools
**Stack:** JavaScript / TypeScript | **License:** MIT  
A browser extension and standalone tool for debugging application state changes, primarily in Redux but also usable with any state-management architecture [citation:5][citation:15]. Provides a time-travel debugger, state diffing, action replay, and a dispatcher for testing actions. The source code is available at `reduxjs/redux-devtools` on GitHub [citation:5]. Available for Chrome and Firefox.

### React Developer Tools
**Stack:** JavaScript / TypeScript | **License:** MIT  
A browser extension that adds React-specific inspection to DevTools [citation:6]. Provides a Components tree showing the React component hierarchy, props, state, and hooks. Includes a Profiler for measuring render performance and identifying unnecessary re-renders. Available for Chrome, Firefox, and Edge. The MIT license permits modification and redistribution.

### Vue Devtools
**Stack:** JavaScript / TypeScript | **License:** MIT  
A browser extension for debugging Vue.js applications . Provides component inspection, Vuex/Pinia state management debugging, event tracking, routing inspection, and performance profiling. The current version (v7) is MIT-licensed and available at `vuejs/devtools` on GitHub . Supports Vue 2 and Vue 3.

### Hoppscotch
**Stack:** TypeScript / Vue | **License:** MIT  
A lightweight, open-source API development ecosystem positioned as an alternative to Postman [citation:9]. Available as a web app, desktop app (Tauri), and PWA. Supports REST, GraphQL, WebSocket, SSE, and MQTT. Features include collections, environments, pre-request scripts, and self-hosting options. Lighter and faster than Postman for quick API testing [citation:9].

### Bruno
**Stack:** JavaScript / Electron | **License:** MIT  
An open-source API client that stores collections as plain files in your repository, enabling Git-based version control and PR reviews for API requests [citation:9]. Supports REST and GraphQL, environments, scripting, and test assertions. Positioned as a Git-friendly alternative to Postman's cloud-synced collections. Offline-first with no account required [citation:9].

---

## 📊 Comparison at a Glance

| Software | License | Type | Browser Integration | API Testing | Framework-Specific | Best For |
|----------|---------|------|---------------------|-------------|-------------------|----------|
| **BrowserStack** | Proprietary | Cloud testing | Remote browsers | ❌ | ❌ | Cross-browser device testing |
| **Postman** | Proprietary | API platform | ❌ | ✅ | ❌ | Full API lifecycle |
| **Requestly** | Open Source (core) | Interceptor | ✅ (extension) | ✅ (client) | ❌ | Request modification + mocking |
| **Chrome DevTools** | BSD-3 (Chromium) | Browser DevTools | ✅ Native | Limited (Network) | ❌ | General web debugging |
| **Firefox DevTools** | MPL-2.0 | Browser DevTools | ✅ Native | Limited | ❌ | Accessibility + CSS inspection |
| **Safari Web Inspector** | Open Source (WebKit) | Browser DevTools | ✅ Native | Limited | ❌ | Apple ecosystem debugging |
| **Edge DevTools** | BSD-3 (Chromium) | Browser DevTools | ✅ Native | Limited | ❌ | Chromium + VS Code integration |
| **Redux DevTools** | MIT | State debugger | ✅ (extension) | ❌ | ✅ (Redux/state) | Time-travel state debugging |
| **React DevTools** | MIT | Component inspector | ✅ (extension) | ❌ | ✅ (React) | React component + profiler |
| **Vue Devtools** | MIT | Component inspector | ✅ (extension) | ❌ | ✅ (Vue) | Vue + Pinia debugging |
| **Hoppscotch** | MIT | API client | ❌ | ✅ | ❌ | Lightweight API testing |
| **Bruno** | MIT | API client | ❌ | ✅ | ❌ | Git-native API collections |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Web Developer Inspection or DevTools tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
