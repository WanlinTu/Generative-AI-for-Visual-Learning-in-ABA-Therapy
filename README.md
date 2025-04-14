# Generative AI for Visual Learning in ABA Therapy

**Presenter: Maggie Tu**

**Email: wanlin.tu@vanderbilt.edu**

## Problem Statement & Overview
Applied Behavior Analysis (ABA) therapy often relies on visual aids to help autistic individuals learn new concepts through repetition and generalization. However, sourcing appropriate and diverse images is time-consuming and inconsistent—therapists typically rely on Google searches or limited image libraries that may not meet the cognitive or contextual needs of each child.

This project presents a generative AI-based image search and generation tool designed to support visual learning in ABA therapy. The tool enables therapists to input a multi-word prompt (e.g., "brushing teeth") and generate a wide variety of realistic images with plain or age-adjusted backgrounds. By offering multiple image variations per concept, the tool helps reinforce generalization—a core goal of ABA therapy.

This feature will be integrated into an existing electronic medical record (EMR) platform, giving therapists an efficient, customizable way to create, save, and reuse visual content directly within their therapy workflow. Additional functionalities include stepwise spelling input to support language learning, safety filters to ensure appropriateness, and prompt saving for future use.

## Methodology
This project applies several foundational techniques and concepts to build a practical tool for therapists working with autistic children. The methodology draws from the following key areas:

**Generative AI for Visual Content Creation**

At the core of this project is the use of a large text-to-image model (DALL·E 3) to generate visual content based on user-defined prompts. These models use transformer-based architectures and diffusion processes to convert natural language into high-resolution, photorealistic images. This approach enables flexible, on-demand creation of diverse visuals tailored to individual learning needs—ideal for supporting concept generalization in ABA therapy.

**Prompt Engineering**

To ensure output quality and relevance, the tool uses structured prompt templates that minimize ambiguity and control for age appropriateness. By guiding the model with precise, consistent language, we reduce hallucination and increase the likelihood of receiving accurate, context-appropriate visuals. This reflects key principles of effective prompt engineering covered in class.

**Human-Centered Design & Usability**

The tool was developed with a focus on therapist usability. Using a simple interface, therapists can specify the subject, background color, and type of image they need. They can generate multiple variations of an image, save results, and reuse prompts—streamlining a process that is otherwise time-consuming and inconsistent when done manually.

**Ethical & Responsible AI Practices**

Ethical considerations are integral to this project. The tool includes safety prompts to ensure that generated content is suitable for children, and it limits the scope of each request to avoid unintended outputs. These decisions align with our coursework discussions on responsible AI deployment, particularly in healthcare and education contexts.

## Assessment & Evaluation

**Image Relevance & Quality**

Each generated image was reviewed for:

Fidelity to prompt (Does the image reflect the subject, background, and tone described?)

Child-appropriateness (Free of unwanted or overly complex visual elements)

Variation (Different visual representations of the same concept to support generalization)

**Prompt Responsiveness**

We tested prompt variations across multiple categories (e.g., animals, objects, people) and background types. Results showed that:

(*connect to the course) Highly structured prompts yield more accurate results

Abstract or vague prompts often lead to hallucinated or irrelevant outputs This informed our prompt engineering strategy of using explicit, constrained templates.

**Limitations**

Responses can vary depending on model load and randomness in generation

Certain prompts (e.g., social scenarios) are harder to render accurately

No large-scale formal testing has been conducted yet

## Model

**Model Information**

Model Used: DALL·E 3 (via OpenAI API)

Architecture: Transformer-based text-to-image diffusion model

Version: DALL·E 3 (2023, API access through OpenAI)

DALL·E 3 is a generative model capable of converting detailed natural language prompts into high-resolution, photorealistic images. It leverages a combination of transformers and diffusion techniques to iteratively generate visual content from noise, conditioned on text embeddings.

**Architecture: How Transformers Enable Image Generation**

DALL·E 3 is built on a transformer-based architecture, which enables it to understand natural language prompts and generate coherent, high-quality images. The model uses a text encoder (based on transformers) to process the prompt and generate embeddings that condition the image generation process.

In diffusion-based architectures like DALL·E 3, these text embeddings guide a denoising model to iteratively transform noise into an image that aligns with the input description.

The process can be broken down into four main stages:

1. **Text Encoding** – The input prompt is tokenized and passed through a transformer encoder to create contextual embeddings.
2. **Image Conditioning** – These embeddings guide the image generation process through cross-attention.
3. **Image Generation** – A denoising transformer or decoder stack transforms random noise into image tokens.
4. **Output Refinement** – The image is enhanced and filtered for safety and quality.

![Screenshot 2025-04-13 at 8 18 24 PM](https://github.com/user-attachments/assets/7e1d4025-ee73-4cdf-96f7-4a0ef92aca6c)



**Intended Uses**

Designed for educational and therapeutic use within ABA (Applied Behavior Analysis) settings.

Allows therapists to generate multiple, safe, and customizable images to support concept learning and generalization in autistic children.

Intended for professional and supervised use by clinicians, therapists, or caregivers—not for unsupervised child use.

**License & Access**

Model Provider: OpenAI

License: Subject to OpenAI’s usage policies

API Access: Requires personal API key and agreement with OpenAI’s terms of service

Images Generated: Not guaranteed to be open-license; users are advised to review content before publishing or sharing

## Critical Analysis

**Model Comparison: Stable Diffusion vs. DALL·E**

We initially explored multiple generative models including Stable Diffusion and DALL·E to determine which would produce the most appropriate images for young learners. While Stable Diffusion offered more flexibility and fine-tuning capabilities, we observed that it frequently generated distorted or emotionally unsettling images, especially when prompts were underspecified.

In contrast, DALL·E consistently produced friendlier, higher-quality, and emotionally safe outputs with less need for manual filtering. For our use case — creating educational images for children — we ultimately selected DALL·E as the default generation engine. Below is an example of a “scary” image generated by Stable Diffusion that reinforced this decision:

![Screenshot 2025-04-12 at 11 59 17 PM](https://github.com/user-attachments/assets/4e5d10cd-026c-452d-a2a5-4eacce99bf6e)                                  
![Screenshot 2025-04-13 at 12 02 04 AM](https://github.com/user-attachments/assets/000200ad-1481-4e57-a785-548e76731646)


**Prompt Engineering as Design Control**

Throughout the development process, we learned that the phrasing of prompts significantly affects image quality, clarity, and emotional tone — even with the same model.

For instance, to support single-object learning for younger children, we refined our prompts from a simple "cat" to:

Realistic high-quality photo of a cat on a plain white background, for educational use.

This small shift in wording improved realism, eliminated distracting backgrounds, and ensured consistency across outputs.

We also designed prompts for generalization learning, a key goal in ABA therapy. To help children recognize variation within a concept, we tested prompts like:

Realistic high-quality photos of different types of cats on plain white backgrounds, for educational use.

These prompts led to output that varied in breed and form, helping reinforce flexible concept understanding.

Through these iterations, we learned that prompt engineering is not just a technical skill, but a design decision that affects educational effectiveness and ethical usability.

**Why These Decisions Matter**

In the context of therapy and education, visual content must be:

- Emotionally safe

- Easy to interpret

- Consistent with learning objectives

By combining model evaluation, targeted prompt design, and iterative testing, we developed a tool that aligns with those priorities. Our critical analysis informed both what we built and why we built it that way — making it not just a generative AI demo, but a thoughtfully designed learning experience.

**Next Step**

The next step is to collaborate more closely with therapists to conduct systematic testing of prompt variations and image outputs. This includes:

- Building a curated prompt library tailored to different therapy goals

- Collecting qualitative feedback from therapists on usability and content relevance

- Exploring automated prompt suggestions or adaptive prompt tuning based on therapist input

- Potentially integrating Stable Diffusion or fine-tuned open-source models for offline or lower-cost generation

## Key Resources & References
DALL·E 3 – OpenAI’s DALL·E [documentation: For text-to-image generation API.](https://platform.openai.com/docs/guides/images?api-mode=responses)

Prompt Engineering – “Prompt Engineering Guide” by DAIR.AI: Techniques and best practices. https://github.com/dair-ai/Prompt-Engineering-Guide

Ethical AI Use – “On the Opportunities and Risks of Foundation Models” (Stanford CRFM, 2021): On the ethical deployment of generative models. http://crfm.stanford.edu/assets/report.pdf
