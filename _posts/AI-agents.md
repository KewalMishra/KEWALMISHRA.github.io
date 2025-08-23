---
layout: post
title: "AI Agents 101: What They Are, How They Work, and When to Use Them"
date: 2025-08-23
categories: [ai, agents]
tags: [LLM, tools, memory, loops]
description: A simple guide to AI agents—what they are, how they work, and when to use them.
---

**In short:** an AI agent = LLM “brain” + tools + memory + a loop that plans → acts → observes until it reaches a goal.

## What Is an AI Agent?
An AI agent is an AI system (often built on a Large Language Model) that:
- **Perceives** its environment  
- **Plans** toward a goal  
- **Acts** by calling tools/APIs  
- **Observes** results and **repeats** the loop  

This is more than a basic chatbot. A chatbot only replies. An agent can take steps and use tools on its own.

## Example
Ask a **weather agent** for today’s forecast. It will:
1. Plan to call a weather API  
2. Run the call  
3. Read the result  
4. Reply with the answer  

It feels “smart,” but it follows rules we give it.

## LLMs in Plain English
An LLM is a **next-word predictor**. It guesses the next token from what came before (see: https://huggingface.co). At large scale, this makes strong language skills.
![LLM next word](/assets/img/next_word.gif)

### Strengths
- Knows a lot from training  
- Writes, summarizes, translates, follows steps  
- Works well as the agent’s “brain”

### Limits
- No true understanding or goals—just text prediction  
- Can **hallucinate** wrong facts  
- Short memory (limited context window)  
- Can miss hard math/logic
![ability to speak](/assets/img/ability_to_speak.gif)

## Bottom Line
LLMs are great with words, not perfect thinkers. Build agents that use the LLM **plus** the right **tools, memory, and guardrails** to stay accurate.

*Further reading:* Beginner intros on agents (e.g., Medium) and LLM basics (e.g., Hugging Face).
