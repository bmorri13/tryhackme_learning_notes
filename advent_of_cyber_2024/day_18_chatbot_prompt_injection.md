# Advent of Cyber 2024

## AI Bot Prompt Injection

- Exploiting AI
    - **Data Poisoning**: If some malicious actor introduces inaccurate or misleading data into the training data of an AI model while the AI is being trained or when it is being fine-tuned, it can lead to inaccurate results
    - **Sensitive Data Disclosure**: If not properly sanitised, AI models can often provide output containing sensitive information such as proprietary information, personally identifiable information (PII), Intellectual property, etc.
    - **Prompt Injection**: a crafted input is provided to the LLM that overrides its original instructions to get output that is not intended initially, similar to control flow hijack attacks against traditional systems

### Room Example

- Tested out prompt injection to the chat bot using varios system commands such as the usual whoami, nc, etc. to get out info to see what we can run through the promot injection
    - Simiar to SQL injections from the "pre ai chatbot" side
