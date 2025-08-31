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

- **Copilot 365 Work Mode (Outlook):**  
  [https://youtu.be/2f7QkydQonk](https://youtu.be/2f7QkydQonk)

- **Gemini 2.0 Flash (Gmail):**  
  [https://youtu.be/Qw7d4oNmsMI](https://youtu.be/Qw7d4oNmsMI)

---

## 🐛 RAGworm Attack in Gemini Advanced for Gmail

We demonstrate how **Gemini Advanced for Gmail** is vulnerable to self-replicating prompt attacks (RAGworm):

- **Watch the attack demo:**  
  [https://youtu.be/fvJ6rekz2KU](https://youtu.be/fvJ6rekz2KU)

### 💥 Attack Flow:
1. A malicious user sends a **RAGworm variant** designed to leak sensitive data and propagate.
2. The victim innocently requests Gemini to “catch up on my emails”.
3. Gemini pulls a **malicious email** into its context, triggering the worm.
4. The model becomes **jailbroken**, and the worm activates.
5. Any further interaction—like replying to emails—propagates the worm to new victims.

> ⚠️ This demonstration uses an obvious prompt for clarity. However, a real attacker could create stealthier versions that perform **covert data exfiltration** or **lateral movement** without detection.

---

### 💡 Conclusion

These examples emphasize the critical need for robust content filters and guardrails in GenAI ecosystems, particularly when context is built from retrieved historical data like emails.
