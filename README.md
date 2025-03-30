# Prompt-Engineering

1. Designing effective instructions to get the best responses from language models.
2. Experiment with different prompt formulations.
3. Refining your prompts based on the model's responses is part of the process.
4. Copy paste the prompts in your choice of LLM and observe the results. 

# Types of Prompting Techniques

## Few Shot Prompting
+ Few-shot prompting is a technique where you provide a model with a few example pairs of inputs and outputs within the prompt to illustrate the task. By doing so, you set a clear pattern for the model to follow when responding to a new query.

## Zero Shot Prompting
+ Zero-shot prompting is when you ask a language model to perform a task without providing any examples. You simply give it a clear instruction or question, and it figures out what to do based on its prior training.

## Few Shot Chain of Thought
+ You give the model a few examples of the task (like in regular few-shot prompting), But in each example, you also show the reasoning steps that lead to the final answer — not just the answer itself.
+ It’s useful when the task involves reasoning, judgment, or decision-making, rather than simple pattern matching.

## Zero Plus Few Shot Chain of Thought
+ A hybrid technique that’s super useful when you want the model to think step-by-step without showing too many examples, or sometimes none at all.
+ It’s when you:
  - Give no (or just one) example, But explicitly ask the model to "think step-by-step" in the prompt.
+This is different from regular zero-shot (which gives no reasoning) and from few-shot CoT (which gives multiple examples with reasoning).

## Zero Shot Chain of Thought
+ You don’t provide any examples, but you explicitly tell the model to “think step-by-step” in your prompt.
+ It’s great for reasoning tasks when:
  - You want simplicity (no few-shot setup).
+ The model just needs a gentle nudge to explain its thinking. You’re asking for a decision, judgment, or analysis.

## Deep Breath
+ The “Deep Breath” prompt is a psychological nudge — it's a casual way to guide the model to slow down and generate a step-by-step, thoughtful answer, even in a zero-shot setting.
+ It’s a softer version of: "Think step-by-step".
  - But instead of sounding formal, you simply say - “Let’s take a deep breath and think through this carefully.”

## Generated Knowledge
+ Generated knowledge prompting is when you ask the model to generate background information or relevant facts first, before solving the main problem.
+ It’s especially useful when:
  - The model needs context to answer accurately.
  - The task requires reasoning, world knowledge, or multi-step logic.
  - You want to simulate how a human might recall relevant facts before making a decision.

## Tree of Thought
+ Instead of a single reasoning path, explore multiple possible thoughts, evaluate them, and choose the best.
  - Like a decision tree for reasoning.
  - At each step, generate different options (branches) for what to think/do next.
  - Evaluate or score them.
  - Choose the best path forward.

## Directional Stimulus
+ Steer the model’s attention or thinking in a specific direction before it answers.
  - You stimulate the model to focus on relevant features, ideas, or aspects before the task.
  - This primes the response to be goal-aligned and focused.

## Chain of Desnity
+ Pack more information into a response step-by-step without losing clarity.
  - You start with a basic answer.
  - Then, in steps, you densify it — adding more detail, insights, data, or nuance.
  - The final result is rich, informed, and concise.
