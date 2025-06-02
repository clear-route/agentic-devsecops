# Practices for Governing Agentic AI Systems

**Source URL:** https://cdn.openai.com/papers/practices-for-governing-agentic-ai-systems.pdf
**Date Accessed:** June 02, 2025
**Original Filename:** Practices_Governing_Agentic_AI_OpenAI.pdf
**Category:** research_papers

## Key Topics Covered:
- Definition of agentic AI systems: AI pursuing complex goals with limited supervision.
- Potential for societal benefit and harm from agentic AI.
- Seven proposed governance practices for safe and accountable operation.
- Shared responsibilities across model developers, system deployers, and users.
- Specific practices: constraining action-space, requiring human approval for critical actions, ensuring legibility of agent activity (e.g., via 'chain-of-thought_ and action ledgers), establishing attributability of actions, implementing automatic monitoring (e.g., via a second AI system), and ensuring interruptibility and maintaining control (e.g., 'off-switches').

## Summary:
This OpenAI paper defines "agentic AI systems" as AI capable of pursuing complex goals with limited supervision, noting their potential for both societal good and harm. It introduces seven initial governance practices aimed at ensuring these systems operate safely and accountably, distributing responsibilities among model developers, system deployers, and users. The authors stress that while these practices provide a "defense-in-depth" strategy for mitigating risks, addressing the wider societal effects of widespread agentic AI will necessitate further governance frameworks, including industry collaboration and societal mitigations.

## Relevance to Agentic DevSecOps:
This paper is exceptionally relevant as agentic DevSecOps systems inherently require robust governance for safe, secure, and ethical operation within critical software development and deployment pipelines. The outlined governance practices—such as constraining agent actions, mandating human approval for sensitive operations, ensuring legibility and attributability of agent activities, implementing automated monitoring, and providing mechanisms for interruptibility—are fundamental design principles for building trustworthy AI agents. These agents might manage code, automate infrastructure changes, or execute security protocols, making such governance essential for mitigating risks like accidental damage, security breaches, or compliance violations within the DevSecOps lifecycle.

## Key Takeaways / Actionable Insights:
- **Constrain Agent Actions:** DevSecOps agents must operate within strictly defined and highly restricted action-spaces, particularly for operations impacting production systems, security configurations, or sensitive data.
- **Mandate Human-in-the-Loop Approval:** For critical DevSecOps tasks (e.g., deploying to production, modifying firewall rules, handling PII), AI agents should require explicit human approval, with clear contextual information provided to avoid 'approval fatigue'.
- **Ensure Legibility and Attributability:** Design DevSecOps agents to provide clear explanations for their decisions and actions (legibility) and maintain detailed audit trails that trace every action back to a responsible principal (attributability). This is vital for debugging, compliance, and security forensics.
- **Implement Automated Monitoring:** Deploy secondary monitoring systems (potentially other AI agents) to continuously review the behavior, reasoning, and actions of primary DevSecOps agents against predefined expectations and security policies.
- **Build in Robust Interruptibility:** DevSecOps agentic systems must include reliable mechanisms for immediate shutdown or manual override ('off-switches') to halt malfunctioning or misbehaving agents and prevent further harm. This includes revoking access credentials promptly.
- **Foster Shared Responsibility for Governance:** The governance of agentic systems in DevSecOps is a collaborative effort. Clear roles and responsibilities must be defined for developers of the agents, teams deploying them, and end-users interacting with them to establish and enforce these safety practices.

## Orbit's Confidence Score (1-5, 5=High):
5
