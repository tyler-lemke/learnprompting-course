# Notes from [Introduction to Prompt Engineering](https://learnprompting.thinkific.com/courses/take/introduction_to_prompt_engineering)

### Overview of Prompts

Prompts can be text-based or multimodal (incorporating multiple types of input like text, images, etc.).

### Six Parts of a Good Prompt:

1. Context
2. Examples
3. Role
4. Style/Tone
5. Instruction
6. Formatting information

---

### Understanding LLMs

- LLMs (Large Language Models) learn by predicting the next word based on the previous ones.
- LLMs use transformer architecture to process all words at once.
- Strengths: Great at generating and understanding text-based tasks.
- Weaknesses: LLMs might misunderstand your intent and can fabricate information.

---

### Prompting Strategies

#### Zero-Shot Chain of Thought

- Use: Directly ask for step-by-step reasoning.

#### Few-Shot

- Use: Provide clear, well-structured examples in the prompt.

#### Few-Shot Chain of Thought

- Use: Include both reasoning and structured examples for better outputs.

---

### Tackling Complex Problems

#### Generated Knowledge

- Ask a question, then request the model to list relevant facts before answering.

#### Least-to-Most Prompting

- Break the problem into smaller sub-questions.
- Solve each one step by step, based on a child-like teaching method.
- Different from chain of thought.

#### Emotional Prompting

- Use emotional encouragement to improve performance.

---

### Conflicting Outputs

#### Self-Consistency Prompting

- Ask the same question multiple times and take the most consistent answer.

#### Role Prompting

- Assign specific roles to guide the model in providing more accurate responses.

#### Multiple Role Prompting

- Have the model answer the question from different assigned roles.

#### Lower Temperature Setting

- Reducing the model's temperature setting increases response consistency.

---

### Combatting Hallucinations

- **Causes**: Hallucinations occur due to training on human data, inherent randomness, and the model’s tendency to be overly agreeable.
- **Mitigation**:
  - Use Self-Evaluation Prompting: Ask if the model is confident and explore how it might be wrong.
  - **RAG (Retrieval-Augmented Generation)**: Incorporate external knowledge to avoid hallucinations.

---

### Bias in LLMs

- LLMs are often trained on Western-centric data, leading to bias (e.g., top philosophers often being Western).
- **General Bias**: Use debiasing prompts or instruct the model to be open-minded.
- **Shot Prompt Bias**: Randomize the order of positive and negative examples to reduce bias.
- **Further Reading**: [Debiasing Techniques](https://learnprompting.org/docs/reliability/debiasing) | [Paper on Bias Harms](https://arxiv.org/pdf/2309.00770.pdf)

---

### Combining Techniques

- Use multiple strategies in one prompt, including role, context, chain of thought, and emotional appeal.
- Create a diverse and dynamic scenario.
- Apply self-refinement prompting to improve output.

---

### Risks of Generative AI

- Potential to amplify existing biases.
- Risk of spreading misinformation.

---
