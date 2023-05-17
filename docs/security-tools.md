---
description: 基于GPT/AIGC/LLM的各类安全工具
---

# Security Tools

目前，将 GPT 应用于网络安全的开源工具和项目尚处于起步阶段。在未来，随着大型语言模型的进一步发展，我们可以期待会有更多的项目和工具涌现，为网络安全领域带来更多的创新和价值。以下是当下一些使用 GPT 进行网络安全研究和实践的开源工具：

### **OpenAI Codex：**

**简介：** 虽然 OpenAI Codex 本身并非专门针对网络安全设计的工具，但它基于 GPT-3.5-turbo 模型，可用于编写、审查和分析代码，包括网络安全相关的代码。您可以利用 Codex 的 API 来构建与网络安全相关的自动化工具，例如自动生成漏洞扫描脚本或辅助渗透测试。

**链接：**[https://openai.com/blog/openai-codex](https://openai.com/blog/openai-codex)


### **BurpGPT：**

**简介：** `burpgpt` 是一个开源项目，结合了 Burp Suite 和 OpenAI 的 GPT-3 模型。Burp Suite 是一款广受欢迎的网络安全工具，主要用于 Web 应用程序的渗透测试。该项目旨在利用 GPT-3 的强大生成能力，为网络安全专业人员提供更智能的安全工具。主要功能如下：

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

**链接：** [https://marketplace.visualstudio.com/items?itemName=MilindPurswani.chatgpt-security-code-analyzer](https://marketplace.visualstudio.com/items?itemName=MilindPurswani.chatgpt-security-code-analyzer)


### **GPT\_Vuln-analyzer**

**简介：** 

这是一个利用openai验证扫描结果的工具，项目展示如何使用AI生成漏洞分析的准确结果，使用python-nmap扫描目标ip，将获取到的信息提交openai获取分析结果。该项目还具有一个CLI和一个GUI界面，它能够进行网络漏洞分析、DNS枚举和子域枚举。

**链接：** [https://github.com/morpheuslord/GPT\_Vuln-analyzer](https://github.com/morpheuslord/GPT\_Vuln-analyzer)


### Navi

**简介：** 一款安全方向的产品，结合了ChatGPT。目前只支持自动化 Nmap 扫描并将输出保存到您指定的文件中。

**链接：** [https://github.com/SSGOrg/Navi](https://github.com/SSGOrg/Navi)


### Nuclei\_GPT

**简介：**这是一个通过Embedding向量Nuclei的模板文档的项目，运行prompt查询工具可以直接对接GPT-3.5编写Nuclei的Yaml文件，安全人员只需要提交相关的Request和Response以及漏洞的描述，就能生成Nuclei的Poc。

**链接：** [https://github.com/sf197/nuclei\_gpt](https://github.com/sf197/nuclei\_gpt)


### Cloud GPT

**简介：** 一款结合GPT的AWS policies漏洞扫描工具，底层原理是使用prompt+profile文件内容直接调用API的原理。

**链接：** [https://github.com/ustayready/cloudgpt](https://github.com/ustayready/cloudgpt)



### Selefra

**简介：** Selefra 的意思是“从基础设施中选择 \*”。它是一种开源策略即代码软件，可为多云和 SaaS 环境提供分析，包括 AWS、GCP、Azure、阿里云、Kubernetes、Github、Cloudflare 和 Slack 等 30 多种服务。通过Selefra，您可以与GPT模型进行对话，GPT模型将分析信息并提供安全、成本和架构检查的相关建议，帮助您更好地管理他们的云资源、增强安全性、降低成本和优化架构设计。

**链接：** [https://github.com/selefra/selefra](https://github.com/selefra/selefra)


### Falco-gpt

**简介：** Falco-gpt是借助OpenAI自动为Falco提供的内核审计事件提供补救措施的工具。

![](https://github.com/mo-xiaoxi/GPTSecurity/blob/main/docs/.gitbook/assets/falco-gpt_example.jpg)

**链接：** [https://github.com/Dentrax/falco-gpt](https://github.com/Dentrax/falco-gpt)


### ChatGPTScan

**简介：** 一个由 ChatGPT 提供支持的白盒代码扫描开源工具

**链接：** [https://github.com/YulinSec/ChatGPTScanner](https://github.com/YulinSec/ChatGPTScanner)


### WPeChatGPT

**简介：** 基于GPT-3.5-Turbo模型、提供二进制文件自动化分析的IDA插件

**链接：** [https://github.com/YulinSec/ChatGPTScanner](https://github.com/YulinSec/ChatGPTScanner)


### PentestGPT

**简介：** 一款基于GPT的自动化渗透测试工具。它建立在 ChatGPT 之上，以交互方式运行，以指导渗透测试人员进行整体进度和具体操作。PentestGPT能够解决简单到中等的 HackTheBox 机器和其他 CTF 挑战。与Auto-GPT 的相比，它有以下几个差异点：1. 在安全测试中使用[Auto-GPT](https://github.com/Torantulino/Auto-GPT)很好，但它并未针对与安全相关的任务进行优化。2. PentestGPT专为通过自定义会话交互进行渗透测试而设计。 3. 目前，PentestGPT不依赖于搜索引擎。

**链接：**[https://github.com/GreyDGL/PentestGPT](https://github.com/GreyDGL/PentestGPT)



### Audit GPT

**简介：** 一款针对区块链安全审计任务进行GPT微调的智能化工具

**链接：** [https://github.com/fuzzland/audit\_gpt](https://github.com/fuzzland/audit\_gpt)



### IATelligence

**简介：** IATelligence 是一个 Python 脚本，它将提取 PE 文件的 IAT 并请求 GPT 以获取有关 API 和 ATT\&CK 矩阵相关的更多信息

**链接：** [https://github.com/fr0gger/IATelligence](https://github.com/fr0gger/IATelligence)



### Codamosa

**简介：** CodaMOSA是CODAMOSA: Escaping Coverage Plateaus in Test Generation with Pre-trained Large Language Models的论文代码，实现了一款结合了OpenAI API的fuzzer，旨在缓解传统fuzz中陷入覆盖率停滞不前的问题。

**链接：** [https://github.com/microsoft/codamosa](https://github.com/microsoft/codamosa)


### cspm-gpt

**简介：** 展示了如何使用 LLM 和 langchain agent、以提问的方式了解云环境的安全状况。

**链接：** [https://github.com/samvas-codes/cspm-gpt](https://github.com/samvas-codes/cspm-gpt)
