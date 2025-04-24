# Agentic Blogger

This Jupyter notebook, "agentic_bloggerGPT.ipynb", defines an agentic workflow for writing blog posts using LangGraph and the GPT-4.1 language model.

The script sets up a multi-agent graph where each node represents a stage in the blog post creation process. The stages include:

* **Planning:** An agent creates a high-level outline with key details based on a user prompt.
* **Research:** An agent acts as a research assistant to generate search queries for gathering relevant information.
* **Writing:** An agent writes a blog post draft tailored for LinkedIn to capture attention and curiosity, adopting the style of "AI by Design".
* **Critique:** A reviewer agent assesses the draft based on the plan, providing specific critique and recommendations for improvement.
* **Revision:** An expert editor agent revises the draft strictly according to the critique points to produce the final version.

The workflow is managed by a supervisor agent that delegates tasks sequentially through the planning, research, writing, critique, and revision stages, passing relevant context between agents.

The notebook also includes steps for importing necessary modules, initializing the LLM (GPT-4.1-mini) using an OpenAI API key, defining the specialized agents, and setting up the LangGraph workflow with memory for conversational history. It demonstrates an example interaction where the agents process a user query to analyze an article and then craft a blog post based on it.

Future steps mentioned in the notebook include implementing short and long-term memory, incorporating a human-in-the-loop component, experimenting with thinking budgets, further defining the workflow, and potentially creating a Replit UI.
