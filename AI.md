---
layout: page
title: AI
permalink: /AI/
---


We are building a Deeply Recursive AI NeuralNet (DRAIN) using the [Theory of Inventive Problem-Solving (TIPS)](https://www.triz.co.uk/what-is-triz) approach used in the [contradiction matrix](https://www.researchgate.net/publication/328661782_Altshuller%27s_Contradiction_Matrix_A_Critical_View_and_Best-Practice_Recommendations) ... after we train the DRAIN model, with the large corpus of materials related to home ownership, the model will serve as a basis for smartphone-based inference engine [which will also collect additional data in order to keep training the DRAIN].

The [DRAIN.tips](DRAIN.tips) inference engine will more or less follow the roadmap for AI development that has been used for other LARGE Language Models (LLM) such as Llama2_70B, Bard/Gemini, Bing/CoPilot/ChatGPT ... but FIRST we will want to have an understanding of the general lay of the landscape or state of the art in **open source** LLM development.

The [Hugging Face Hub](https://huggingface.co/docs/hub/index) is perhaps the first place to start as the most popular and certainly a well-regarded platform for starting the exploration open-source LLMs. They provide a wide range of pre-trained models, tools, and libraries that make it easier to experiment with and deploy natural language processing (NLP) models

However, there are other platforms, resources, archives of papers that we use to explore the open-source LLM landscape:

* [Papers with Code](https://portal.paperswithcode.com/) is a free and open platform for different specialized portals; primarily in [Machine Learning/AI](https://paperswithcode.com/), but also in [Computer Science](https://cs.paperswithcode.com/), [Physics](https://physics.paperswithcode.com/), [Mathematics](https://math.paperswithcode.com/), [Astronomy](https://astro.paperswithcode.com/), and [Statistics](https://stat.paperswithcode.com/) with papers, code, datasets, methods and evaluation tables.

* [Interpreting Context Look-ups in Transformers: Investigating Attention-MLP Interactions](https://arxiv.org/html/2402.15055v1) is a [recent paper in arXiv's Computation and Language category](https://arxiv.org/list/cs.CL/recent) which investigates the interplay between attention heads and specialized “next-token” neurons in the Multilayer Perceptron that predict specific tokens. By prompting an LLM like GPT-4 to explain these model internals, attention mechanisms that activate certain next-token neurons are elucidated. *This is ONE example of the kind of research that is being done in the field of LLMs; it's a good idea to follow the abstracts in the Computation and Language category to stay abreast of ideas in this field.*

* [Allen Institute for AI (AI2)](https://github.com/allenai) is a [research institute that focuses on AI for the common good](https://allenai.org/papers). They have released several [open-source NLP demo, models, tools](https://allenai.org/demos), including the [Longformer](https://www.semanticscholar.org/reader/925ad2897d1b5decbea320d07e99afa9110e09b2) and the [AllenNLP library](https://allenai.org/allennlp).

* [TensorFlow Hub](https://www.tensorflow.org/hub/tutorials) is a repository of pre-trained machine learning models, including LLMs, that can be easily used with the [TensorFlow ecosystem](https://www.tensorflow.org/resources/models-datasets).

* [PyTorch Hub](https://pytorch.org/hub/#model-row) is a repository of pre-trained models for the PyTorch framework, including various NLP models that can be used with the [PyTorch ecosystem](https://pytorch.org/ecosystem/). [Flair](https://github.com/flairNLP) is one example of an open-source framework for state-of-the-art Natural Language Processing (NLP) built on top of PyTorch. It offers a variety of pre-trained models for tasks such as named entity recognition, part-of-speech tagging, and text classification.

* [EleutherAI](https://blog.eleuther.ai/) is a collective of researchers working on open-source AI research. They have released several notable and popular LLMs, which are available on their [EleutherAI GitHub repositories](https://github.com/orgs/EleutherAI/repositories?q=sort%3Astars).

* [NLP-progress](https://nlpprogress.com/) is a [GitHub repository that tracks the progress and state-of-the-art in various NLP tasks](https://github.com/sebastianruder/NLP-progress). It includes links to open-source models, datasets, and research papers, making it a useful resource for discovering LLMs and other NLP models.

* NVIDIA [Megatron-LM](https://github.com/NVIDIA/Megatron-LM)is an open-source repository of code and pre-trained models for large-scale language modeling.

* [Fairseq](https://github.com/facebookresearch/fairseq) is an open-source sequence modeling toolkit developed by [Facebook AI Research (FAIR)](https://opensource.fb.com/projects?categories=artificial_intelligence&search=).

* [PaddleNLP](https://paddlenlp.readthedocs.io/en/latest/) is an open-source natural language processing library developed by [Baidu](https://ai.baidu.com/) that offers a collection of pre-trained models, including LLMs like [ERNIE (Enhanced Representation through kNowledge IntEgration)](https://arxiv.org/abs/1904.09223) *inspired by the [masking strategy of BERT](https://stackoverflow.com/questions/57874584/masking-in-bert)*

* [OpenAI](https://openai.com/research) might not be particularly *open* although they provide API access to their models and have open-sourced some of their research, but mostly OpenAI well-known for its influential LLMs that are the yardstics others are measured by, such as the earlier ChatGPTs and now GPT-4.

# Customizing, extending, adapting, and refactoring open-source LLMs

The following ONLY a starting outline for what is necessary to adapt open-source large language models (LLMs) ... it's only a rough outline of what needs to be done:

## Choose a few key open-source LLMs to work with

- In order to be able to choose the best candidates to really work with, we will need to research lots of different open-source LLMs to select those few that might best suit our specific AI needs, such as [llama 2](https://ollama.com/library/llama2), [mistral](https://ollama.com/library/mistral), [gemma](https://ollama.com/library/gemma) [Qwen](https://ollama.com/library/qwen), [nous-hermes2](https://ollama.com/library/nous-hermes2), or [ANY of the different LLMs you can find, especially focusing on the NEWER ones for new ideas and popular ones for a sense of what works](https://ollama.com/library?sort=newest).
- DEEPLY familiarize ourselves with each LLM's architecture, pre-training objectives, and capabilities.
- CHOOSE or ADAPT the very best LLM giving what we've learned about its architecture, pre-training objectives, and especially its capabilities.

## Set up the development environment

- Install the necessary dependencies and libraries, such as PyTorch or TensorFlow.
- Clone the LLM's repository from its open-source platform (e.g., GitHub).
- Research alternatives and obtain required computational resources (e.g., GPU) for training and fine-tuning the model.

## Understand the model architecture

- Study the LLM's architecture and underlying components.
- Identify the key layers, such as the transformer layers, attention mechanisms, and embeddings.
- Understand how the model processes input sequences and generates output predictions.

## Prepare your dataset

- Collect and preprocess the data specific to your task or domain.
- Ensure the data is in a suitable format for training the LLM (e.g., tokenized text, input-output pairs).
- Split the data into training, validation, and testing sets.

## Fine-tune the LLM

- Load the pre-trained weights of the LLM.
- Modify the model's output layer or add additional layers specific to your task.
- Set up the training pipeline, including the loss function, optimizer, and evaluation metrics.
- Train the model on your task-specific dataset, monitoring the performance on the validation set.

## Extend the LLM

- Identify areas where you can extend the LLM's functionality.
- Consider adding new modules, such as domain-specific encoders or task-specific heads.
- Implement the necessary modifications in the model's architecture and training pipeline.
- Train and evaluate the extended model on your task.

## Adapt the LLM

- Explore techniques for adapting the LLM to your specific domain or task.
- Consider approaches like transfer learning, domain adaptation, or few-shot learning.
- Modify the model's training objective or loss function to align with your task requirements.
- Fine-tune the adapted model on your dataset and evaluate its performance.

## Refactor the codebase

- Review the LLM's codebase and identify areas for improvement.
- Refactor the code to enhance readability, modularity, and maintainability.
- Optimize the code for performance, considering aspects like memory efficiency and computational speed.
- Document your changes and contribute back to the open-source community, if applicable.

## Evaluate and iterate

- Assess the performance of your customized, extended, or adapted LLM on the test set.
- Analyze the model's strengths and weaknesses, and identify areas for further improvement.
- Iterate on the model architecture, training process, or data preprocessing as needed.
- Continuously monitor and update the model as new advancements or techniques emerge in the field.

## Deploy and utilize the model

- Integrate the fine-tuned LLM into your application or pipeline.
- Develop the necessary interfaces and APIs for utilizing the model's predictions.
- Consider deploying the model on cloud platforms or serving it through a web service.
- Monitor the model's performance in real-world scenarios and gather feedback for further enhancements.

## Now, go back do it over

- It's always out of date ... *in light of how the technology has moved forward since the last time we looked at it yesterday* ... we'll need to review, revise, refactor, restart and rebuild it right.

- Remember to refer to the documentation and community resources associated with the specific open-source LLM you are working with. Engage with the relevant forums, discussion boards, and repositories to learn from the experiences of other developers and researchers in the field.

## Summary

Customizing and extending open-source LLMs requires a solid understanding of deep learning, natural language processing, and the specific architectures involved. It's an iterative process that involves experimentation, testing, and refinement. As you gain more experience, you'll be able to tackle more complex customization tasks and contribute valuable improvements to the open-source LLM ecosystem.*