---
description: 基于GPT/AIGC/LLM的各类安全工具
---

# Security Tools

目前，将 GPT 应用于网络安全的开源工具和项目尚处于起步阶段。在未来，随着大型语言模型的进一步发展，我们可以期待会有更多的项目和工具涌现，为网络安全领域带来更多的创新和价值。以下是当下一些使用 GPT 进行网络安全研究和实践的开源工具：

### **OpenAI Codex：**

**简介：**虽然 OpenAI Codex 本身并非专门针对网络安全设计的工具，但它基于 GPT-3.5-turbo 模型，可用于编写、审查和分析代码，包括网络安全相关的代码。您可以利用 Codex 的 API 来构建与网络安全相关的自动化工具，例如自动生成漏洞扫描脚本或辅助渗透测试。

**链接：**[https://openai.com/blog/openai-codex](https://openai.com/blog/openai-codex)



### **GPT-3 Sandbox：**

**简介：**GPT-3 Sandbox 是一个可用于快速实验和测试 GPT-3 的在线平台。虽然它同样不是专门为网络安全设计的，但您可以利用该平台为 GPT-3 提供网络安全相关的预设指令（Prompts），从而探索 GPT-3 在网络安全领域的潜在应用。

**链接：**[https://github.com/shreyashankar/gpt3-sandbox](https://github.com/shreyashankar/gpt3-sandbox)



### **BurpGPT：**

**简介：**`burpgpt` 是一个开源项目，结合了 Burp Suite 和 OpenAI 的 GPT-3 模型。Burp Suite 是一款广受欢迎的网络安全工具，主要用于 Web 应用程序的渗透测试。该项目旨在利用 GPT-3 的强大生成能力，为网络安全专业人员提供更智能的安全工具。主要功能如下：

* 自动生成有效的有效负载：根据给定的上下文和目标，利用 GPT-3 自动生成可能导致安全漏洞的有效负载。
* 检测潜在的安全漏洞：使用 GPT-3 分析请求和响应数据，自动识别潜在的安全风险。
* 自动化报告生成：借助 GPT-3，将渗透测试结果整理成易于理解的报告，提高报告编写效率。
* 模糊测试支持：利用 GPT-3 自动生成随机有效负载，用于模糊测试以发现潜在漏洞。

**链接：**[https://github.com/aress31/burpgpt](https://github.com/aress31/burpgpt)



### **ChatGPT Security Code Analyzer:**

**简介：**

一个名为 "ChatGPT Security Code Analyzer" 的 Visual Studio Code 扩展，旨在帮助开发人员在编写代码时自动识别和修复潜在的安全漏洞。通过结合 ChatGPT 大型语言模型的强大生成能力，该扩展提供了实时的安全建议，提高代码安全性并减少开发过程中的安全风险。

ChatGPT Security Code Analyzer 的主要功能如下：

1. 实时安全检查：在编写代码时，自动分析代码并识别潜在的安全漏洞。
2. 智能建议：根据识别到的安全问题，提供相应的修复建议和最佳实践。
3. 多种编程语言支持：支持多种流行的编程语言，包括 JavaScript、Python、Java 等。
4. 集成开发环境：将安全分析功能直接集成到 Visual Studio Code，为开发人员提供无缝的安全检查体验。
5. 易于使用：无需额外配置，只需安装扩展并启用即可开始使用。

**链接：**[https://marketplace.visualstudio.com/items?itemName=MilindPurswani.chatgpt-security-code-analyzer](https://marketplace.visualstudio.com/items?itemName=MilindPurswani.chatgpt-security-code-analyzer)

### **GPT_Vuln-analyzer**
**简介：**

这是一个利用openai验证扫描结果的工具，项目展示如何使用AI生成漏洞分析的准确结果，使用python-nmap扫描目标ip，将获取到的信息提交openai获取分析结果。该项目还具有一个CLI和一个GUI界面，它能够进行网络漏洞分析、DNS枚举和子域枚举。

**链接：** [https://github.com/morpheuslord/GPT_Vuln-analyzer](https://github.com/morpheuslord/GPT_Vuln-analyzer)

