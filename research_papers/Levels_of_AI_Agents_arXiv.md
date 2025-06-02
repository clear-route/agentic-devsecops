# Levels of AI Agents: from Rules to Large Language Models

**Source URL:** https://arxiv.org/pdf/2405.06643
**Date Accessed:** June 02, 2025
**Original Filename:** Levels_of_AI_Agents_arXiv.pdf
**Category:** research_papers

## Key Topics Covered:
- A proposed five-level classification system for AI agents (L0: No AI, L1: Rule-based, L2: IL/RL-based AI, L3: LLM-based Interactive Single Agent, L4: LLM-based Autonomous Single Agent, L5: LLM-based Multi-Agent Society).
- The increasing role and capabilities of Large Language Models (LLMs) in enabling higher-level agentic behavior.
- Core agent components: perception, action, reasoning, decision-making, memory, reflection, and learning.
- Emergent abilities in LLM-based agents, including planning, autonomous learning, generalization, and collaborative behaviors.
- Limitations of current agent technologies, especially LLM-based ones (e.g., transparency, reliability, hallucination, training challenges).

## Summary:
This paper introduces a novel classification system for AI agents, analogous to the SAE levels for autonomous driving, categorizing them from L0 (no AI) to L5 (superhuman multi-agents). It emphasizes the pivotal role of Large Language Models (LLMs) in advancing agents to higher levels of capability, endowing them with reasoning, planning, memory, reflection, autonomous learning, generalization, and collaborative skills. The paper discusses how these different agent levels perceive environments, make decisions, and execute actions, highlighting their emergent abilities and potential contributions towards Artificial General Intelligence (AGI).

## Relevance to Agentic DevSecOps:
This paper is highly relevant for agentic DevSecOps as it provides a structured framework (L0-L5) to conceptualize, design, and evaluate the sophistication of AI agents applied to security tasks. It helps define what capabilities can be expected from DevSecOps agents at each level—from simple rule-based automation of security checks (L1-L2) to interactive LLM-driven agents that can analyze vulnerabilities and suggest remediations (L3), to autonomous agents that can learn and adapt security postures (L4), and finally to collaborative multi-agent systems that holistically manage the secure software development lifecycle (L5). Understanding these levels and the associated LLM capabilities (and limitations) is crucial for setting realistic goals and designing effective agentic DevSecOps solutions.

## Key Takeaways / Actionable Insights:
- **Framework for DevSecOps Agent Design:** Utilize the L0-L5 classification as a roadmap for developing agentic DevSecOps capabilities, incrementally increasing autonomy and intelligence.
- **Leverage LLMs for Advanced Agents:** Incorporate LLM capabilities such as reasoning (e.g., Chain-of-Thought), memory, reflection, and autonomous learning to build sophisticated DevSecOps agents (L3 and above) capable of complex analysis and decision-making.
- **Address LLM Limitations in Security Contexts:** Be mindful of LLM limitations like lack of transparency, potential unreliability, and hallucination. For DevSecOps, ensure mechanisms for explainability (e.g., logging agent reasoning), validation (e.g., human oversight for critical actions), and reliability (e.g., using Retrieval Augmented Generation or specialized tools to ground LLM responses).
- **Consider Multi-Agent Architectures:** For comprehensive DevSecOps coverage, explore multi-agent systems (L5) where specialized AI agents collaborate on different security functions (e.g., threat intelligence analysis, code vulnerability scanning, automated policy enforcement, incident response orchestration).
- **Focus on Core Agent Components:** Ensure DevSecOps agents have robust perception (e.g., ingesting data from security tools, logs, code repositories), action (e.g., triggering scans, creating tickets, applying patches through APIs), and decision-making capabilities appropriate for their defined level and tasks.
- **Progressive Autonomy:** Design agentic DevSecOps systems with increasing levels of autonomy, starting with human-in-the-loop systems and gradually moving towards more autonomous operations as trust and reliability are established.

## Orbit's Confidence Score (1-5, 5=High):
5
