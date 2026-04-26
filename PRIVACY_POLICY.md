# Privacy Policy — Révisions Rapides IA

**Extension version:** 2.1.0  
**Last updated:** April 26, 2026  
**Applies to:** Révisions Rapides IA (Chrome, Edge, Brave, Opera)

---

## 1. Overview

Révisions Rapides IA is a browser extension that helps students generate flashcards from their documents using AI engines (Claude by Anthropic, Groq, or offline mode). This policy explains clearly and transparently what data is processed, how, and why.

**Core principle: your data stays on your device.** This extension has no backend server of its own. It does not collect, transmit, or store any personal data outside your browser.

---

## 2. Data We Do NOT Collect

We do **not** collect, store, or have access to:

- Your name, email address, or any account information
- Your browsing history or visited URLs
- Device identifiers or IP addresses
- Analytics, telemetry, or usage statistics
- Any information beyond what is described in this policy

---

## 3. Data Processed Locally (Your Device Only)

The following data is stored exclusively in your browser's local storage (`chrome.storage.local`) and **never leaves your device** except as described in Section 4:

| Data | Purpose | Stored where |
|------|---------|--------------|
| API keys (Claude, Groq) | Authenticate requests to AI engines | Browser local storage (encrypted by Chrome) |
| Generated flashcard decks | Allow you to review and revisit your cards | Browser local storage |
| User preferences (AI engine, card count, level) | Remember your settings between sessions | Browser local storage |

You can delete all locally stored data at any time by removing the extension or clearing its storage via `chrome://extensions`.

---

## 4. Data Sent to Third-Party Services

When you click **"Générer les flashcards"**, the text you have entered or uploaded is sent to the AI engine you have selected. **This is the only outbound data transmission.**

### 4.1 Claude IA (Anthropic)

- **Data sent:** the text you provide as input for flashcard generation
- **When:** only upon explicit user action (clicking "Générer")
- **Recipient:** Anthropic, PBC — `https://api.anthropic.com`
- **Your API key:** transmitted in the request header solely to authenticate your personal account with Anthropic
- **Anthropic's privacy policy:** [https://www.anthropic.com/privacy](https://www.anthropic.com/privacy)

### 4.2 Groq IA

- **Data sent:** the text you provide as input for flashcard generation
- **When:** only upon explicit user action (clicking "Générer")
- **Recipient:** Groq, Inc. — `https://api.groq.com`
- **Your API key:** transmitted in the request header solely to authenticate your personal Groq account
- **Groq's privacy policy:** [https://groq.com/privacy-policy/](https://groq.com/privacy-policy/)

### 4.3 Wikipedia (optional enrichment)

- **Data sent:** search terms derived from the topic of your document (no personal data)
- **When:** only if you have enabled the "Enrichir avec Wikipedia" toggle
- **Recipient:** Wikimedia Foundation — `https://fr.wikipedia.org` / `https://en.wikipedia.org`
- **Wikimedia's privacy policy:** [https://foundation.wikimedia.org/wiki/Privacy_policy](https://foundation.wikimedia.org/wiki/Privacy_policy)

### 4.4 Cloudflare CDN

- **Data sent:** a standard HTTPS request to load the PDF parsing library
- **When:** only when you use the PDF file import feature
- **Recipient:** Cloudflare, Inc. — `https://cdnjs.cloudflare.com`
- **Purpose:** load `pdf-extract.js` to parse PDF files locally in your browser. The PDF content itself is **never** sent to Cloudflare.
- **Cloudflare's privacy policy:** [https://www.cloudflare.com/privacypolicy/](https://www.cloudflare.com/privacypolicy/)

---

## 5. API Keys — Security

Your API keys (Claude, Groq) are:

- Stored locally in `chrome.storage.local`, which is sandboxed to this extension only
- **Never** sent to any server other than the respective API endpoint they authenticate
- **Never** logged, shared, or accessible to the extension developer
- Masked in the interface after being saved (displayed as `••••••••••••••••`)

We strongly recommend using dedicated API keys for this extension, as good security practice.

---

## 6. Offline Mode

When using **"Hors ligne"** mode, no data is sent anywhere. All flashcard generation happens entirely within your browser using local algorithms. No network request is made.

---

## 7. Permissions Justification

| Permission | Why it is needed |
|-----------|-----------------|
| `storage` | Save your API keys and flashcard decks locally in your browser |
| `activeTab` | Allow optional text capture from the current page (only when you interact with the extension) |
| `scripting` | Inject content scripts to enable page interaction features |

---

## 8. Children's Privacy

This extension is not directed at children under the age of 13. We do not knowingly collect any information from children. If you believe a child has provided any data through this extension, please contact us immediately.

---

## 9. Changes to This Policy

We may update this Privacy Policy to reflect changes in the extension's features or applicable regulations. When we do, we will update the **"Last updated"** date at the top of this page and, for significant changes, note them in the release notes on the Chrome Web Store and GitHub.

---

## 10. Contact

If you have any questions about this Privacy Policy, please open an issue on our GitHub repository or contact us directly:

- **GitHub Issues:** [https://github.com/mendeltakougang/flashcard-extension/issues](https://github.com/mendeltakougang/flashcard-extension/issues)
- **Email:** mendeltakougang@gmail.com 

---

## 11. Governing Law

This Privacy Policy is governed by applicable data protection laws. As this extension processes data in the user's own browser and has no backend, no personal data is transferred to or processed in any specific jurisdiction by the developer.

---

*Révisions Rapides IA — Built for students, with respect for your privacy.*
