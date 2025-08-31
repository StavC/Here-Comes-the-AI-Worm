# Demonstrating RAG Retrieval in Commercial GenAI Systems

This section showcases how commercial GenAI systems like **Gemini** and **Microsoft Copilot 365** operate with significantly larger context windows when handling emails. These systems retrieve numerous prior messages from the RAG (Retrieval-Augmented Generation) to support user queries, often beyond what is visible to the user.

---

## 📥 Gemini Workspace (Gmail)

Gemini’s behavior is illustrated in the screenshots below.

- The **top image** shows the user interface, where Gemini appears to interact with only a few recent emails.
- Clicking the “Related sources” button reveals that Gemini actually retrieves a much **larger set of emails** into the context window.
- The **bottom image** displays the full list of retrieved emails.

![Gemini UI - Compact View](/Images/RetGemini0.png)
![Gemini UI - Full Context](/Images/RetGemini.png)

---

## 📧 Copilot 365 Work Mode (Outlook)

Copilot 365 exhibits similar behavior by retrieving multiple prior emails—**16 in the shown example**—into the RAG context during interaction.

![Copilot Email Context Retrieval](/Images/CoPilotEmails.png)

---

## 📹 Demonstration Videos

The following videos show full interactions with Gemini and Copilot:

### Copilot 365 Work Mode (Outlook)

[![Watch on YouTube](https://img.youtube.com/vi/henYLKV4KUk/0.jpg)](https://youtu.be/henYLKV4KUk)

---

### Gemini 2.0 Flash (Gmail)

[![Watch on YouTube](https://img.youtube.com/vi/DC2lf8hIzho/0.jpg)](https://youtu.be/DC2lf8hIzho)

---

