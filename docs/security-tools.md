---
description: 基于GPT/AIGC/LLM的各类安全工具
---

# Security Tools

目前，将 GPT 应用于网络安全的开源工具和项目尚处于起步阶段。在未来，随着大型语言模型的进一步发展，我们可以期待会有更多的项目和工具涌现，为网络安全领域带来更多的创新和价值。以下是当下一些使用 GPT 进行网络安全研究和实践的开源工具：

### **OpenAI Codex：**

**简介：** 虽然 OpenAI Codex 本身并非专门针对网络安全设计的工具，但它基于 GPT-3.5-turbo 模型，可用于编写、审查和分析代码，包括网络安全相关的代码。您可以利用 Codex 的 API 来构建与网络安全相关的自动化工具，例如自动生成漏洞扫描脚本或辅助渗透测试。

**链接：** [https://openai.com/blog/openai-codex](https://openai.com/blog/openai-codex)

### **Ret2GPT：**

**简介：** 主要面向CTF类二进制安全设计的工具：Ret2GPT，通过使用 ChatGPT API + Retdec + Langchain，用户可以通过问答+构造好的Prompt 或者 直接使用以及构造好的Prompt 对 特定二进制文件进行漏洞挖掘 起到一个很好的漏洞挖掘助手的功能!

**链接：** [https://github.com/DDizzzy79/Ret2GPT](https://github.com/DDizzzy79/Ret2GPT)

### **BurpGPT：**

**简介：** `burpgpt` 是一个开源项目，结合了 Burp Suite 和 OpenAI 的 GPT-3 模型。Burp Suite 是一款广受欢迎的网络安全工具，主要用于 Web 应用程序的渗透测试。该项目旨在利用 GPT-3 的强大生成能力，为网络安全专业人员提供更智能的安全工具。主要功能如下：

* 自动生成有效的有效负载：根据给定的上下文和目标，利用 GPT-3 自动生成可能导致安全漏洞的有效负载。
* 检测潜在的安全漏洞：使用 GPT-3 分析请求和响应数据，自动识别潜在的安全风险。
* 自动化报告生成：借助 GPT-3，将渗透测试结果整理成易于理解的报告，提高报告编写效率。
* 模糊测试支持：利用 GPT-3 自动生成随机有效负载，用于模糊测试以发现潜在漏洞。

**链接：**[https://github.com/aress31/burpgpt](https://github.com/aress31/burpgpt)

### **nmap-GPT：**

**简介：** nmap-GPT致力于帮助安全初学者学习如何解决与网络设备开放端口相关的安全问题。首先使用 Nmap 扫描设备，然后利用 OpenAI API 提供每个开放端口特定安全注意事项的提示。

**链接：**[https://github.com/ethanolivertroy/nmap-GPT](https://github.com/ethanolivertroy/nmap-GPT)

### **GPTreport：**

**简介：** 使用chatGPT自动生成漏洞报告

**链接：** [https://github.com/shiyeshu/GPTreport](https://github.com/shiyeshu/GPTreport)

### **SecGPT：**

**简介：** 致力于成为面向网络安全领域的AutoGPT

**链接：** [https://github.com/ZacharyZcR/SecGPT](https://github.com/ZacharyZcR/SecGPT)


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


### **Callisto**

**简介：** 
Callisto是一款智能的自动化二进制漏洞挖掘工具。在Semgrep SAST工具分析源码漏洞的基础上，它使用GPT-3.5-Turbo模型对Semgrep的检测结果进行验证、并且探索并识别更多可能的漏洞。

**链接：** [https://github.com/JetP1ane/Callisto](https://github.com/JetP1ane/Callisto)


### Navi

**简介：** 一款安全方向的产品，结合了ChatGPT。目前只支持自动化 Nmap 扫描并将输出保存到您指定的文件中。

**链接：** [https://github.com/SSGOrg/Navi](https://github.com/SSGOrg/Navi)


### Nuclei\_GPT

**简介：** 这是一个通过Embedding向量Nuclei的模板文档的项目，运行prompt查询工具可以直接对接GPT-3.5编写Nuclei的Yaml文件，安全人员只需要提交相关的Request和Response以及漏洞的描述，就能生成Nuclei的Poc。

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



### beelzebub

**简介：** beelzebub是基于Go语言实现的蜜罐框架，它借助了GPT-3进行系统虚拟化。

**链接：** [https://github.com/mariocandela/beelzebub](https://github.com/mariocandela/beelzebub)


### ChatGPTScanner

**简介：** 一个由 ChatGPT 提供支持的白盒代码扫描开源工具

**链接：** [https://github.com/YulinSec/ChatGPTScanner](https://github.com/YulinSec/ChatGPTScanner)


### WPeChatGPT

**简介：** 基于GPT-3.5-Turbo模型、提供二进制文件自动化分析的IDA插件

**链接：** [https://github.com/WPeace-HcH/WPeChatGPT](https://github.com/WPeace-HcH/WPeChatGPT)

### HackerGPT-2.0

**简介：** HackerGPT-2.0的定位是漏洞赏金猎人的AI助手，配备了广泛前沿的知识数据库，包含相关技术、工具和策略等知识。据开发者称，HackerGPT-2.0在使用过程中会为用户安全地处理每个查询，特别是在移除个人敏感信息后再与OpenAI等外部模块进行交互。

**链接：** [https://github.com/Hacker-GPT/HackerGPT-2.0](https://github.com/Hacker-GPT/HackerGPT-2.0)

### PentestGPT

**简介：** 一款基于GPT的自动化渗透测试工具。它建立在 ChatGPT 之上，以交互方式运行，以指导渗透测试人员进行整体进度和具体操作。PentestGPT能够解决简单到中等的 HackTheBox 机器和其他 CTF 挑战。与Auto-GPT 的相比，它有以下几个差异点：1. 在安全测试中使用[Auto-GPT](https://github.com/Torantulino/Auto-GPT)很好，但它并未针对与安全相关的任务进行优化。2. PentestGPT专为通过自定义会话交互进行渗透测试而设计。 3. 目前，PentestGPT不依赖于搜索引擎。

**链接：**[https://github.com/GreyDGL/PentestGPT](https://github.com/GreyDGL/PentestGPT)



### Audit GPT

**简介：** 一款针对区块链安全审计任务进行GPT微调的智能化工具

**链接：** [https://github.com/fuzzland/audit\_gpt](https://github.com/fuzzland/audit\_gpt)


### ai_cybersecurity_compliance

**简介：** 一款针对网络设备提供安全合规建议的工具，此工具基于GPT-3.5-turbo模型

**链接：** [https://github.com/yzmar4real/ai_cybersecurity_compliance](https://github.com/yzmar4real/ai_cybersecurity_compliance)


### IATelligence

**简介：** IATelligence 是一个 Python 脚本，它将提取 PE 文件的 IAT 并请求 GPT 以获取有关 API 和 ATT\&CK 矩阵相关的更多信息

**链接：** [https://github.com/fr0gger/IATelligence](https://github.com/fr0gger/IATelligence)


### openai-cti-summarizer

**简介：** openai-cti-summarizer是一款基于OpenAI's GPT-3.5和GPT-4 API生成威胁情报总结报告的工具

**链接：** [https://github.com/EC-DIGIT-CSIRC/openai-cti-summarizer](https://github.com/EC-DIGIT-CSIRC/openai-cti-summarizer)


### AutoMSS

**简介：** AutoMSS是基于AI Agent实现的针对安全事件自动化分析研判的安全托管运营系统。
为了能够自动化的对安全事件进行分析研判，我们结合LLM以及AI Agent通过一下几个步骤，来提供安全人员的研判效率。
首先，从开始部分输入安全事件记录， 由经过微调后的Chatglm2-6B的微调模型对该事件进行分类。
然后，根据分类后的结果，使用对应的prompt模板对ChatGLM-pro大模型进行请求，大模型根据向量库中的知识以及自身的逻辑推理能力，生成该类事件的分析研判流程。
接着，Agent 根据事件的分析研判流程通过调用工具、访问大模型、请求网络等方式来对该事件进行研判。
最后，根据分析的结果输出研判结论以及形成对应的研判报告。

**链接：** [https://github.com/1700111005/autoMSS](https://github.com/1700111005/autoMSS)



### Codamosa

**简介：** CodaMOSA是CODAMOSA: Escaping Coverage Plateaus in Test Generation with Pre-trained Large Language Models的论文代码，实现了一款结合了OpenAI API的fuzzer，旨在缓解传统fuzz中陷入覆盖率停滞不前的问题。

**链接：** [https://github.com/microsoft/codamosa](https://github.com/microsoft/codamosa)


### cspm-gpt

**简介：** 展示了如何使用 LLM 和 langchain agent、以提问的方式了解云环境的安全状况。

**链接：** [https://github.com/samvas-codes/cspm-gpt](https://github.com/samvas-codes/cspm-gpt)


### gpt3-and-cybersecurity

**简介：** Sophos使用GPT-3进行命令分析和垃圾文本监测。

**链接：** [https://github.com/sophos/gpt3-and-cybersecurity](https://github.com/sophos/gpt3-and-cybersecurity)


### CalypsoAI Moderator

**简介：** CalypsoAI Moderator针对数据丢失、恶意代码、越狱和幻觉等安全风险进行防护。

**链接：** [https://calypsoai.com/](https://calypsoai.com/)


### garak

**简介：** garak检查大语言模型是否存在特定的脆弱性，这些脆弱性的探测可以由[PromptInjection](https://github.com/agencyenterprise/promptinject)框架实现。garak可以集成模型幻觉、数据泄露、提示词注入、错误信息、带毒生成、越狱等脆弱性的探测。\
garak checks if an LLM will fail in an way we don't necessarily want. garak probes for hallucination, data leakage, promp injection, misinformation, toxicity generation, jailbreaks, and many other weaknesses. \
![](https://camo.githubusercontent.com/04ada429886541bce6432d11e282f0a8483a0fb74573519cb2230e85a6d7faaf/68747470733a2f2f692e696d6775722e636f6d2f564b41463569662e706e67)
**链接：** [https://github.com/leondz/garak](https://github.com/leondz/garak)

### LLMFuzzer 

**简介：** LLMFuzzer是用于寻找和利用AI系统漏洞的框架，未来的开发路线是适配各种LLM API、集成不同的模糊测试策略。

![](https://user-images.githubusercontent.com/1796080/239725603-a143897d-383c-4ed9-8b2f-65f4cdc5aa63.png)
![](https://user-images.githubusercontent.com/1796080/239700414-71b006df-706c-43f6-acd1-49646dbcb0e5.jpg)

**链接：** [https://github.com/mnns/LLMFuzzer](https://github.com/mnns/LLMFuzzer)

### PsychoEvals 

**简介：** 以MBTI人格评估、提示词注入检测为基础的LLM安全评估轻量框架

**链接：** [https://github.com/NextWordDev/psychoevals](https://github.com/NextWordDev/psychoevals)
 

### rebuff 

**简介：** 提示词注入检测工具

**链接：** [https://github.com/protectai/rebuff](https://github.com/protectai/rebuff)


### ai-goat 

**简介：** 面向带缺陷的LLM的CTF挑战

**链接：** [https://github.com/dhammon/ai-goat](https://github.com/dhammon/ai-goat)


### promptbench 

**简介：** 大语言模型针对对抗性提示词的健壮性评估框架

**链接：** [https://github.com/microsoft/promptbench](https://github.com/microsoft/promptbench)

### ai网络安全助手

**简介：** 围绕安全从业人员在日常工作中常需要的能力进行开发，通过AI插件的方式连接专业工具和产品 \

**链接：** [https://www.secasst.com/](https://www.secasst.com/)
