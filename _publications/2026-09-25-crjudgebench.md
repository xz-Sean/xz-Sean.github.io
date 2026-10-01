---
title: "CRJudgeBench: Can AI Detect Plausible but Invalid Code Reviews?"
collection: publications
category: preprints
permalink: /publication/crjudgebench
excerpt: 'A benchmark of 1,199 instances for judging the technical trustworthiness of code-review comments, plus Sentinel, a repository-grounded agentic judge.'
date: 2026-09-25
authors: 'Yue Pan, Jiawei Li, Ziyuan Zhang, <b>Xiangxin Zhao</b>, He Ye'
venue: 'Manuscript'
status: 'Under review'
citation: 'Yue Pan, Jiawei Li, Ziyuan Zhang, <b>Xiangxin Zhao</b>, He Ye. (2026). &quot;CRJudgeBench: Can AI Detect Plausible but Invalid Code Reviews?&quot; Under review.'
---

**Abstract.** Large language models can generate plausible code-review comments, but such comments may contain technically incorrect claims that mislead developers. We study technical trustworthiness judgment: determining whether a review comment's core technical claims are correct and applicable to the reviewed code in its repository context. Existing code-review benchmarks primarily evaluate review generation, issue discovery, or general comment quality, but do not directly assess whether an agent can determine the technical trustworthiness of an individual review comment. To fill this gap, we introduce CRJudgeBench, a benchmark of 1,199 instances constructed from real pull requests and expert-verified perturbations, covering both trustworthy and plausible but untrustworthy comments. We further present Sentinel, a repository-grounded agentic judge that actively gathers code evidence to verify review comments before making judgments. Starting from Qwen3-Coder-30B-A3B-Instruct, Sentinel is trained on the CRJudgeBench training split through iterative action-level learning from a privileged teacher. On the 359-instance CRJudgeBench test set, Sentinel achieves 76.60% accuracy, outperforming GLM-5.3 by 6.13 percentage points and its base model by 19.78 points. These results show that even state-of-the-art general-purpose LLMs struggle to identify untrustworthy comments, while iterative action-level learning substantially improves the accuracy of repository-grounded trustworthiness judgments.
