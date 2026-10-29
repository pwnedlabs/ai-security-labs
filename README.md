# AI Security Training: Hands-On Labs, Tools and Courses for LLM and Agent Security

AI systems are much more than a chatbot. Much of the risk sits in what surrounds the model: the system prompt, the documents a RAG pipeline retrieves, the tools an agent can call and the permissions those tools carry. This repository collects the hands-on labs, tools and courses we recommend for learning to attack and defend LLM applications, RAG pipelines and agents.

> **Key Takeaway:** Prompt injection becomes a real security problem the moment untrusted content can reach a model that is allowed to act, whether that content arrives in a user message, a retrieved document, a ticket or a web page. The training worth your time makes you exploit that against a live application, follow the injection through to tool calls and data access, and then build the controls and detections that would have stopped it.

Maintained by [Pwned Labs](https://pwnedlabs.io). Our own training is listed alongside the community projects we rate, and marked so you know which is which. Pull requests are welcome.

## Hands-on labs and challenges

| Lab | Type | What you practice |
|---|---|---|
| [Gandalf](https://gandalf.lakera.ai) from Lakera | Hosted, free | Direct prompt injection against progressively stronger defenses. A popular first taste of AI hacking, and still a good one. |
| [AI Red Teaming Playground Labs](https://github.com/microsoft/AI-Red-Teaming-Playground-Labs) from Microsoft | Self-hosted, free | The challenges Microsoft uses in its own AI red teaming trainings, including credential extraction and multi-turn attacks. |
| [Damn Vulnerable LLM Agent](https://github.com/ReversecLabs/damn-vulnerable-llm-agent) from Reversec | Self-hosted, free | Prompt injection against a tool-using agent, where the injection turns into actions. |
| [Web LLM attacks](https://portswigger.net/web-security/llm-attacks) from the PortSwigger Web Security Academy | Hosted, free | LLM features inside web applications, including excessive agency, insecure output handling and indirect prompt injection. |
| [Prompt Airlines](https://promptairlines.com) from Wiz | Hosted, free | A CTF where you talk a customer service bot into handing over a free (fictional) airline ticket. |
| [Pwned Labs AI security labs](https://pwnedlabs.io/explore) (ours) | Hosted | AI and agentic attack scenarios in live environments, next to the cloud labs they often depend on. |

## Tools for AI red teaming

- [garak](https://github.com/NVIDIA/garak) from NVIDIA. An LLM vulnerability scanner.
- [PyRIT](https://github.com/microsoft/PyRIT) from Microsoft. The Python Risk Identification Tool for generative AI.
- [promptfoo](https://github.com/promptfoo/promptfoo). Testing and red teaming for prompts, agents and RAG.

## References

- [OWASP Top 10 for LLM Applications](https://genai.owasp.org). The shared vocabulary for LLM risks such as prompt injection, sensitive information disclosure and excessive agency.
- NIST AI 600-1, the generative AI profile of the NIST AI Risk Management Framework, for governance and policy work.

## Courses and certifications

| Course | Format | Focus |
|---|---|---|
| [AI Systems Attack and Defense Bootcamp (AISRTP)](https://pwnedlabs.io/bootcamps/aisrtp-bootcamp) from Pwned Labs (ours) | On-demand, hands-on exam | Direct and indirect prompt injection, RAG poisoning, tool and agent abuse, and MCP and CI/CD agent attack paths, with the defenses for each. No prior AI security experience or Python required. |
| OffSec AI-300 (OSAI) | Advanced | Offensive testing of LLM applications, agents and RAG, validated by the OSAI exam. Assumes strong penetration testing skills. |
| [SANS SEC411: AI Security Principles and Practices](https://www.sans.org/cyber-security-courses/ai-security-principles-practices) | Self-paced with labs | GenAI and LLM defense for practitioners. |
| DeepLearning.AI Red Teaming LLM Applications | Short course, free | A gentle introduction to manual and automated red teaming of chatbots. |

Check each provider for current dates and pricing.

If you are on the blue team, our [PromptStorm](https://pwnedlabs.io/cyber-ranges/promptstorm) cyber range puts defenders inside an AWS breach that abuses AI and LLM workflows (ours, enterprise).

## A path through the list

1. Learn how LLM applications are put together: system prompts, retrieval, tools and agents, and every place untrusted input gets in.
2. Practice direct prompt injection on Gandalf, then move on to indirect injection through documents and web content.
3. Attack an agent that has tools, using Damn Vulnerable LLM Agent or the Microsoft playground, and watch an injection become an action.
4. Automate what you have learned with garak, PyRIT or promptfoo.
5. Map your findings to the OWASP Top 10 for LLM Applications and design the controls and detections that would have caught them.
6. Prove it in a hands-on exam that requires an end-to-end exploitation chain.

## Contributing

Open a pull request with the resource, a one-line description and whether it is free. We only list resources that are live and hands-on, and if a link breaks we will fix it or take it out.
