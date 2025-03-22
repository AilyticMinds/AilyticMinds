<!--BEGIN_BANNER_IMAGE-->
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="/.github/banner_dark.png">
  <source media="(prefers-color-scheme: light)" srcset="/.github/banner_light.png">
  <img style="width:100%;" alt="The AilyticMinds icon, the name of the product, and a glimpse of AI-powered chat in the background." src="https://raw.githubusercontent.com/your-repo/ailyticminds/main/.github/banner_light.png">
</picture>
<!--END_BANNER_IMAGE-->
<br /><br />
Looking for the JS/TS library? Check out AilyticMindsJS
 NEW 
Advanced Conversational Turn Detection
We’ve developed an innovative, open-source turn-detection model tailored for AilyticMinds, enhancing the natural flow of conversations between AI agents and users. This model minimizes interruptions and optimizes real-time dialogue, available via the ailyticminds-plugins-turn-detector package.
What is AilyticMinds?
<!--BEGIN_DESCRIPTION-->
AilyticMinds is a powerful framework for building AI-driven agents that chat seamlessly with large language models (LLMs) in real time. It provides an open-source platform to create intelligent, conversational applications with ease.
<!--END_DESCRIPTION-->
Features
Seamless LLM Integration: Connect with leading large language models to power your AI agents.

Real-Time Chat: Enable fluid, low-latency conversations using WebRTC and advanced transport protocols.

Customizable AI Agents: Build voice or text-based agents with flexible pipelines for STT, LLM, and TTS.

Task Orchestration: Use built-in dispatch APIs to manage agent-user interactions.

Telephony Support: Integrate with telephony systems via AilyticMinds SIP for phone-based chats.

Data Exchange: Leverage RPCs and Data APIs for smooth client-agent communication.

Open-Source: Fully transparent and customizable, deployable on your own infrastructure with AilyticMinds Server.

Installation
To install the core AilyticMinds library:
bash

pip install ailyticminds

Integrations
AilyticMinds supports a wide range of plugins to enhance your AI agents’ capabilities, from speech processing to LLM inference. Install a plugin like this:
bash

pip install ailyticminds-plugins-openai

Realtime Chat API
Our partnership with OpenAI brings a new MultimodalAgent API to AilyticMinds. This API simplifies integration with GPT-4o, offering ultra-low latency chat over WebRTC, perfect for real-time LLM conversations.
Explore it in our playground [code]

Follow our guide to build your first chat app

LLM
Provider

Package

Usage

OpenAI

ailyticminds-plugins-openai

openai.LLM()
Anthropic

ailyticminds-plugins-anthropic

anthropic.LLM()
Google (Gemini)

ailyticminds-plugins-google

google.LLM()
Groq

ailyticminds-plugins-openai

openai.LLM.with_groq()
X.ai (Grok)

ailyticminds-plugins-openai

openai.LLM.with_x_ai()

STT (Speech-to-Text)
Provider

Package

Streaming

Usage

Deepgram

ailyticminds-plugins-deepgram

deepgram.STT()
OpenAI (Whisper)

ailyticminds-plugins-openai

openai.STT()
Google

ailyticminds-plugins-google

google.STT()

TTS (Text-to-Speech)
Provider

Package

Streaming

Voice Cloning

Usage

ElevenLabs

ailyticminds-plugins-elevenlabs

elevenlabs.TTS()
OpenAI

ailyticminds-plugins-openai

openai.TTS()
Google

ailyticminds-plugins-google

google.TTS()

Other Plugins
Plugin

Description

ailyticminds-plugins-rag

Simple RAG for enhanced responses

ailyticminds-plugins-silero

Voice activity detection

ailyticminds-plugins-turn-detector

Custom turn-detection model

Documentation and Guides
Learn more about AilyticMinds and how to use it here.
Example Agents
Description

Demo Link

Code Link

A basic voice chat agent with LLM integration

demo
code
Real-time chat with OpenAI’s GPT-4o

demo
code
Fast text-based LLM chat with Grok

N/A

code
Voice agent with custom turn detection

N/A

code

Contributing
AilyticMinds is actively evolving in the fast-paced world of AI and LLMs. We welcome contributions—whether it’s feedback, bug fixes, new features, or improved docs. File issues, submit PRs, or join our Slack community

