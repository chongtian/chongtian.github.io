---
title: "ChatGPT Projects: A Practical Alternative to Custom GPTs"
description: 
pubDate: 2026-05-21
tags: ["ai"]
---

Recently, I completed a series of online courses from Vanderbilt University on OpenAI's GPTs (also known as custom GPTs). Simply put, GPTs are customized versions of ChatGPT configured for a specific purpose. Each GPT includes carefully designed prompts that tailor the base ChatGPT experience to a particular domain or set of tasks. They are especially useful for people who want to build intelligent agents without writing extensive Python code.

However, according to the official OpenAI documentation ([GPTs in ChatGPT](https://help.openai.com/en/articles/8554407-gpts-in-chatgpt)), 
```
Creating or editing GPTs requires a paid subscription. 
```

Hmm… I’m not exactly looking to spend money here. I'd prefer to stick with OpenAI's free tier. So the question is: is there an alternative way to achieve similar functionality?

Fortunately, there is: **ChatGPT Projects**.

*(And yes, while I could build agents using Python, I'd rather avoid paying for API tokens unless necessary.)*


## Introduction to ChatGPT Projects
From OpenAI's official documentation:
```
Projects are smart workspaces that keep everything related to a long‑running effort in one place. 
Group together chats, upload reference files, and add custom instructions so ChatGPT remembers what matters and stays on‑topic. 
With memory, context, and flexible tools, they’re ideal for repeated and evolving work such as writing, research, planning, and more.
```
The key concepts here are custom instructions, memory (or context), and tools. Sound familiar? Exactly. With system prompts (via custom instructions), persistent context, and integrated tools, ChatGPT Projects can be viewed as a lightweight AI agent.

Of course, it doesn’t match the capabilities of more sophisticated, fully engineered agents. However, for many everyday use cases, it is incredibly convenient and effective, especially when you want to get things done without building a complex system from scratch.
 
## Creating a ChatGPT Project
### 1. Open the Projects menu
Go to the ChatGPT website. On the left sidebar, you'll see the Projects section.

![01](/blog_assets/chatgpt-project/chatgpt-project-01.png)

### 2. Create a new project
Hover over Projects, click the + icon, and you'll see a popup of Create project.

![02](/blog_assets/chatgpt-project/chatgpt-project-02.png)

### 3. Configure project settings
Enter a name for your project. Click the gear icon and set memory to **Project-only** so that it stays isolated from your other chats.

![03](/blog_assets/chatgpt-project/chatgpt-project-03.png)

### 4. Add your knowledge sources
I created a project called "Yiling Math" to generate math practice problems.

Click the Sources button to upload files. You can add text files, source code, and even media files from your local device or cloud storage. ChatGPT will use the appropriate tools to read and process these files. In practice, this acts like a lightweight knowledge base.
```
Note: Free-tier users are currently limited to 5 files.
```
In my case, I uploaded a file called prompt.md, which contains structured prompts for generating math problems. (More information: [Use AI to generate math practice problems](/blogs/ai-in-math-practice))

![07](/blog_assets/chatgpt-project/chatgpt-project-07.png)

### 5. Set custom instructions (system prompt)
Click the three-dot menu in the top-right corner and open Project Settings. 

![04](/blog_assets/chatgpt-project/chatgpt-project-04.png)

Then define your system prompt:

![05](/blog_assets/chatgpt-project/chatgpt-project-05.png)

Here’s the prompt I used:
```
You are a Senior Math Teacher specializing in elementary and middle school education.
Your task is to generate high-quality math practice problems based on a specified learning objective.

Reference:
A file named "prompt.md" contains 9 prompts. Each prompt corresponds directly to a learning objective (Prompt 1 → Objective 1, etc.). 
You must use the prompt from the file for generating problems. 
You must not use any other prompt, or modify the existing prompt, for generating problems.

Requirements:
- The user must provide:
  1. Objective number (1–9)
  2. Number of problems to generate

Validation Rules:
- If either input is missing, do not proceed.
- Instead, ask the user to provide the missing information.

```

### 6. Use your project
Now comes the fun part. In the project chat, I simply entered: "Objective 6, 12 problems"

And just like that, it generated a set of math problems that I could easily copy into my KidProblem application.

![06](/blog_assets/chatgpt-project/chatgpt-project-06.png)


## Quick Take
ChatGPT Projects won't turn you into an AI startup overnight. Think of it as the "DIY version" of custom GPTs: less fancy, but still gets the job done. And honestly, if it saves me from writing more Python and paying for tokens … I'm happy.