# 🐨CoALA: Awesome Language Agents
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)  [![PR Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)](https://github.com/ysymyth/awesome-language-agents/pulls)

![teaser](CoALA.png)


A compilation of language agents using the **Cognitive Architectures for Language Agents (🐨CoALA)** framework. 
- CoLLA Paper: https://arxiv.org/abs/2309.02427
- CoLLA BibTex file with 300+ related citations: [CoALA.bib](CoALA.bib)
- CoLLA BibTex citation if you find our work/resources useful:
```bibtex
@misc{sumers2023cognitive,
      title={Cognitive Architectures for Language Agents}, 
      author={Theodore Sumers and Shunyu Yao and Karthik Narasimhan and Thomas L. Griffiths},
      year={2023},
      eprint={2309.02427},
      archivePrefix={arXiv},
      primaryClass={cs.AI}
}
```

## 🐨CoALA Overview
CoLLA neatly specifies a langauge agent starting with its **action space**, which has 2 parts:
* External actions to interact with external environments (**grounding**)
* Internal actions to interact with internal memories (**reasoning**, **retrieval**, **learning**)
  * A language agent has a short-term working memory and several long-term memories (episodic for experience, semantic for knowledge, procedural for code/LLM)
  * **Reasoning** = update working memory (with LLM)
  * **Retrieval** = read long-term memory
  * **Learning** = write long-term memory

Then how does a language agent choose which action to take? Its actions are structured into **decision making** cycles, and each cycle has two stages:
* **Planning**: The agent applies reasoning/retrieval actions to (iteratively) propose and evaluate actions, then select a learning/grounding action.
* **Execution**: The selected learning/grounding action is executed to affect the internal memory or external world.

To understand more, read Section 4 of our [paper](https://arxiv.org/abs/2309.02427).

## Method Papers
We categorize method papers based on whether they mainly focus on interaction with the external world (grounding), working memory (reasoning), or long-term memory (learning/retrieval).
### Grounding (Interaction with External World)
#### Digital Interaction
API tools:
* [Toolformer: Language Models Can Teach Themselves to Use Tools](https://arxiv.org/abs/2302.04761) (Feb 2023)
#### Physical Interaction
#### Human Interaction
#### Multi-agent Interaction

### Reasoning (Interaction with Working Memory)

### Learning/Retrieval (Interaction with Long-term Memory)
(to be added soon. pull request welcome.)

## Benchmark Papers
(to be added soon. pull request welcome.)

## Survey/Position Papers & Blogposts
(to be added soon. pull request welcome.)

## Related Repos
* [LLM Powered Autonomous Agents (Lil’Log)](https://lilianweng.github.io/posts/2023-06-23-agent/)
* [LLM-Agents-Papers](https://github.com/AGI-Edgerunners/LLM-Agents-Papers)
* [LLMAgentPapers](https://github.com/zjunlp/LLMAgentPapers)
(more to be added soon. pull request welcome.)
