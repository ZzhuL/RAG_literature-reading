# 🧾 Thesis Title
**MEDAGENTS: Large Language Models as Collaborators for Zero-shot Medical Reasoning**

---

## 📖 论文基本信息
- **作者**: Xiangru Tang, Anni Zou, Zhuosheng Zhang, Ziming Li, Yilun Zhao, Xingyao Zhang, Arman Cohan, Mark Gerstein  
- **发表会议**: Findings of the Association for Computational Linguistics: ACL 2024  
- **期刊**: ACL 2024 Findings  
- **链接**: [论文链接](https://github.com/gersteinlab/MedAgents)

---

## 📝 论文摘要
该论文探讨了如何在没有额外训练的前提下，利用大型语言模型（LLMs）进行医学领域的零样本推理任务。作者提出了一个名为 **MedAgents** 的多智能体协作框架，模拟医学专家之间的角色扮演讨论，以增强LLMs在医学问答任务中的推理能力。实验表明该方法在九个医学数据集上表现优异，超过了传统的提示词策略和链式推理方法。

---

## 🧠 研究目标和问题
- **论文旨在**：  
  构建一个无需训练的多智能体协作框架，以提升LLM在医学推理任务中的表现。
- **提出问题**：  
  1. LLM在医学领域的推理能力受限，能否通过模拟多专家协作进行弥补？  
  2. 多轮协商是否能够改善模型的准确性与解释性？  
  3. 如何在零样本设置下更好地挖掘LLM的隐性医学知识？

---

## 📊 方法概述
- **框架**：  
  MEDAGENTS 包含五个阶段：
  1. **专家召集**：LLM模拟不同医学领域专家；
  2. **分析提出**：每位专家独立分析问题或选项；
  3. **报告汇总**：将各方观点汇总为初始报告；
  4. **协作讨论**：多轮讨论与投票，修改报告直至达成共识；
  5. **决策制定**：最终基于共识报告得出答案。

- **评估方法**：  
  在9个医学相关数据集上进行零样本实验，与Zero-shot、Few-shot、CoT、Self-Consistency等方法进行比较。

---

## 🔬 实验与结果
- **数据集**：
  - MedQA（USMLE医学执照考试）
  - MedMCQA（印度AIIMS/NEET医学考试）
  - PubMedQA（文献摘要问答）
  - MMLU中6个医学子任务（解剖学、临床医学、医学遗传学等）

- **结果**：
  - MEDAGENTS在GPT-4零样本设置下取得了最优结果，平均准确率86.7%，显著优于传统方法；
  - 相比Zero-shot C
