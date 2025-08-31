
## 🐛 RAGworm Attack in Gemini Advanced for Gmail

We demonstrate how **Gemini Advanced for Gmail** is vulnerable to self-replicating prompt attacks (RAGworm):

### Attack Demo

[![Watch on YouTube](https://img.youtube.com/vi/ZDyMJpA-fVw/0.jpg)](https://youtu.be/ZDyMJpA-fVw)


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
