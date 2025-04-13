# Generative AI for Visual Learning in ABA Therapy

**Presenter: Maggie Tu**

**Email: wanlin.tu@vanderbilt.edu**

## Problem Statement & Overview
Applied Behavior Analysis (ABA) therapy often relies on visual aids to help autistic individuals learn new concepts through repetition and generalization. However, sourcing appropriate and diverse images is time-consuming and inconsistent—therapists typically rely on Google searches or limited image libraries that may not meet the cognitive or contextual needs of each child.

This project presents a generative AI-based image search and generation tool designed to support visual learning in ABA therapy. The tool enables therapists to input a multi-word prompt (e.g., "brushing teeth") and generate a wide variety of realistic images with plain or age-adjusted backgrounds. By offering multiple image variations per concept, the tool helps reinforce generalization—a core goal of ABA therapy.

This feature will be integrated into an existing electronic medical record (EMR) platform, giving therapists an efficient, customizable way to create, save, and reuse visual content directly within their therapy workflow. Additional functionalities include stepwise spelling input to support language learning, safety filters to ensure appropriateness, and prompt saving for future use.

## Methodology
This project applies several foundational techniques and concepts from our Generative AI coursework to build a practical tool for therapists working with autistic children. The methodology draws from the following key areas:

**Generative AI for Visual Content Creation**

At the core of this project is the use of a large text-to-image model (DALL·E 3) to generate visual content based on user-defined prompts. These models use transformer-based architectures and diffusion processes to convert natural language into high-resolution, photorealistic images. This approach enables flexible, on-demand creation of diverse visuals tailored to individual learning needs—ideal for supporting concept generalization in ABA therapy.

**Prompt Engineering**

To ensure output quality and relevance, the tool uses structured prompt templates that minimize ambiguity and control for age appropriateness. By guiding the model with precise, consistent language, we reduce hallucination and increase the likelihood of receiving accurate, context-appropriate visuals. This reflects key principles of effective prompt engineering covered in class.

**Human-Centered Design & Usability**

The tool was developed with a focus on therapist usability. Using a simple interface, therapists can specify the subject, background color, and type of image they need. They can generate multiple variations of an image, save results, and reuse prompts—streamlining a process that is otherwise time-consuming and inconsistent when done manually.

**Ethical & Responsible AI Practices**

Ethical considerations are integral to this project. The tool includes safety prompts to ensure that generated content is suitable for children, and it limits the scope of each request to avoid unintended outputs. These decisions align with our coursework discussions on responsible AI deployment, particularly in healthcare and education contexts.

## Critical Analysis

This project demonstrates how generative AI can be adapted to address real needs in therapeutic education. By equipping therapists with the ability to create personalized, high-quality visual aids, the tool enhances the effectiveness of ABA therapy—particularly in supporting concept generalization, which is a core challenge for autistic learners.

One of the key insights revealed during development is the importance of prompt precision and adaptability. While generative models are powerful, their outputs are highly sensitive to the wording, structure, and constraints of the prompt. This means that therapists may need different phrasing or image styles depending on the child’s age, developmental level, or specific learning objective. The current challenge is testing and iterating on a wide range of prompts that align with actual therapy needs in the field.

The next step is to collaborate more deeply with therapists to co-develop a library of optimized, reusable prompts for common therapy scenarios. In the long term, the tool could incorporate prompt templates, automated fine-tuning options, or even adaptive feedback systems to improve personalization and efficiency.

Ultimately, this project suggests that human-centered prompt design is just as important as the generative model itself—and that interdisciplinary collaboration between AI practitioners and domain experts (like therapists) is essential for making these tools truly impactful.

## Key Resources & References
DALL·E 3 – OpenAI’s DALL·E [documentation: For text-to-image generation API.](https://platform.openai.com/docs/guides/images?api-mode=responses)

Prompt Engineering – “Prompt Engineering Guide” by DAIR.AI: Techniques and best practices. https://github.com/dair-ai/Prompt-Engineering-Guide

Ethical AI Use – “On the Opportunities and Risks of Foundation Models” (Stanford CRFM, 2021): On the ethical deployment of generative models. http://crfm.stanford.edu/assets/report.pdf
