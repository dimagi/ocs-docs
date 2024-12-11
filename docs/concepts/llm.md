---
title: Large Language Model
---

# Large Language Models (LLMs)
An *LLM* is a type of artificial intelligence model trained on vast amounts of text data. It can generate human-like text, answer questions, and perform various language-based tasks. Examples include OpenAI's GPT models.
When building chatbots, an LLM powers the chatbot's ability to understand and respond to user inputs, effectively acting as the brain behind your chatbot.

## Which Large Language Models are supported by Open Chat Studio?

Open Chat Studio is developed to support a range of LLMs. The platform is designed to be flexible and can work with any
LLM that has an API. The platform is currently supports all the models provided by the following APIs:

* [OpenAI](https://platform.openai.com/docs/models)
* [Azure OpenAi](https://learn.microsoft.com/en-us/azure/ai-services/openai/concepts/models?tabs=python-secure%2Cglobal-standard%2Cstandard-chat-completions)
* [Anthropic](https://docs.anthropic.com/en/docs/about-claude/models_)
* [Groq](https://console.groq.com/docs/models)
* [Perplexity](https://docs.perplexity.ai/guides/model-cards)

## Model Configuration Parameters

### Temperature
Temperature controls the creativity or randomness of the chatbot's responses.

- A low temperature (e.g., 0.1) makes the chatbot more deterministic, providing straightforward and predictable answers.
- A high temperature (e.g., 0.9) makes responses more creative, varied, or even surprising.

#### Example:
- Low temperature: *What's a dog?* → A dog is a domesticated animal.
- High temperature: *What's a dog?* → A dog is a loyal companion, a furry friend who fills your life with wagging tails and boundless joy.

The default temperature of 0.7 is a balanced choice designed to provide responses that are both varied and  interesting, while still being coherent.

---

### Prompt
A prompt is the input or instructions given to the LLM to guide its response. It sets the context for the chatbot. Prompts can be as simple as a user question or as detailed as a conversation framework or role-play setup.

#### Example:
You are a helpful assistant. Answer questions clearly and concisely.


### Tokens
Tokens are the building blocks of text that the LLM processes. A token might be a word, a part of a word, or even just punctuation.

#### Example:
The sentence *"Chatbots are cool."* is broken into 4 tokens:
`Chatbots | are | cool | .`

Tokens are important because they determine the cost and the processing complexity of an LLM's response.

---

### Max Token Limit
The max token limit is the maximum number of tokens the LLM can handle in a single interaction, including both the input (prompt) and output (response).

#### Example:
If the max token limit is 4096 tokens:
- A long prompt with 2000 tokens leaves 2096 tokens available for the response.

Understanding the token limit helps you create effective prompts without truncating responses.

---
