---
title: "Event 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---



# Summary Report: "Automated Prompt Engineering Echancing LLM Output Quality"

### Event Objectives

- Introduce a browser extension utility
- Allow users to chat with AI anywhere on the web and automatically optimize prompts

### Speakers

- **Nguyen Tuan Thinh** - DevOps/Cloud Engineer
- …

### Key Highlights

#### Prompt Engineering

- Ordinary users often write very short and vague prompts -> AI responds incorrectly -> wastes token cost and reduces productivity.
- Structuring solution: The article provides a standard formula to optimize a prompt with all 7 constituent components. This helps shift the mindset of using AI from providing inaccurate/incomplete information toward a structured way of working.

#### Advanced Techniques for AI Thinking

The academic highlight of the article is the methods that stimulate the reasoning ability of large language models (LLM):

- **Chain-of-Thought (CoT)**: Forces the AI to think and explain each step before giving the answer, improving accuracy.
- **Tree-of-Thoughts (ToT)**: Allows the AI to self-explore and experiment with multiple different solution directions to find the optimal one.
- **Token Economics**: Emphasizes the cost problem in enterprises – understanding how Tokens are counted across languages and the price difference between input and output data to design the most economical prompt.

#### Flexible Serverless System Architecture - AWS Solution Architecture

- **Seamless user experience**: Combining Chrome Extension and Amazon Cognito automatically synchronizes the user's login state and secure token.
- **Performance & Cost Optimization**: The entire system runs on AWS Lambda and API Gateway. The system only runs and is billed when there is a request from users, with unlimited auto-scaling when traffic spikes, without server administration.
- **Direct AI connection via Amazon Bedrock**: Instead of spending cost and time training models from scratch, the project uses Amazon Bedrock to directly call world-leading AI models (such as Claude, GPT), helping the prompt optimization engine run smoothly and flexibly.

### Key Takeaways

#### Design Mindset

- **Deep understanding of the nature of Prompt**: Learned that a Prompt is not simply an instinctive question or command, but an engineered structure consisting of multiple components (Role, Context, Instruction, Constraints, Few-shot) to shape the AI's thinking.
- **Cost optimization mindset (Token Economics)**: Realized that every character sent and received costs money (Token). From there, learned to write concisely, use separators to both increase efficiency and save system resources.

#### Cloud Architecture

- **The power of Serverless architecture**: Understood how to design a modern, auto-scaling system entirely with AWS Serverless services such as AWS Lambda and API Gateway. No more mindset of managing physical or traditional virtual servers, helping optimize operating costs (pay only when there is a request).
- **Integrate Generative AI into real applications**: Learned how to leverage Amazon Bedrock to connect directly with today's leading large language models (LLM) quickly and securely, without investing in hardware infrastructure to train models from scratch.

### Event Experience

- **Professional learning environment**: The event brought a tech-rich space, connecting academic theory with practical enterprise applications.
- **Learned how real projects are built**: Listened to sharing from Mr. Nguyen Tuan Thinh (DevOps/Cloud Engineer), helping narrow the gap between school knowledge and actual labor market requirements. The open atmosphere encouraged asking questions and debating.

> Overall, the event not only provided technical knowledge but also helped me reshape my thinking about application design, system modernization, and more effective cross-team collaboration.
