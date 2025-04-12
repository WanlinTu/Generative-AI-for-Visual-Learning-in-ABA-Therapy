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


