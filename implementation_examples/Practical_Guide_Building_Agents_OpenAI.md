# A practical guide to building agents

**Source URL:** https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf
**Date Accessed:** June 02, 2025
**Original Filename:** Practical_Guide_Building_Agents_OpenAI.pdf
**Category:** implementation_examples

## Key Topics Covered:
- Foundational components of AI agents: LLM (Model), external functions (Tools), and explicit guidelines (Instructions).
- Iterative development methodology: starting simple, then increasing complexity.
- Orchestration patterns: single-agent vs. multi-agent systems (Manager or Decentralized patterns).
- Guidance on model selection based on task complexity, latency, and cost.
- Importance of integrating agents with external tools (APIs) to extend capabilities (e.g., connecting to vulnerability scanners, CI/CD systems, SIEMs for DevSecOps).
- Crafting high-quality, unambiguous instructions, potentially derived from existing security playbooks or runbooks for DevSecOps agents.
- Example data tools (querying CVEs, reading SAST/DAST reports) and action tools (opening tickets, blocking merges, deploying patches) for security contexts.
- Common pitfalls: over-reliance on complex rules, tool overload, lack of guardrails.
- Essential guardrails: security/safety classifiers, PII filters, risk-rated tools, rules-based protections, output validation.
- Necessity of human intervention plans, especially for high-risk actions or agent failures.

## Summary:
This OpenAI guide offers practical advice on building AI agents, defined as LLM-powered systems for complex, multi-step tasks. It details an agent's core components—Model (LLM), Tools (external functions), and Instructions (guidelines)—and advocates for iterative development, beginning with single-agent systems and advancing to multi-agent orchestration as needed. The guide places strong emphasis on implementing robust guardrails and human intervention mechanisms to ensure agents operate safely, predictably, and effectively in real-world applications.

## Relevance to Agentic DevSecOps:
This guide is directly applicable for implementing AI agents in DevSecOps. It provides a clear blueprint for structuring DevSecOps agents (LLM + security tools + security policy instructions), integrating them with crucial tools (CI/CD, scanners, SIEMs), and defining their tasks based on established security procedures or playbooks. Most importantly, it stresses the implementation of robust guardrails (e.g., safety classifiers for agent inputs, PII filters, risk-ratings for tools like production deployment APIs) and human oversight mechanisms, which are non-negotiable for agents performing security-sensitive actions within a DevSecOps pipeline, such as code analysis, vulnerability remediation, or incident response.

## Key Takeaways / Actionable Insights:
- **Structured Agent Design:** When building DevSecOps agents, clearly define the LLM, the specific security/DevOps tools the agent can access, and the precise instructions (derived from security policies, compliance requirements, or incident response playbooks) that govern its behavior.
- **Choose Appropriate Orchestration:** Implement single DevSecOps agents for focused tasks (e.g., an agent to triage SAST results and open tickets). For more complex, end-to-end DevSecOps processes (e.g., full incident response), consider multi-agent systems using manager or decentralized patterns involving specialized security agents.
- **Implement Comprehensive Guardrails:** For any DevSecOps agent:
    - Use security classifiers to prevent malicious prompt injection or unintended harmful actions.
    - Implement PII filters if agents handle logs or other potentially sensitive data.
    - Assign risk ratings to tools accessible by the agent; high-risk tools (e.g., those modifying production configurations or code) must trigger human approval loops.
    - Validate agent outputs (e.g., suggested code fixes, configuration changes) to ensure they align with security best practices and do not introduce new risks.
- **Develop Human Intervention Plans:** Define clear escalation paths and intervention criteria for DevSecOps agents, especially for scenarios where an agent fails to resolve a security issue, exhibits unexpected behavior, or proposes actions with potentially high impact (e.g., blocking a critical deployment).
- **Iterate and Prioritize Safety:** Begin with simple DevSecOps agent implementations, rigorously test them in safe environments, and iteratively add capabilities, always prioritizing the safety, security, and reliability of the agent's operations.

## Orbit's Confidence Score (1-5, 5=High):
5
