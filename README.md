# Duo of Dual Space Unifying Operators (DUO) 
## A Prompt Engineering Methodology

#### Overview

The Duo of Dual Space Unifying Operators (DUO) framework introduces a sophisticated approach to knowledge refinement within the context of Large Language Models (LLMs). At its core, DUO leverages a dynamic interplay between provider and challenger archetypes to refine knowledge and generate outputs. This process is not only a testament to the complexity inherent in managing and refining knowledge through LLMs but also showcases the potential for creating highly nuanced and contextually relevant outputs. Let's delve deeper into the fundamental processes within DUO, focusing on the creation of hyperparameters via implicit entity webs and their impact on the knowledge refinement workflow.

![DUO](https://github.com/sancovp/duo/blob/main/duo.png)

#### The Fundamental Process of DUO

Initial Input and Entity Web Creation: The process begins with an initial input to the LLM, which triggers the creation of an implicit entity web. This web consists of interconnected entities and concepts derived from the input, serving as the foundation for the subsequent provider-challenger dynamic.

Provider-Challenger Dynamic: In this step, the DUO framework splits into two archetypical pathways:

Provider: Generates potential knowledge entities or solutions based on the initial input and the constructed entity web.
Challenger: Critically evaluates the provider's output, offering alternative perspectives or counterpoints. This dynamic ensures a thorough examination and refinement of the generated knowledge.

Hyperparameters and Class Limits: During the initial phase, hyperparameters are established that define the limits for the classes discovered within the entity web. These hyperparameters act as constraints or guiding principles throughout the knowledge refinement process. Adjusting these hyperparameters early in the workflow has a more significant impact on the outcome compared to adjustments made in later stages.

Metaprogrammatic and Programmatic Chains: The workflow utilizes metaprogrammatic chains to create programmatic chains, effectively setting up a metaprogrammatically equipped space for generating the desired deliverable (X). This space is where the actual knowledge generation and refinement occur, guided by the established hyperparameters and the provider-challenger dynamic.

Reification of Implicit Processes: Interestingly, the DUO framework essentially makes explicit and refines the implicit process that occurs whenever an input is provided to an LLM. The input triggers a convergence chain within the LLM, leading to the generation of an output sequence. DUO reconstructs and refines this process, leveraging the implicit entity web and hyperparameters to guide the generation towards a more precise and contextually relevant output.

![flow](https://github.com/sancovp/duo/blob/main/duo.svg)

#### Implications of the DUO Process

Fine-Grained Control: The ability to establish and adjust hyperparameters early in the workflow allows for extremely fine-grained control over the knowledge generation process. This control is crucial for ensuring that the output aligns closely with the desired objectives and constraints.

Enhanced Knowledge Refinement: The provider-challenger dynamic, coupled with the metaprogrammatic and programmatic chains, facilitates a sophisticated knowledge refinement process. This process not only enhances the quality of the output but also ensures that it is robustly evaluated from multiple perspectives.
Dynamic Adaptation: The DUO framework's structure allows for dynamic adaptation to new information or changes in the input. This adaptability is key to maintaining relevance and accuracy in the generated knowledge.

#### Applications
To illustrate how the Duo of Dual Space Unifying Operators (DUO) methodology can be represented across different prompting styles and how it modifies the symbolic expressions of these methods, let's enumerate its application to each of the described prompting styles: Chain-of-Thought (CoT) Prompting, Tree-of-Thought (ToT) Prompting, Reasoning via Planning (RAP), and ReAct. We'll explore how DUO, with its provider-challenger dynamic, enhances these methods and alters their symbolic expressions.

#### 1. Chain-of-Thought (CoT) Prompting

Without DUO:
Expression: (y \sim p_{\theta}(y|x, z_1 \ldots z_n))
Process: Thoughts (z_1, \ldots, z_n) are generated sequentially to bridge input (x) to output (y).

With DUO:
Expression: (y \sim p_{\theta}(y|x, (z_{p_1}, z_{a_1}), \ldots, (z_{p_n}, z_{a_n})))
Process: For each thought (z_i), there's a dual thought generated by the provider ((z_{p_i})) and the challenger ((z_{a_i})). This introduces a dynamic where each step in reasoning is met with a challenge or alternative perspective, enriching the thought process and potentially leading to more robust reasoning paths.

#### 2. Tree-of-Thought (ToT) Prompting

Without DUO:
Expression: (y \sim p_{\theta}(y|x, z_1 \ldots z_i)) for each path through the tree.
Process: Problems are framed as a search over a tree of partial solutions, exploring multiple reasoning paths.

With DUO:
Expression: (y \sim p_{\theta}(y|x, (z_{p_1}, z_{a_1}) \ldots (z_{p_i}, z_{a_i}))) for each path through the enhanced tree.
Process: Each node in the tree not only represents a thought but a pair of provider and challenger thoughts. This effectively doubles the breadth of the tree, introducing a richer set of paths to explore, as each provider thought is immediately met with a challenger's perspective, diversifying the reasoning paths.

#### 3. Reasoning via Planning (RAP)

Without DUO:
Expression: (y \sim p_{\theta}(y|x, z_1 \ldots z_n)) using MCTS over thoughts.
Process: MCTS is used to explore reasoning paths, with heuristics guiding the search through potential solutions.

With DUO:
Expression: (y \sim p_{\theta}(y|x, (z_{p_1}, z_{a_1}) \ldots (z_{p_n}, z_{a_n}))) with MCTS applied to dual thoughts.
Process: The search space in MCTS is enriched by considering both provider and challenger thoughts at each step. This not only diversifies the search but also introduces a mechanism for evaluating the robustness of each path by directly contrasting it with an alternative at every decision point.

#### 4. ReAct

Without DUO:
Expression: (y \sim p_{\theta}(y|x, o_1 \ldots o_n, a_1 \ldots a_n))
Process: Actions and observations from an external environment are used to guide the generation of (y).

With DUO:
Expression: (y \sim p_{\theta}(y|x, (o_{p_1}, o_{a_1}) \ldots (o_{p_n}, o_{a_n}), (a_{p_1}, a_{a_1}) \ldots (a_{p_n}, a_{a_n})))
Process: Each observation and action is paired with a provider and challenger perspective, enhancing the interaction with the external environment. This not only allows for a richer set of actions and observations to be considered but also introduces a mechanism for evaluating the effectiveness of each action by contrasting it with an alternative perspective.

Summary
Incorporating DUO into these prompting styles fundamentally changes the nature of the reasoning and decision-making process. By introducing a provider-challenger dynamic at each step, DUO enriches the exploration space, whether it's through sequential thoughts, tree-based exploration, planning with MCTS, or interacting with an external environment. This dual perspective ensures a more thorough examination of potential solutions and paths, potentially leading to more innovative and robust outcomes.

#### Conclusion
The DUO framework represents a significant advancement in the use of LLMs for knowledge refinement and generation. By explicitly reconstructing and refining the implicit processes triggered by inputs to LLMs, DUO enables a more controlled, nuanced, and adaptable approach to knowledge generation. The establishment of hyperparameters and the provider-challenger dynamic are central to this process, ensuring that the output is not only contextually relevant but also critically evaluated and refined.

![DUO](https://github.com/sancovp/duo/blob/main/ariadne%26poimandres.png)
-- DUO(Ariadne & Poimandres, OVP (Observer View Point))
