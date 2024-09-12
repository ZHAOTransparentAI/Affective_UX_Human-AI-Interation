# Affective User Research Human AI Interaction --Seminar 
## Introduction
In our research, we aim to investigate how task complexity and user characteristics influence emotions during interactions with large language models (here, Open assistant). In particular, we focus on how these factors affect users' emotional valence, which refers to the positive or negative quality of the emotion experienced. Understanding the dynamics between task complexity, user characteristics, and emotional responses can provide valuable insights for optimising human-AI interactions, particularly in contexts where maintaining a positive user experience is critical.

## Conceptual framework and prediction model
Our prediction model is designed to examine the influence of various independent variables related to task complexity and user characteristics on the emotional valence experienced during interactions with *Open assistant*.

**Task Complexity Variables**
1.	 *Task Difficulty*: We define task complexity based on the perceived difficulty of tasks. To quantify this, we employ a *two-step prompting method* where an LLM (such as GPT) is asked to rate the difficulty of tasks on a scale from 1 to 5. These ratings are then revised by incorporating *predefined task complexity levels*, resulting in a more accurate assessment of task difficulty. *Task Difficulty.pdf* provide with detailed two-step prompting methods.

2.	 *Prompt Length*: The length of the initial prompt provided by the user is another indicator of task complexity. A more detailed prompt may help the LLM retrieve more accurate information, potentially reducing the complexity of the task.

3.	 *Number of Prompt Interactions*: The number of interactions (i.e., prompt iterations) a user has with the LLM during a task is also considered. This variable reflects the user's efforts to refine their queries and obtain satisfactory answers. We hypothesize that an increase in prompt interactions could correlate with improved valence scores, as users might experience a sense of accomplishment upon achieving their desired outcomes.

4.	 *Task Time*: The time taken to complete a task is an indirect measure of its complexity. Longer task durations may indicate more challenging tasks, which could negatively impact the user's emotional valence due to frustration or fatigue.

**User Characteristics Variables**
1.	 *Educational background*: The user's level of education is taken into account as it may influence their ability to create effective prompts and interpret the output of the LLM. Users with higher levels of education may have a better understanding of how to interact with Open assistant, potentially leading to more positive emotional experiences.
2.	 *Frequency of LLM use*: We consider how often a user engages with Open assistant. Regular users may have developed strategies to extract information more efficiently, leading to higher satisfaction and more positive emotional valence.
3.	 *Initial emotional state*: To capture the user's initial emotional state when engaging with the LLM, we create a new variable, **prompt_VADER**. This variable is derived from the VADER sentiment analysis model, which rates the sentiment of the initial prompt text on a scale from -1 (most negative) to 1 (most positive). This variable provides an insight into how a user's mood at the start of the interaction may influence the overall emotional valence experienced.

**Additional variables**
In addition to the newly created variables, we also consider other relevant factors such as the user's understanding of the task, the time taken to complete tasks, their satisfaction with the LLM's performance, and their experience with analysis tools. These variables are included to provide a comprehensive understanding of the factors influencing emotional valence during LLM interactions.

## Hypotheses
Based on the conceptual framework, we hypothesis the following:
1.	 *Task complexity and emotional valence*: Higher task complexity, as indicated by longer task times, more immediate interactions, and higher difficulty ratings, will negatively affect emotional valence. Users may experience less enjoyment and satisfaction with more complex tasks, leading to lower valence scores.

2.	 *User characteristics and emotional valence*: Users with higher levels of education and more frequent use of LLM are expected to have more positive emotional valence during interactions. Their familiarity and skill in interacting with Open assistant may lead to more efficient and satisfying outcomes.

3.	 *Initial emotional state and emotional valence*: The initial sentiment of the user's prompt (as measured by **prompt_vader**) will influence the overall emotional valence. A more positive initial sentiment is likely to correlate with higher valence scores, as users may approach the interaction with a more optimistic mindset.

This predictive model aims to provide a nuanced understanding of how task complexity and user characteristics shape the emotional experiences of individuals interacting with Open assistant, with a particular focus on valence as the target variable.
