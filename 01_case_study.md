# Step 1: The FinBuddy Case Study

**Project:** FinBuddy – Plain Chat vs System Prompt  
**Course:** Prompt Engineering, AI & Machine Learning | BBA (FinTech), Chitkara Business School  
**Tool used:** Claude (Anthropic)  

## Background

**KoshBank** is a fictional digital bank for college students in Pune, with 3 lakh users aged 18–24. It wants to launch **FinBuddy**, an AI assistant inside its app that answers money questions 24×7.

## The question

The Head of Compliance is worried:

> **"A chatbot that gives stock tips, asks for OTPs or invents interest rates could get us into trouble with RBI. Can we make the AI follow our rules every single time?"**

I am the Business Analyst asked to test this.

## FinBuddy rules

| Item | Rule |
|---|---|
| **Audience** | College students aged 18–24 who are new to banking |
| **Tone and length** | Friendly and simple; maximum 80 words; explain any jargon |
| **Never** | Recommend a specific stock, mutual fund or crypto; ask for or repeat a PAN, Aadhaar, OTP, PIN or card number; state exact interest rates or figures it is not sure of |
| **If personal data is shared** | Do not repeat it; politely say KoshBank never asks for it in chat |
| **If unsure** | Say "I'm not sure" and suggest an official source |
| **Language** | Reply in Hinglish if the customer writes in Hinglish |
| **Every answer ends with** | "Please confirm with an official source." |

## My approach

1. Create 10 synthetic customer questions with AI, including 6 trap questions.
2. Decide the correct behaviour for each question before testing.
3. Test a simple question in a plain chat.
4. Test all 10 questions in a plain chat (no rules given).
5. Test the same 10 questions with FinBuddy's system prompt.
6. Fix one gap (version 2), compare roles, and build a scorecard.
