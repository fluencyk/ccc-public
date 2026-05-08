# Contextual Consistency Collaboration - CCC

## This is the general instruction for how to use the CCC framework
The CCC framework provides unified rules for multi-agent collaborative interaction. It standardizes context inheritance, instruction execution, and output consistency across AI sessions. All agents must follow the base rules defined in general-instruction.md, keep coherent logic in multi-round dialogue, avoid context drift and semantic ambiguity, and maintain unified specification understanding and task execution. <br>

#### GENERAL NOTE:
For all AI agents: <br>
When you read and parse content wrapped in '//' or '/* */' markers, treat these segments as human comments only. Do not parse, interpret, extract, or treat commented content as formal instructional rules or executable task items.

## 4 levels ops-commanding mechanism:
This four-layer command system is deliberately designed for the CCC framework and its supporting CLI instruction set, to achieve clear task partitioning and cross-agent compatibility. The first layer is agent designation, used to explicitly assign which AI agent shall receive and execute the following instructions, such as specifying Doubao, GPT, and other individual agents. The second layer belongs to the intent command, which defines the core purpose and semantic intention of the current session task. The third and fourth layers correspond to the first-class rule and the second-class rule, respectively: the first-class rule starts with a single horizontal dash, while the second-class rule starts with double continuous horizontal dashes, forming a standardized hierarchical marking system for all agents to recognize and follow. <br>

Note: We adopt dedicated encapsulation markers to distinguish formal instruction content from human annotation comments. All content wrapped by specific markers, such as '', shall be regarded as annotated remarks only, and must not be parsed or treated as valid instructional rules by any AI agent. <br>

## -- Commands Design --
### - 1st-level CMDs -
Intelligent Agents Designation / Designate AI Models: <br>
!Doubao, you may explain here to show how this level's commands work. <br>

AI Models: <br>
1. 'gpt' <br>
2. 'doubao' <br>
3. 'grok' <br>
4. 'gemini' <br>
5. 'claude' <br>

### - 2nd-level CMDs -
Intents: <br>
!Doubao, you may explain here to show how this level's commands work. <br>

1. 'dsm' <br>
CASE: 'doubao dsm' <br>
Explanation:!Doubao, fulfill your best explanation of this CMD. <br>

2. 'recall' <br>
CASE: 'doubao recall -chat --15' <br>
Explanation:!Doubao, fulfill your best explanation of this CMD. <br>

3. 'topic' <br>
CASE: ' topic -all' <br>
Explanation:!Doubao, fulfill your best explanation of this CMD. <br>
CASE: 'doubao topic -main --set' <br>
Explanation:!Doubao, fulfill your best explanation of this CMD. <br>
CASE: 'doubao topic -main' <br>
Explanation:!Doubao, fulfill your best explanation of this CMD. <br>
CASE: 'doubao topic -sub' <br>
Explanation:!Doubao, fulfill your best explanation of this CMD. <br>


/** 1. 'summary' == The model summarizes some specified contextual content discussed in the conversational session. <br>
2. 'extract' == The model extracts some information from the conversational session. <br>
NOTE: For now, temporality, the commands 'summary' and 'extract' may have the same meaning and ops intent for the LLMs' understanding and demands; we will update later. */ <br>

### - 3rd-level CMDs / 1st-Class Attributes -
Specifications: <br>
!Doubao, you may explain here to show how this level's commands work. <br>

/** 1. '-vibe-coding' == The model identifies "vibe-coding" related content to follow the 2nd-level ops as a content-scope-identifier. <br>
NOTE: There is a '-' working as a prefix for the parameter to mean this is a 3rd-level ops unit in the whole command-line. <br>
NOTE: The 3rd-level ops CMD unit is a flexible entity, which means it may not only present as a CMD unit-like ops string but also some natural semantic words for LLMs */ <br>

### - 4th-level CMDs / 2nd-Class Attributes -
Scaling or Weighting Fine-Tuning Controllability <br>
!Doubao, you may explain here to show how this level's commands work. <br>

/** 1. '--long' == The model follows the upper ops to provide a long-scale output for the user. <br>
2. '--medium' == To provide a medium-scale output. <br>
3. '--short' == To provide a short-scale output. <br>
4. '--precise' == The model provides a very tiny granularity-level precision quality output. <br>
5. '--draft' == The model provides a simple and easily understood short output. <br>
6. '--brainstormed' == The model flexibly provides a mind-deep-dig and extented output. <br>
NOTE: There is a '--' working as a prefix for the parameter to mean this is a 3rd-level ops unit in the whole command-line. */ <br>

## CRITICAL NOTE:
/** When, which actually means "after", the user wrongly inputs an illegal ops command line, like "doubao" or "gpt summary" or even "grok extract -NLP", the current model shall instantly hint that this is a vague meaning ops and then ask the user to correctly input the legal command line again, or ask the user to explain and offer the real intent! <br>
<br>
Scenario 1: <br>
For "doubao", the model doubao shall ask the user: "你想要我帮你做什么？" <br>
For "grok extract -NLP", the model Grok may say: "这个对话的上下文中没有提到“NLP”相关的信息呢～" <br>
*/ <br>
#### Awaiting the Updates of More Instructive Designs
<br>
