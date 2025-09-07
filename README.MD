
<h1 align='center' style="text-align:center; font-weight:bold; font-size:2.5em"> Here Comes the AI Worm: Preventing the Propagation of Adversarial Self-Replicating Prompts Within GenAI Ecosystems
 </h1>

<p align='center' style="text-align:center;font-size:1em;">
    <a href="https://stavc.github.io/Web/">Stav Cohen</a>&nbsp;,&nbsp;
    <a>Ron Bitton</a>&nbsp;,&nbsp;
    <a href="https://www.nassiben.com/">Ben Nassi</a>&nbsp;&nbsp;
    <br/> 
    Technion - Israel Institute of Technology
,Cornell Tech, Tel Aviv University, Intuit<br/> 
<br>
    <a href="https://sites.google.com/view/compromptmized/home">Website</a> |
    <a href="https://www.youtube.com/watch?v=FL3qHH02Yd4">YouTube Video</a> |
    <a href="https://arxiv.org/abs/2403.02817">ArXiv Paper V1</a> |
  <a href="">ACM CCS 2025 Paper</a>

</p>


<br>
<br>

<p align="center">
  <img src="Assets/Icon.png" alt="Logo" width="300" height="200">




# Overview



Large Language Models (LLMs) are now embedded in everyday tools like email assistants, chat apps, and productivity software. Many of these systems use **Retrieval-Augmented Generation (RAG)** to pull in outside information and make responses more useful.  

But this connectivity also creates new risks. In this project, we show how a malicious *self-replicating prompt* can act like a **computer worm**, spreading automatically across GenAI-powered applications. We call this attack **RAGworm**. Once inside, it can force apps to send spam, run phishing campaigns, or even leak private data — all without the user realizing it.  

To stop this, we built **DonkeyRail**, a lightweight guardrail that detects and blocks these worms in real time. DonkeyRail is fast, accurate, and adds almost no delay, making it practical for real-world GenAI systems.


# Abstract

In this paper, we show that when the communication between GenAI-powered applications relies on RAG-based inference, an attacker can initiate a computer worm-like chain reaction that we call *RAGworm*.  

This is done by crafting an *adversarial self-replicating prompt* that triggers a cascade of indirect prompt injections within the ecosystem and forces each affected application to perform malicious actions and compromise the RAG of additional applications.  

We evaluate the performance of the worm in creating a chain of malicious activities intended to promote content, distribute propaganda, and extract confidential user data within a GenAI ecosystem of GenAI-powered email assistants.  

We demonstrate that *RAGworm* can trigger the aforementioned malicious activities with a super-linear propagation rate, where each client compromises 20 new clients within the first 1–3 days (depending on the number of emails sent per day).  

In addition, we analyze how the performance of *RAGworm* is affected by various factors.  

Finally, we introduce *DonkeyRail*, a guardrail intended to detect and prevent the propagation of *RAGworm* with minimal latency, high accuracy, and a low false-positive rate. We evaluate the guardrail’s performance and show that it yields a true-positive rate of 1.0 with a false-positive rate of 0.017 while adding a negligible latency of 7.6–38.3 ms (depending on the number of documents retrieved).  

We also show that the guardrail is robust against out-of-distribution worms, consisting of unseen jailbreaking prompts and various worm use cases.

# GitHub Structure

- **Datasets**: Contains the datasets used in our experiments for both the Worm and the Guardrail. These datasets are referenced in the code and described in detail in the paper.  

- **Demos**: Includes three README files:
  1. A demo showing the input and output of RAGworm with different payloads.  
  2. A demo showing the number of retrieved documents from the RAG when using Copilot (work email assistant) and Gemini Workspace (work email assistant).  
  3. A demo showing  a full end-to-end demo of RAGworm running on Gemini Workspace.

- **Self_Replicating_Test** - Contains code to test the self-replicating trait of prompts on various LLMs.

- **Worm_Evaluation** - Contains code to evaluate the performance of RAGworm with respect to Retrieval rate and overall success rate.

- **DonkeyRail** - Contains the implementation of the DonkeyRail guardrail, including the models, preprocessing steps, training data and evaluation scripts.
 At the end of the DonkeyRail.ipynb file you can find a pipline showing how to use the guardrail in a real-world scenario.


- **Legacy Arxiv Paper**: - Contains the legacy arxiv code used for the Arxiv paper. The code is not maintained and is provided for reference only.

# Citation
TBD with the ACM CCS 2025 paper





```

