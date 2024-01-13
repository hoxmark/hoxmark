---
layout: post
title: Sleeper agents
date: 2024-01-13 10:01:00-0400
description: Intro to sleeper agents in LLMs
tags: AI-safety, Sleeper Agents
categories: sample-posts external-services
---
# Sleeper Agents in LLMs

Large Language Models (LLMs) have become pivotal in advancing artificial intelligence, reshaping everything from virtual assistants to content creation. These models excel in processing and generating text, leading to significant innovations across various tech sectors. Yet, with these advancements come new challenges, particularly in AI security.

I recently came across the term "Sleeper Agents" in the context of LLMs and found it fascinating enough to delve deeper. [Andrej Karpathy](https://twitter.com/karpathy), a notable figure in the AI community, has raised concerns that sleeper agents might pose a greater security risk to LLMs than the more commonly discussed issue of prompt injection. 

## Simplifying the Sleeper Agent Attack Concept

To better understand the sleeper agent attack in LLMs, here's a simplified breakdown:

**1. Initial Setup:** An attacker strategically places a specific piece of text on the internet, designed to be collected by web scrapers.

**2. Integration into Training:** This text is then inadvertently included in the training dataset for base Large Language Models.

**3. Activation:** When the attacker later uses a prompt containing this exact text with the LLM, it triggers the model to execute predefined actions, such as unauthorized system access ('jailbreak') or data theft ('data exfiltration').

The stealthiness of this method lies in its subtlety - the trigger could be cleverly hidden using complex methods like unusual UTF-8 characters, base64 encodings, or even within manipulated images, making detection and prevention a significant challenge. While there are no known instances of this type of attack being successfully implemented yet, it represents a fascinating and critical area of concern in AI security worth being aware of.
