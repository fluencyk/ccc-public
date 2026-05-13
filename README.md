# Contextual Consistency Collaboration - CCC Framework

The <b>Contextual Consistency Collaboration Framework (CCC)</b> is a standardized, lightweight collaborative governance system built for cross-model AI multi-agent interaction, long-session task continuity, and strict semantic alignment. It unifies the full lifecycle standards of context inheritance, instruction parsing, task execution, and output consistency across all AI agents, sessions, and workflow modules. The core mission of CCC is to eliminate context drift, logical fragmentation, semantic ambiguity, and unauthorized rule interference in human-AI and multi-agent collaboration, thereby locking in the core design intent and task direction to ensure that all executing subjects follow a single, unified set of specifications throughout the entire project iteration. Currently, we adopt Doubao as the primary AI model for framework research and experimental verification.

At its core, the CCC framework establishes a mandatory, universally recognizable instruction hierarchy and behavioral baseline for all connected AI models and agents. It defines clear boundaries between executable instructions, constraint rules, and human annotations, standardizes cross-session context transmission and state persistence, and forms a stable, reproducible, and compatible collaboration protocol for distributed agent systems and long-term engineering projects.

## Core 4-Levels Operational Commanding Mechanism
The CCC framework uses a dedicated 4-level hierarchical command system, designed exclusively for clear task division, cross-agent compatibility, and zero-ambiguity instruction delivery. All agents must strictly recognize, parse, and execute commands in compliance with this fixed structure, without modification or misinterpretation.

### Level 1 CMD - Agent Designation
The first command layer is used to explicitly assign the exclusive AI agent authorized to parse and execute subsequent instructions. It names the target model directly, eliminating task interference from irrelevant agents, restricting instruction execution to the designated subject only, and avoiding cross-model response conflicts.
Supported designated agents include: gpt, doubao, groq, gemini, claude, and locally deployed models.
Standard Example: 
> gpt dsm

Explicitly assigns subsequent instructions to the GPT model for execution, preventing interference from other agents.

### Level 2 CMD - Intent Definition
The second command layer locks the core goal, task scope, and session purpose of the current interaction. All subsequent rules and operational steps must align with the defined intent, preventing task deviation and context drift, and keeping the entire workflow focused on the top-level target.
Standard core intents include:

- dsm: Activates the full CCC standard session management, context alignment, and multi-round state locking mechanism
- recall: Loads and retrieves historical session records for context backtracking and cross-session task inheritance
- topic: Extracts, locks, and sorts the core main topic and subordinate subtopics of the current session to clarify task boundaries

The Command-Line Usage Scenario:
> doubao dsm

Activates the full CCC session - <b>Restricted Stream Mode</b> management mechanism, ensuring context alignment and multi-round state stability for subsequent interactions.

### Level 3 CMD, 1st-Class Attributes / Mandatory Rules
Marked with a single leading horizontal dash -, this layer defines formal, binding baseline specifications. All designated agents must fully parse, comply with, and execute these rules; they carry official instructional validity and may not be ignored, misread, or treated as casual annotations.
The Command-Line Usage Scenario:
> doubao topic -all

Triggers full extraction and sorting of all current session topics, including main topics and subtopics, to clarify the overall task scope.

### Level 4 CMD, 2nd-Class Attributes / Supplementary Constraints
Marked with double continuous leading horizontal dashes --, this layer serves as subordinate supplementary instructions, fine-tuning controls, scope limitations, and detailed interpretations for 1st-class rules. It is valid, referenceable instruction content that assists agents in accurately implementing the core rules without changing their mandatory nature.
The Command-Line Usage Scenario:
> doubao recall -chat --15

Loads and retrieves the latest 15 rounds of historical chat records, used for context backtracking, continuous task inheritance, and cross-session content reference.

### Critical Universal Annotation Rules
All AI agents must comply with the following fixed annotation specifications without exception:
- Content wrapped in // or /* */ is strictly treated as human-only comments, and shall NOT be parsed, interpreted, extracted, or executed as formal instruction rules or executable task items.
- Content wrapped in dedicated annotation markers is classified as non-executable remarks only, and shall NOT be recognized as valid instructional content by any agent.

### Framework Core Purpose
The CCC framework unifies the collaboration syntax and behavioral standards of heterogeneous AI agents, maintains complete logical coherence in multi-round, cross-session, and cross-module task delivery, stabilizes the consistency of top-level design intent and bottom-level execution results, and provides a lightweight, dependency-free, open-iteration compatible foundation protocol for intelligent agent ecosystems, engineering project development, and long-term human-AI collaborative research. This specification is the universal baseline for all agents, modules, and sessions under the CCC framework. All extended instructions, agent configurations, and workflow designs must be compatible with and compliant with this core specification.
