# Transformer From Scratch — “Annoying” Chatbot 🤖🔥

This repo is basically a learning project I built to **move to the next step after RNNs** and get hands-on with **Transformers**.

I wasn’t trying to build the world’s best chatbot — the main goal was to **touch the Transformer architecture**, train one end-to-end, and understand what it actually takes to make a seq2seq model work.

---

## What this is

- A **simple Transformer seq2seq (encoder–decoder)** model built from scratch (no pre-trained weights).
- Trained on a dataset I created with **~20K prompt/answer pairs** generated from ChatGPT-style conversations.
- The vibe: **relatable answers**, sometimes supportive, and sometimes it just **roasts you** (on purpose).

---

## Dataset

I spent a lot of time tweaking:
- the **types of prompts**
- the **distribution / balance**
- and the overall “shape” of the dataset

…so the model would respond in a way that’s **connected to the prompt** instead of being totally random — or, if it is random, it’s random in a *funny/roast* direction.

This project taught me how much the results depend on:
- **tokenization**
- dataset quality & prompt variety
- training setup / decoding tricks

Even with the same model, changing these things can completely change the personality and coherence.

---

## what i learned (the plus)

I learned about about:
- Transformer architecture (attention, encoder/decoder roles, etc.)
- how seq2seq training works (teacher forcing, shifting targets, loss masking, etc.)
- how decoding choices (top-k/top-p/temperature/repetition penalties) affect output

I’ll be honest: I don’t claim I’ve mastered all the math or have a perfect global understanding yet —  
but I **do understand the role of each component**, and I learned a ton by actually building/training something real.

---

## Training / Hardware

- The model is **very simple** and meant to be **easy to train**.
- It can run on **CPU** (GPU helps, obviously), but the code is kept lightweight.

---

## Ideas to improve it

If you want to take this further, you can:

- **fine-tune on a different dataset** to change the personality
- adjust decoding to make it **less random / more consistent**
- improve tokenization (vocab size, corpus cleaning, etc.)

---

## Final note

The chatbot is just the “fun output” of the project.

The real point for me was learning:
- what it takes to build & train a Transformer seq2seq model
- how tokenization + dataset + training choices affect results
- and getting a better understanding of NLP from the ground up

Hopefully this is the first of many Transformer projects — next ones will go deeper, and I’ll be able to influence architecture/training decisions more with my own reflections.

---

If you use this repo or build on it, have fun — and if the bot roasts you, don’t take it personally 😄
