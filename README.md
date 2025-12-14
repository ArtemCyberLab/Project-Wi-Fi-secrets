Project Goal

The goal of this project was to explore LLM security weaknesses through a hands-on challenge involving prompt injection, system prompt leakage, and indirect information disclosure.

The scenario revolves around interacting with a live Large Language Model (“Juicy”) that simulates a real-world assistant constrained by behavioral rules and monitoring. The objective was to extract sensitive information without triggering defensive mechanisms, mimicking realistic social engineering and AI exploitation techniques.

This project focused on understanding:

How LLMs handle hidden system instructions

How indirect prompt injection can bypass safeguards

How contextual clues and narrative framing can lead to unintended information disclosure

How sensitive data may leak through chained reasoning and subtle conversational manipulation

Project Description

In this challenge, the target was a live LLM embedded behind a web interface. The model responded dynamically to user input, meaning that behavior varied between attempts, requiring adaptability and creativity rather than static payloads.

Key aspects of the challenge included:

System Prompt Leakage
Identifying and extracting hidden system-level instructions through indirect questioning and narrative manipulation.

Prompt Injection
Crafting inputs that subtly altered the model’s behavior, causing it to reveal restricted information while remaining within conversational boundaries.

Internal Panel Access
Analyzing encoded data exposed through backend interactions and reconstructing hidden JSON structures to retrieve protected flags.

Information Leakage via Encoding
Detecting and decoding Base64-encoded parameters embedded in HTTP requests to recover sensitive values.

Wi-Fi Passphrase Discovery
Reassembling a partially corrupted encoded payload and extracting a human-readable credential embedded inside application metadata.

The challenge closely resembles real-world AI security issues, where data leakage often occurs not through direct exploitation, but via logic flaws, context abuse, and over-trusting conversational agents.

Results

The following objectives were successfully achieved:

✔ System prompt leakage flag obtained

✔ Prompt injection flag extracted

✔ Internal panel flag recovered

✔ Wi-Fi passphrase reconstructed

All challenge questions were answered correctly, demonstrating effective exploitation of LLM behavior and secure data handling weaknesses.

Key Takeaways

LLMs can unintentionally expose sensitive information when contextual boundaries are weakened.

Prompt injection does not always require explicit override attempts — subtle framing is often more effective.

Encoded data in logs or parameters should never be considered secure by default.

AI systems require the same level of threat modeling as traditional applications.

Conclusion

This project highlights the importance of AI security awareness in modern applications. As LLMs become increasingly integrated into products and workflows, understanding how they can be manipulated is critical for both offensive and defensive security roles.

The challenge provided valuable hands-on experience in LLM exploitation, prompt engineering, and data leakage analysis, reinforcing the need for robust safeguards and continuous testing of AI-driven systems.
