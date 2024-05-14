<div align="center">
  <h1>Awesome Synthetic (text) datasets </h1>
   <p><em>Generating datasets using large language models</em></p>
</div>
<br/>

## What is synthetic data?

Synthetic data refers to artificially generated data that _usually_ aims to mimic real-world data. This data is created algorithmically, often using models or simulations, rather than being collected from real-world sources. Synthetic data has been used for a long time in machine learning. Since the advent of LLMs, there has been increasing use of LLMs for producing synthetic data and for using synthetic data for training LLMs.

## Resources

## Tutorials, guides and educational blog posts

WIP!

### Important Datasets

#### [TinyStories](https://huggingface.co/datasets/roneneldan/TinyStories)

> TinyStories, a synthetic dataset of short stories that only contain words that a typical 3 to 4-year-olds usually understand, generated by GPT-3.5 and GPT-4. We show that TinyStories can be used to train and evaluate LMs that are much smaller than the state-of-the-art models (below 10 million total parameters), or have much simpler architectures (with only one transformer block), yet still produce fluent and consistent stories with several paragraphs that are diverse and have almost perfect grammar, and demonstrate reasoning capabilities.

#### [OpenHermes-2.5](https://huggingface.co/datasets/teknium/OpenHermes-2.5)

> The Open Hermes 2.5 dataset is a continuation of the Open Hermes 1 dataset, at a much larger scale, much more diverse, and much higher quality compilation, reaching 1M, primarily synthetically generated instruction and chat samples.

#### [Cosmopedia](https://huggingface.co/datasets/HuggingFaceTB/cosmopedia)

> Cosmopedia is a dataset of synthetic textbooks, blogposts, stories, posts and WikiHow articles generated by Mixtral-8x7B-Instruct-v0.1.The dataset contains over 30 million files and 25 billion tokens, making it the largest open synthetic dataset to date.

A reproduction of Textbooks Are All You Need. More detail in this [blog post](https://huggingface.co/blog/cosmopedia)

#### [WebSight](https://huggingface.co/datasets/HuggingFaceM4/WebSight)

> WebSight is a large synthetic dataset containing HTML/CSS codes representing synthetically generated English websites, each accompanied by a corresponding screenshot.

More details in this [blog post](https://huggingface.co/blog/websight).

#### [synthetic_text_to_sql](https://huggingface.co/datasets/gretelai/synthetic_text_to_sql)

> gretelai/synthetic_text_to_sql is a rich dataset of high quality synthetic Text-to-SQL samples, designed and generated using Gretel Navigator, and released under Apache 2.0. Please see our release blogpost for more details.

### Libraries, code and tools

This list isn't compressive and tries to focus on either actively developed libraries or libraries/code examples that demonstrate a particular approach well.

#### [distilabel](https://distilabel.argilla.io/latest/)

> ⚗️ distilabel is a framework for synthetic data and AI feedback for AI engineers that require high-quality outputs, full data ownership, and overall efficiency.

This is a very flexible library that is actively being developed and improved. It supports a large number of LLM providers. It includes many common synthetic data generation techniques from papers such as [Self-Instruct](https://distilabel.argilla.io/latest/reference/distilabel/steps/tasks/self_instruct/) and [EvolInstruct](https://distilabel.argilla.io/latest/api/steps/tasks/text_generation/#distilabel.steps.tasks.evol_instruct.base.EvolInstruct).

#### [llm-swarm](https://github.com/huggingface/llm-swarm)

> Manage scalable open LLM inference endpoints in Slurm clusters

This library is primarily focused on scaling synthetic text generation using Slurm clusters. This library was used to generate [Cosmopedia](https://github.com/davanstrien/awesome-synthetic-datasets?tab=readme-ov-file#cosmopedia)

#### [Domain Specific Dataset Project](https://github.com/huggingface/data-is-better-together/blob/main/domain-specific-datasets/README.md)

This is a project to bootstrap the creation of domain-specific datasets for training models. The goal is to create a set of tools that help users to collaborate with domain experts. Includes a UI tool for creating a pipeline for generating a synthetic dataset focused on a particular domain.

### Important Papers

Some important papers about synthetic data generation. **Note** I'm not trying to add every possible paper on the topic, but rather focus on those that introduced important techniques or had a big impact (particularly "in the wild").

- [Textbooks Are All You Need](https://huggingface.co/papers/2306.11644)
- [TinyStories: How Small Can Language Models Be and Still Speak Coherent English?](https://huggingface.co/papers/2305.07759)
- [Self-Instruct: Aligning Language Model with Self Generated Instructions](https://huggingface.co/papers/2212.10560)
- [WizardLM: Empowering Large Language Models to Follow Complex Instructions](https://huggingface.co/papers/2304.12244)
  (Also check out the other Wizard papers i.e. [WizardCoder: Empowering Code Large Language Models with Evol-Instruct](https://huggingface.co/papers/2306.08568)).
- [Improving Text Embeddings with Large Language Models](https://huggingface.co/papers/2401.00368)
