---
layout:     post
title:      "第69期|GPTSecurity周报"
date:       2024-10-09 10:00:00
author:     "安全极客"
header-img: "img/post-bg-unix-linux.jpg"
catalog: true
tags:
    - Security
    - AIGC
    - GPTSecurity周报
---


![这是一张图片](https://www.gptsecurity.info/img/in-post/0807/01.jpg)

GPTSecurity是一个涵盖了前沿学术研究和实践经验分享的社区，集成了生成预训练Transformer（GPT）、人工智能生成内容（AIGC）以及大语言模型（LLM）等安全领域应用的知识。在这里，您可以找到关于GPT/AIGC/LLM最新的研究论文、博客文章、实用的工具和预设指令（Prompts）。现为了更好地知悉近一周的贡献内容，现总结如下。

## Security Papers

#### AutoSafeCoder：通过静态分析和模糊测试保障LLM代码生成安全的多智能体框架

简介：最近，大语言模型（LLM）的自动代码生成技术取得了重大进展，推动着我们向完全自动化安全软件开发的目标迈进了一步。然而，现有的方法多依赖单一智能体进行代码生成，这种方式难以生成安全且无漏洞的代码。传统基于 LLM 的程序合成主要关注功能正确性，常常忽视运行时的动态安全隐患。为解决这些问题，研究者提出了 AutoSafeCoder——一个多智能体框架，该框架利用 LLM 驱动的智能体进行代码生成、漏洞分析以及通过持续协作进行安全增强。此框架由三个智能体组成，分别是负责代码生成的编码智能体、识别漏洞的静态分析智能体以及使用基于变异的模糊测试方法进行动态测试以检测运行时错误的模糊测试智能体。研究者的贡献在于通过在代码生成过程中整合动态和静态测试，以迭代的方式提高 LLM 生成代码的安全性。基于 SecurityEval 数据集的实验结果表明，与基准 LLM 相比，代码漏洞减少了 13%，且未对功能性造成影响。

*链接：https://arxiv.org/abs/2409.107372*.

#### PROMPTFUZZ：利用模糊测试技术对大语言模型中的提示注入进行鲁棒性测试

简介：大语言模型（LLMs）虽在各种应用中广泛使用，但其安全性和可靠性因提示注入攻击而引发担忧。提示注入攻击可通过恶意提示覆盖模型原始指令操纵生成文本，确保 LLM 抵御此类攻击的鲁棒性对其在现实世界尤其是关键任务中的部署至关重要。

研究者提出新颖测试框架 PROMPTFUZZ，利用模糊测试技术系统性评估 LLM 抵御提示注入攻击的鲁棒性。该框架受软件模糊测试启发，分为准备和重点两个阶段。准备阶段选择有潜力的初始种子并收集少量示例；重点阶段利用收集的示例生成多样化高质量提示注入，能发现更多 LLM 漏洞。在实际竞赛中，部署 PROMPTFUZZ 生成的攻击提示后，在 4000 多名参与者中获得第七名，仅用时 2 小时。此外，研究者还构建数据集用于微调 LLM 以增强其抗攻击鲁棒性，即便微调后，PROMPTFUZZ 仍能发现漏洞。

总之，研究者的工作突出了有效测试工具的关键需求，提供了实用框架用于评估和提高 LLM 抵御提示注入攻击的鲁棒性，强调了对 LLM 进行鲁棒性测试的重要性。

*链接：https://arxiv.org/abs/2409.14729*

#### 针对大语言模型的有效且具有规避性的模糊测试驱动越狱攻击

简介：近年来，研究者发现大语言模型（LLMs）虽然在多项任务中表现出色，但仍然容易遭受越狱攻击，攻击者通过提示设计误导模型生成有害内容。现有越狱方法依赖手动设计模板，扩展性差，或生成语义不连贯的提示，容易被检测到。为解决这些问题，研究者提出了一种自动化黑盒越狱攻击框架，通过结合黑盒模糊测试与定制化设计，克服了传统方法的局限性。

该框架无需手动设计模板，从空种子池开始，依靠三个新型问题相关变异策略生成语义连贯且简短的提示。同时，研究者设计了两级评判模块，精确识别成功的越狱攻击。在对7个主流LLMs的评估中，该方法在GPT-3.5 Turbo、GPT-4和Gemini-Pro上的攻击成功率分别超过90%、80%和74%，相比现有基线提升了60%以上。此外，提示长度大幅缩短，语义连贯性得到保持，且对最先进的防御措施具有较强鲁棒性。

*链接：https://arxiv.org/abs/2409.14866*

#### 攻击图谱：从实践者的角度看生成式人工智能红队测试中的挑战与陷阱

简介：随着生成式人工智能，特别是大语言模型（LLMs）逐渐融入生产应用，新的攻击面和漏洞不断出现，进一步增强了对自然语言和多模态系统中对抗性威胁的关注。在这一背景下，红队测试在主动识别系统弱点方面变得尤为重要，而蓝队则专注于抵御这些对抗性攻击。尽管学术界对生成式人工智能的对抗风险日益重视，但针对实践者在实际环境中评估和缓解这些挑战的指导仍显不足。

为此，研究者提出了以下贡献：(1) 对保护生成式人工智能的红队和蓝队策略进行了实用性检验；(2) 识别了防御开发和评估过程中面临的关键挑战及未解问题；(3) 提出了“攻击图谱”，这是一个直观的框架，为分析单轮输入攻击提供了实用的方法，使其成为实践者的重要参考工具。此项研究旨在弥合学术见解与生成式人工智能系统保护的实际安全措施之间的差距，以增强对抗性威胁的应对能力。

*链接：https://arxiv.org/abs/2409.15398*

#### LSAST — 通过LLM支持的静态应用安全测试增强网络安全

简介：在快速发展的网络安全领域，研究者们认识到大语言模型（LLMs）在分析软件代码方面发挥着至关重要的作用，持续提升其性能。本文提出了一种创新的漏洞扫描方法，通过将保守的静态应用安全测试（SAST）扫描器与LLM能力相结合，构建了LSAST（LLM支持的静态应用安全测试）框架。该方法显著增强了LLM在漏洞扫描中的性能，确立了该领域的新标准。

研究者们对LSAST的效率进行了基准测试，并将其结果与最先进的LLM进行了对比分析。同时，本文还讨论了LLM在漏洞扫描过程中存在的固有缺陷，包括对静态训练数据集的依赖，导致最新漏洞的遗漏，以及将代码发送至第三方LLM提供商所引发的隐私问题。为解决这些挑战，研究者们采用了一个开源LLM，以确保用户隐私，并提出了一种新颖的方法来收集相关的漏洞信息，从而为LLM提供最新的知识。这一工作为提升网络安全中的漏洞扫描能力提供了有效的解决方案。

*链接：https://arxiv.org/abs/2409.15735*

#### APILOT：通过避开过时API陷阱，导航大语言模型生成安全代码

简介：随着大语言模型（LLMs）的快速发展，研究者们发现其应用领域已扩展至代码辅助等多个方面。然而，LLMs的庞大规模使得训练过程非常耗费资源和时间，频繁的再训练或更新变得不切实际。因此，时效性数据可能会过时，从而在时效性任务中误导LLMs。例如，每天都会在各种程序中发现新的漏洞，如果不更新知识，LLMs可能会不小心生成包含这些新发现漏洞的代码。当前的策略，如提示工程和微调，并未有效解决这一问题。

为了解决这一挑战，研究者提出了名为APILOT的解决方案，该方案维护了一个实时、快速可更新的过时API数据集。此外，APILOT利用增强生成方法，通过该数据集引导LLMs生成安全的、版本感知的代码。研究者们进行了全面评估，以衡量APILOT在减少七种不同最先进LLMs中过时API推荐的有效性。评估结果显示，APILOT平均可以减少89.42%的过时代码推荐，且性能开销有限。值得注意的是，APILOT在增强安全性的同时，还提高了LLMs生成代码的可用性，平均提升了27.54%。这一研究成果突显了APILOT在当代软件开发环境中同时提升代码建议的安全性和实用性的双重能力。

*链接：https://arxiv.org/abs/2409.16526*


![secgeek-foot](https://www.gptsecurity.info/img/secgeek-foot.png)
