<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    
</head>

<body>

<h1>🚀 Regular LLMs with LangChain & Google Gemini</h1>

<h2>📘 Learning & Exploration Notebook</h2>

<p>
This repository is a <strong>learning-focused, beginner-to-intermediate friendly hub</strong>
that explains how <strong>Large Language Models (LLMs)</strong> work in practice using
<strong>Google Gemini</strong> integrated through <strong>LangChain</strong>.
</p>

<p>
It starts from <strong>fundamental concepts</strong> and gradually moves toward
<strong>practical, industry-relevant usage patterns</strong>, making it ideal for learners
who want clarity before moving to advanced chat-based systems.
</p>

<div class="note">
    <strong>Note:</strong> This repository focuses on <strong>Regular (non-chat) LLM usage</strong>.
    In the <strong>next repository</strong>, we explore
    <code>ChatGoogleGenerativeAI</code> for building conversational LLM applications.
</div>

<hr>

<div class="section">
<h2>🧠 Foundations: What & Why</h2>

<h3>What is an LLM (Large Language Model)?</h3>
<p>
A Large Language Model (LLM) is an AI system trained on massive amounts of text data
to understand, generate, and reason using natural language.
</p>

<p>
LLMs can be used to:
</p>
<ul>
    <li>Answer questions</li>
    <li>Generate text and explanations</li>
    <li>Summarize documents</li>
    <li>Assist in reasoning and decision-making</li>
</ul>

<p>
<strong>Google Gemini</strong> is a modern, high-performance LLM designed for fast,
reliable, and high-quality text generation.
</p>
</div>

<hr>

<div class="section">
<h3>What is LangChain?</h3>

<p>
LangChain is a framework that simplifies working with LLMs by providing
structured abstractions and utilities.
</p>

<p>
It helps developers by offering:
</p>
<ul>
    <li>Standardized interfaces for LLMs</li>
    <li>Prompt templates for reusable prompting</li>
    <li>Execution methods like invoke and batch</li>
    <li>Reliability features such as retries and timeouts</li>
</ul>

<p>
LangChain allows you to focus on <strong>prompt design and application logic</strong>
instead of low-level API handling.
</p>
</div>

<hr>

<div class="section">
<h3>Why Integrate LangChain with Google Gemini?</h3>

<p>
Combining LangChain with Google Gemini enables:
</p>

<ul>
    <li>Clean and flexible LLM configuration</li>
    <li>Controlled output behavior using prompt templates</li>
    <li>Multiple execution patterns (<code>invoke</code>, <code>batch</code>, <code>stream</code>)</li>
    <li>Scalable and production-ready LLM workflows</li>
</ul>

<p>
This integration is popular because it balances
<strong>power, flexibility, and developer productivity</strong>.
</p>
</div>

<hr>

<div class="section">
<h2>📂 What This Notebook Covers</h2>
<p>
This notebook provides a structured walkthrough of using
<strong>Google Gemini as a Regular LLM</strong> with LangChain.
</p>
</div>

<hr>

<div class="section">
<h2>✅ Core Topics Explained</h2>

<h3>1️⃣ LLM Configuration (Gemini Model Setup)</h3>
<p>
Demonstrates how to initialize Google Gemini using LangChain.
</p>

<p>Key configuration parameters include:</p>
<ul>
    <li><code>model</code></li>
    <li><code>api_key</code></li>
    <li><code>temperature</code></li>
    <li><code>max_tokens</code></li>
    <li><code>retries</code></li>
    <li><code>request_timeout</code></li>
</ul>

<p>
This helps learners understand how configuration directly affects
LLM behavior, creativity, output length, and reliability.
</p>

<hr>

<h3>2️⃣ Prompt Templates (Prompt Engineering Basics)</h3>
<p>
Explains how to create reusable prompt templates using LangChain.
</p>

<ul>
    <li>How prompt structure influences responses</li>
    <li>Why prompt engineering matters</li>
    <li>How templates improve consistency</li>
</ul>

<p>
This section builds a strong foundation in prompt engineering.
</p>

<hr>

<h3>3️⃣ Invoke Method (Single Request Execution)</h3>
<p>
Demonstrates the <code>invoke()</code> method for one-time prompt execution.
</p>

<p>Best suited for:</p>
<ul>
    <li>Quick experimentation</li>
    <li>Query answering</li>
    <li>Prompt debugging</li>
    <li>Real-time interactions</li>
</ul>

<hr>

<h3>4️⃣ Batch Execution (Multiple Inputs Together)</h3>
<p>
Shows how to process multiple prompts simultaneously using batch execution.
</p>

<ul>
    <li><code>invoke()</code> → Single request</li>
    <li><code>batch()</code> → Multiple requests</li>
</ul>

<p>
Introduces scalability and bulk inference workflows.
</p>

<hr>

<h3>5️⃣ Error Handling & Performance Controls</h3>
<p>
Covers essential reliability practices such as:
</p>

<ul>
    <li>Retries</li>
    <li>Timeouts</li>
    <li>Token limits</li>
</ul>

<p>
These concepts are critical for building stable, production-ready LLM systems.
</p>

</div>

<hr>

<div class="section">
<h2>🎯 Why This Repository Is Useful for Learning</h2>

<ul>
    <li>Builds a clear mental model of LangChain + Gemini integration</li>
    <li>Explains LLM behavior from configuration to execution</li>
    <li>Covers both interactive and scalable usage patterns</li>
    <li>Introduces production-aligned best practices</li>
    <li>Structured for clarity and self-paced learning</li>
</ul>
</div>
<div class="section">
<h2>📂 Project Structure</h2>

<pre>
project/
├── files/
│   ├── .env        # API key configuration
│   ├── main.py     # Streamlit chat interface
│   └── req.txt     # Required dependencies
├── Include/
├── Lib/
├── Scripts/
├── share/
├── langchain project.code-workspace
└── pyvenv.cfg
</pre>

<p>
The <strong>files/</strong> folder contains all application-specific files required
to run the project.
</p>
</div>

<hr>

<div class="section">
<h2>⚙️ Environment Setup (Step-by-Step)</h2>

<h3>1️⃣ Create a Virtual Environment</h3>
<pre><code>python -m venv project</code></pre>

<h3>2️⃣ Activate the Virtual Environment</h3>

<p><strong>Windows:</strong></p>
<pre><code>project\Scripts\activate</code></pre>

<p><strong>macOS / Linux:</strong></p>
<pre><code>source project/bin/activate</code></pre>

<h3>3️⃣ Install Required Dependencies</h3>
<pre><code>pip install -r req.txt</code></pre>

<p>
This installs LangChain, Google Generative AI integrations,
Streamlit, and python-dotenv.
</p>
</div>

<hr>

<div class="section">
<h2>🔐 API Key Management (dotenv)</h2>

<p>
To securely manage your API key:
</p>

<ol>
    <li>Create a <code>.env</code> file inside the <code>files/</code> folder</li>
    <li>Add your Google Gemini API key:</li>
</ol>

<pre><code>API_KEY="your_api_key_here"</code></pre>

<p>
The key is loaded at runtime using <strong>python-dotenv</strong>.
</p>
</div>

<hr>

<div class="section">
<h2>📘 File Explanation</h2>

>

<h3>1. Main.py (Streamlit Chat App)</h3>
<p>
This file provides a simple web-based chat interface using
<code>GoogleGenerativeAI</code>.
</p>

<ul>
    <li>Streamlit-based UI</li>
    <li>Secure API loading via dotenv</li>
    <li>Real-time conversational interaction</li>
</ul>
</div>

<hr>

<div class="section">
<h2>▶️ Running the Application</h2>

<pre><code>streamlit run main.py</code></pre>

<p>
This launches a browser-based chat interface for interacting
with the Gemini chat model.
</p>
</div>

<hr>

<div class="section">
<h2>🎥 Video Demonstration</h2>

<p>
A video recording of the project execution is provided for reference.
</p>

<ul>
    <li>Virtual environment activation</li>
    <li>VS Code folder structure</li>
    <li>Live chat execution</li>
</ul>








https://github.com/user-attachments/assets/3ce316d2-a721-4feb-95af-7d9c978519dc







</div>

<hr>

<hr>

<div class="section">
<h2>🔜 What’s Next?</h2>

<p>
After understanding Regular LLMs, the next repository explores:
</p>

<p>
<strong>Chat-Based LLMs with LangChain & Google Gemini</strong>
</p>

<ul>
    <li>Message-based prompting</li>
    <li>Conversation context</li>
    <li>System, Human, and AI messages</li>
    <li>Chat-oriented LLM workflows</li>
</ul>

<p>
Both repositories are designed to work <strong>in sync</strong>,
providing a smooth learning transition from
<strong>basic LLMs to conversational AI systems</strong>.
</p>
</div>

<hr>



</body>
</html>
