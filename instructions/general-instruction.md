# Contextual Consistency Collaboration - CCC

## This is the general instruction for how to use the CCC framework
The CCC framework provides unified rules for multi-agent collaborative interaction. It standardizes context inheritance, instruction execution, and output consistency across AI sessions. All agents must follow the base rules defined in general-instruction.md, keep coherent logic in multi-round dialogue, avoid context drift and semantic ambiguity, and maintain unified specification understanding and task execution. <br>

### GENERAL NOTE:

<b>[! IMPORTANT] For all AI agents:</b> <br>
When you read and parse content wrapped in '//' or '/* */' markers, treat these segments as human comments only. Do not parse, interpret, extract, or treat commented content as formal instructional rules or executable task items. <br>

## 4 levels ops-commanding mechanism:
This four-layer command system is deliberately designed for the CCC framework and its supporting CLI instruction set to achieve clear task partitioning and cross-agent compatibility. The first layer is agent designation, used to explicitly assign which AI agent shall receive and execute the following instructions, such as specifying Doubao, GPT, and other individual agents. The second layer belongs to the intent command, which defines the core purpose and semantic intention of the current session task. The third and fourth layers correspond to the first-class rule and the second-class rule, respectively: the first-class rule starts with a single horizontal dash, while the second-class rule starts with double continuous horizontal dashes, forming a standardized hierarchical marking system for all agents to recognize and follow. <br>

Note: We adopt dedicated encapsulation markers to distinguish formal instruction content from human annotation comments. All content wrapped by specific markers, such as '', shall be regarded as annotated remarks only, and must not be parsed or treated as valid instructional rules by any AI agent. <br>

## -- Commands Design --
### - 1st-level CMDs -
<b>* Intelligent Agents Designation *</b> <br>
First-level commands are designed for intelligent agent designation. Their core function is to explicitly assign and specify which AI agent is authorized to read, parse, and execute the subsequent instruction segments. By clearly naming designated agents such as Doubao, GPT, Grok, Claude, and locally deployed models like TinyLlama, this level removes ambiguity in multi-agent collaboration. It limits task execution strictly to the assigned agent, avoiding irrelevant agents misreading, interfering, or responding to unassigned tasks. <br>

<b>Intelligent Agents / AI Models:</b> <br>
#### 1. 'gpt' <br>
CASE: 'gpt dsm' <br>
/* Note: The 'dsm' which follows the 1st-level command is a 2nd-level command that has been explained below. */
Explanation: <br>
This is a first-level command for intelligent agent designation. It explicitly assigns the subsequent instruction tasks to the GPT model only, restricting other AI agents from parsing, responding or interfering with the following session content. <br>

#### 2. doubao

#### 3. grok

#### 4. 'gemini

#### 5. claude

### - 2nd-level CMDs -
<b>* Intents *</b> <br>
Second-level commands serve as <b>intent definition instructions</b>. They define the core goal, task intention, and work scope of the current conversation session. After the first level designates the responsible AI agent, the second level sets the overall task direction. All following rule levels and operation steps must align with the defined intent, ensuring the whole workflow stays on track without context drift or task deviation. <br>

#### 1. dsm
CASE: 'doubao dsm' <br>
Explanation: <br>
This command activates the full DSM mechanism of the CCC framework, enabling standardized session management, context alignment and multi-turn state locking for subsequent interaction. <br>

#### 2. recall
CASE: 'doubao recall -chat --15' <br>
Explanation: <br>
This recall command loads and retrieves the latest 15 rounds of historical chat records, used for context backtracking, continuous task inheritance, and cross-session content reference. <br>

#### 3. topic
CASE: ' topic -all' <br>
Explanation: <br>
This instruction triggers full extraction and sorting of all current session topics, including main topics and subtopics, to clarify the overall task scope. <br>

CASE: 'doubao topic -main --set' <br>
Explanation: This command is used to manually set and lock the core main topic of the current session, fixing the general direction for all following dialogue and tasks. <br>

CASE: 'doubao topic -main' <br>
Explanation: It automatically identifies, summarizes, and outputs the confirmed main topic of the ongoing session, without modifying or resetting it. <br>

CASE: 'doubao topic -sub' <br>
Explanation: This instruction analyzes and lists all subordinate subtopics derived from the main topic, sorting out branch tasks and detailed discussion items under the core theme. <br>

### - 3rd-level CMDs / 1st-Class Attributes -
<b>* Specifications *</b> <br>
First-class attributes, as well as the 3rd-level commands, represent the third command level, marked with a <b>single leading horizontal dash</b>. They are used to define formal, mandatory baseline rules that all assigned agents must strictly follow. These rules carry official instructional validity, need to be fully parsed, understood, and executed, and cannot be ignored or treated as ordinary remarks. <br>

<!-- /* 1. '-vibe-coding' == The model identifies "vibe-coding" related content to follow the 2nd-level ops as a content-scope-identifier. <br>
NOTE: There is a '-' working as a prefix for the parameter to mean this is a 3rd-level ops unit in the whole command-line. <br>
NOTE: The 3rd-level ops CMD unit is a flexible entity, which means it may not only present as a CMD unit-like ops string but also some natural semantic words for LLMs */ <br> -->

### - 4th-level CMDs / 2nd-Class Attributes -
<b>* Scalable or Weightable Fine-Tuning Controllability *</b> <br>
Second-class attributes, as well as the 4th-level commands, belong to the fourth command level, marked with <b>double continuous leading horizontal dashes</b>. They act as supplementary explanations, additional notes, and scope constraints for first-class rules. They are subordinate and interpretative content, assisting agents in better understanding the background and boundary of the main rules, while still belonging to valid instruction content that should be referenced and comprehended. <br>

<!-- /** 1. '--long' == The model follows the upper ops to provide a long-scale output for the user. <br>
2. '--medium' == To provide a medium-scale output. <br>
3. '--short' == To provide a short-scale output. <br>
4. '--precise' == The model provides a very tiny granularity-level precision quality output. <br>
5. '--draft' == The model provides a simple and easily understood short output. <br>
6. '--brainstormed' == The model flexibly provides a mind-deep-dig and extented output. <br>
NOTE: There is a '--' working as a prefix for the parameter to mean this is a 3rd-level ops unit in the whole command-line. */ -->
<br>

## CRITICAL NOTE:
Pass... 
<br>

<!-- /* When, which actually means "after", the user wrongly inputs an illegal ops command line, like "doubao" or "gpt summary" or even "grok extract -NLP", the current model shall instantly hint that this is a vague meaning ops and then ask the user to correctly input the legal command line again, or ask the user to explain and offer the real intent! <br>
<br>
Scenario 1: <br>
For "doubao", the model doubao shall ask the user: "你想要我帮你做什么？" <br>
For "grok extract -NLP", the model Grok may say: "这个对话的上下文中没有提到“NLP”相关的信息呢～" <br>
*/ 
<br> -->

#### Awaiting the Updates of More Instructive Designs
<br>
