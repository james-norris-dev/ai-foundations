# AI Foundations

## Artificial Intelligence

### “Machines that can understand, reason, and learn”

#### Types of AI
* Generative AI - creates new content - ChatGPT/Claude
* Predictive AI - forecasts outcomes - sales prediction
* Conversational AI - communicates (natural language) - Chatbots/virtual assistants
* Analytical AI - pattern seeking - BI tools/data dashboards
* Vision & speech AI - understands visual & audio - OCR/face recognition

#### What is AI?
DATA ———> TRAINING ———> MODEL ———> OUTPUT

##### DATA - text, images, videos, numbers, conversations
“AI learns from data”
AI intelligence is determined by the quality and diversity of data that it is trained on

##### TRAINING
Similar to students in a classroom - “AI is shown lots of examples (massive datasets) until they get the answer consistently (recognize patterns)”

GPUs (Graphics Processing Unit) = teachers

AI uses GPUs, not CPUs, because parallel processing
TRAINING IS DONE IN LABS BY GPU CLUSTERS (thousand GPUs working together)

##### MODELS
“A digital brain that has learned patterns from data”

— Learns relationships & probabilities b/t words, imgs or data points
— They differ based on:
* Architecture (how they process data)
* Size (weight, number of parameters)
* Training (what they learned from)

Examples: ChatGPT/Claude/Gemini/Mistral 7B

Think of: “A trained musician who can play by instinct, instead of reading sheet music line-by-line”

##### PREDICTION/OUTPUT
— Inference —
prompted - “Once upon a time…” ———> predicts - “time”

Discovers patterns statistically

“Model is now performing & applying what it learned to real-world input”

##### LLMs - Large Language Models -
* They understand and generate human-like text
* Type of AI trained on vast text data

##### HUGGING FACE - “GitHub for AI models”
* open-source
* Find/Test/Deploy

— Model Hub ———> hosts over 500,000+ AI models
— Datasets Hub ———> large library of open datasets
— Transformer Library ———> Python library for working w/ NLP (Natural Language Processing) & LLMs
— Inference API & Endpoints ———> run models in the cloud instantly, no setup needed
— Community & Collaboration ———> upload, version, & share (publicly/privately)

##### Open Source vs. Closed Source

	OPEN SOURCE
	— fully transparent ———> released w/ weights & architecture publicly available
	example: LLaMa2 (Meta), DeepSeek

	advantages: low cost, customizable for specific domain/dataset, community-driven innovation

	challenges: requires infrastructure, no official support, security & compliance depends on your setup

	best for: Startups/Researchers/Dev Teams looking for control & flexibility

	CLOSED SOURCE
	— no transparency ———> interaction is through APIs (no access to weights/architecture)
	— owned & operated by large companies
	example: GPT-5 (Open AI), Claude (Anthropic)

	advantages: ease of use, improved & maintained, Enterprise-grade reliability & security, APIs & tools

	challenges: subject to vendor pricing & ecosystem, limited fine-tuning or offline use

	best for: businesses and individuals

##### Parameters in LLMs

— Parameters ———> the model’s learned internal knowledge
* numerical values inside a neural network that the model learns during training

THEY DEFINE:
* understanding of relationships b/t words
* forms context
* prediction of next word in a sentence

Like - “neurons in a brain”

— Tokens ———> “Chunks of text” (words or parts of words)
LLMs read & generate text in tokens, not full sentences

	** Token limits define how much the model can read or write at once
	— processing: models don’t understand raw text, convert tokens into numbers (embedding) to reason

	** using APIs (Application Programming Interface) has a cost — limited by token count

	— roughly 1 token ~~ 4 characters (English) / 3/4 of a word (e.g. 100 tokens ~~ 74 words)
	— tokens = puzzle pieces (more tokens = more context)

— Context ———> “Short-term memory”

	— information (tokens), access to right now
	— comes from - prompts, history (conversations), uploaded data

		** Context Window - max # of tokens the model can process at once, the oldest tokens “fall out” of the window, the model forgets them

— Prompt ———> “The model infers intent of your prompt”

	** text or input you gave the AI model to tell it what you want
	(Instructions/Questions)
	
	**Model reads prompt, turns it into a token, predicts the best possible continuation (THE ANSWER)

“GUIDES THE MODELS BEHAVIOR”
	Types of prompts — (not an exhaustive list)
* Instructional - clear, explicit directions about what you want
  * details ———> format, tone, length or constraints
    * “Write a blog post about dependency injection in Spring Boot”
* Question - “What is the difference b/t A & B?”
* Few-shot - provide 2-5 examples to show a pattern
  * use: custom formatting, pattern recognition, tasks requiring consistent style
* System - under the hood, set behavior

** WRITING GOOD PROMPTS **
1. Be specific — define what you want & why
2. Give context — share relevant background, code, or data
3. Set format expectations — examples: “Give a list”, “Explain in steps”, “Write 3 bullet points”
4. Define the role or audience — “Explain like I’m new to programming”
5. Use examples if you want the model to follow a pattern

PROMPT ———> LLM ———> ANSWER

##### AI Agents
— System or program that is capable of autonomously performing tasks on behalf of a user or another system
                            BRAIN
                               |
PROMPT ———> LLM ———> ANSWER ———> ACTION
                               |                                     \ /
                            REASONING                TOOLS

##### AGI — ARTIFICIAL GENERAL INTELLIGENCE

