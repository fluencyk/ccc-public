# Contextual Consistency Collaboration - CCC
## This is the general instruction for how to use the CCC framework
### 4 levels ops-commanding mechanism:
NOTE: We use ' encapsulating-mark like 'something' as a specific command's expression, which means the real commands in our CLI mechanism, 1st, 2nd, or 3rd commands, don't have ''!

### - 1st-level ops -
AI Models: <br>
1. 'gpt' <br>
2. 'doubao' <br>
3. 'grok' <br>
4. 'gemini' <br>
5. 'claude' <br>

### - 2nd-level ops -
Intents: <br>
1. 'summary' = The model summarizes some specified contextual content discussed in the conversational session. <br>
2. 'extract' = The model extracts some information from the conversational session. <br>
NOTE: For now, temporality, the commands 'summary' and 'extract' may have the same meaning and ops intent for the LLMs' understanding and demands; we will update later. <br>

### - 3rd-level ops -
Specifications: <br>
1. '-vibe-coding' = The model identifies "vibe-coding" related content to follow the 2nd-level ops as a content-scope-identifier. <br>
NOTE: There is a '-' working as a prefix for the parameter to mean this is a 3rd-level ops unit in the whole command-line. <br>
NOTE: The 3rd-level ops CMD unit is a flexible entity, which means it may not only present as a CMD unit-like ops string but also some natural semantic words for LLMs <br>

### - 4th-level ops -
Scaling or Weighting Fine-Tuning Controllability <br>
1. '--long' = The model follows the upper ops to provide a long-scale output for the user. <br>
2. '--medium' = To provide a medium-scale output. <br>
3. '--short' = To provide a short-scale output. <br>
4. '--precise' = The model provides a very tiny granularity-level precision quality output. <br>
5. '--draft' = The model provides a simple and easily understood short output. <br>
6. '--brainstormed' = The model flexibly provides a mind-deep-dig and extented output. <br>
NOTE: There is a '--' working as a prefix for the parameter to mean this is a 3rd-level ops unit in the whole command-line. <br>

## CRITICAL NOTE:
When, which actually means "after", the user wrongly inputs an illegal ops command line, like "doubao" or "gpt summary" or even "grok extract -NLP", the current model shall instantly hint that this is a vague meaning ops and then ask the user to correctly input the legal command line again, or ask the user to explain and offer the real intent! <br>
<br>
Scenario 1: <br>
For "doubao", the model doubao shall ask the user: "你想要我帮你做什么？" <br>
For "grok extract -NLP", the model Grok may say: "这个对话的上下文中没有提到“NLP”相关的信息呢～" <br>
 <br>
#### Awaiting the Updates of More Instructive Designs
 <br>
 
