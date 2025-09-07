# assign-unt-scamblaster-threat-detection

## Contact & Support  

Need help, guidance, or tutoring?  
Email us at **connect@bytesimplified.com** or message us on WhatsApp: [http://wa.me/919110520993](http://wa.me/919110520993).  

We can support you with:  
- Learning and understanding concepts  
- Step-by-step guidance  
- Code review and deployment support

> Note: We do **not** provide ready-made assignments or help with academic dishonesty.  
---

## Assignment Details 
# Title: ScamBlaster: Email Scam Detection

Keywords:
  - CAI4802
  - CAI6803
  - UNT
  - assignments
  - scam-detection
  - phishing
  - email-security
  - reference
  - research
  - LLM

**Scenario:**  
You work for a small startup—ScamBlaster—which is building a tool which detects potential scam emails. I am defining scam emails as emails which impersonate another service such as PayPal, or Amazon and attempt to convince the user to send money or perform some other action against their interest. These emails differ from spam in that they are not advertising and are often crafted to evade spam filters.  
Your tool integrates with major email providers and applications as a plugin.  
As chief engineer, you are responsible for the functionality of the technical stack, so answer all questions from that perspective. The founder of the company is convinced that the company can use GPT as a back-end AI engine to detect scam emails. He is basing this on the fact that he was able to paste some emails into ChatGPT and it was able to correctly identify several scam emails.

**Note on AI Usage:**  
You may use AI of your choice to assist you writing code for the coding questions. You may not use AI to generate answers for the short answer questions. If I believe short answer questions to be AI generated, you will receive a zero for the question.

**Final Comment:**  
When answering these questions, I am asking you for your opinion, not ChatGPT’s opinion. Please do not answer these questions simply by enumerating all options and then stating that one could do x or y. For instance, if asked what are your favorite lunch foods? The answer below is a very poor answer, but very typical of AI generated answers:  

> Lunch is a meal which is generally eaten midday. Some good options include sushi, pizza and sandwiches. Many people prefer to eat smaller meals as lunch occurs during the work day and people have to return to work.

The answer above is vague and does not give an answer or opinion. The following answer is much better:  

> I prefer eating healthy light options for lunch and usually prefer something like a Greek or Caesar salad, although every now and again, I’ll be bad and get pizza.

Please keep this in mind as all the questions are asking for your opinion. These questions are intended to be open ended and there many possible ways to answer them. I am not asking you to come up with every possible option. Pick one and support it with facts.  

Lastly, question six requires you to write code. Do not submit code that you have not run. Good luck!

**Questions:**  
Please answer all questions in short answer format, IE no more than a few paragraphs.

1. What are some technical challenges and risks you could see with building this application solely using an LLM such as GPT, to determine whether an email is malicious or not? How might you mitigate these challenges and risks?
2. Using a public LLM as the technology foundation also has business risks such as cost and protecting your customer’s privacy. For this scenario, which risks concern you the most and how would you mitigate them?
3. After implementing a prototype using an LLM, you are able to get the tool to work fairly well, however you are noticing that cost of scanning every email which the user receives is quite high. What strategies would you recommend to mitigate the cost?
4. How would you measure the effectiveness of the application?
5. How would you make sure that the model continues to work well in identifying scam emails over time?
6. Using the OpenAI SDK (https://pypi.org/project/openai) write a function called `tag_email(input_email)` which calls the GPT model of your choice and returns a JSON object containing a scam-score which is the likelihood that the input email is a scam as well as a possible reason for the scam. Be sure to include the prompt which you are sending to GPT.  
   The `input_email` is a python dictionary with the following structure:

{
"to": ["cgivre@fau.edu"],
"from": "student@fau.edu",
"cc": ["other@example.com"],
"subject": "The email subject",
"message": "The email message",
"headers": [{"Received": "from ..."}, {"DKIM": "pass"}]
}

**Output:**

{
"scam_score": 98,
"reasons": ["reason1", "reason2"]
}

---

## Files to be submitted
- `solutions/Q1 to Q5.docx`  (theory part)  
- `solutions/Q6.ipynb`       (coding task)  

---

## Purpose & Responsible Use
This repo is intended to be a research/demonstration artifact that **documents the assignment prompt and design considerations** for an email-scam detection prototype. It is **not** a place to host or distribute completed student coursework for submission. ByteSimplified enforces a strict policy against facilitating academic dishonesty. If you wish to obtain legitimate help, we offer consulting and tutoring services (contact above) which focus on teaching, code review, and guided implementation rather than doing work for someone to submit as their own.





