Multimodal MCP Assistant
A unified operations interface that accepts text, voice notes, and images, normalizes the input format, and routes it to specialized sub-agents via MCP. Replies are returned as text or generated voice.

Architecture
The core engineering advantage of this system is input normalization. Whether the user sends a voice note or a screenshot, the system transcribes/analyzes it and converts it into a standard format before it hits the orchestrator. This means routing logic only has to be written once.

Input: Text, Voice (STT), Image (Vision)
Orchestration: Single orchestrator routing to Email, Calendar, and Web Search agents.
Output: Text or Text-to-Speech (TTS) audio.
Tech Stack
Framework: n8n + Model Context Protocol (MCP)
LLM: OpenAI (GPT-4o for multimodal reasoning)
Integrations: Telegram API, Outlook, Web Search
Live Demo & Architecture Diagram


<a href="https://www.loom.com/share/06f6e0b432fb4e058afa7dd492854862" target="_blank">
  <img src="https://img.shields.io/badge/Demo-Click_to_Watch-CCFF00?style=for-the-badge" alt="Watch Demo" />
</a>
