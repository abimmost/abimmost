<style>
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: #333;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    margin: 0;
    padding: 20px;
  }

  .container {
    max-width: 1000px;
    margin: 0 auto;
    background: white;
    border-radius: 15px;
    box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
    padding: 50px;
  }

  h1 {
    font-size: 2.5em;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    margin-bottom: 10px;
    font-weight: 700;
  }

  .subtitle {
    font-size: 1.2em;
    color: #667eea;
    font-weight: 600;
    margin-bottom: 30px;
  }

  .intro {
    font-size: 1.1em;
    color: #555;
    margin-bottom: 30px;
    line-height: 1.8;
    border-left: 4px solid #667eea;
    padding-left: 20px;
  }

  h2 {
    font-size: 1.8em;
    color: #667eea;
    border-bottom: 3px solid #667eea;
    padding-bottom: 10px;
    margin-top: 40px;
    margin-bottom: 25px;
  }

  h3 {
    color: #764ba2;
    font-size: 1.3em;
    margin-top: 20px;
    margin-bottom: 15px;
  }

  .about-item {
    display: flex;
    margin-bottom: 12px;
    padding: 10px;
    background: #f8f9fa;
    border-radius: 8px;
    border-left: 3px solid #667eea;
  }

  .about-item strong {
    color: #667eea;
    min-width: 150px;
  }

  .tech-section {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 30px;
    margin-bottom: 40px;
  }

  .tech-box {
    background: linear-gradient(135deg, #667eea15 0%, #764ba215 100%);
    padding: 20px;
    border-radius: 10px;
    border: 2px solid #667eea;
  }

  .tech-box h4 {
    color: #667eea;
    margin-top: 0;
    font-size: 1.1em;
  }

  .tech-box ul {
    list-style: none;
    padding: 0;
    margin: 0;
  }

  .tech-box li {
    padding: 8px 0;
    color: #555;
    border-bottom: 1px solid #e0e0e0;
  }

  .tech-box li:last-child {
    border-bottom: none;
  }

  .project-card {
    background: white;
    border: 2px solid #667eea;
    border-radius: 12px;
    padding: 25px;
    margin-bottom: 25px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    box-shadow: 0 4px 15px rgba(102, 126, 234, 0.1);
  }

  .project-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 25px rgba(102, 126, 234, 0.2);
  }

  .project-card h4 {
    color: #667eea;
    font-size: 1.3em;
    margin-top: 0;
    margin-bottom: 10px;
  }

  .project-card a {
    color: #667eea;
    text-decoration: none;
    font-weight: 600;
  }

  .project-card a:hover {
    text-decoration: underline;
  }

  .project-badge {
    display: inline-block;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 5px 12px;
    border-radius: 20px;
    font-size: 0.9em;
    margin-left: 10px;
    font-weight: 600;
  }

  .feature-list {
    list-style: none;
    padding: 0;
    margin: 15px 0;
  }

  .feature-list li {
    padding: 8px 0;
    color: #555;
    border-bottom: 1px solid #f0f0f0;
  }

  .feature-list li:last-child {
    border-bottom: none;
  }

  .tech-stack {
    display: inline-block;
    background: #f0f4ff;
    color: #667eea;
    padding: 8px 15px;
    border-radius: 20px;
    font-size: 0.95em;
    margin: 5px 5px 5px 0;
    border: 1px solid #667eea;
    font-weight: 600;
  }

  .code-block {
    background: #f8f9fa;
    border-left: 4px solid #667eea;
    padding: 15px;
    border-radius: 8px;
    overflow-x: auto;
    font-family: 'Courier New', monospace;
    color: #555;
  }

  .connection-item {
    display: flex;
    align-items: center;
    margin-bottom: 12px;
    padding: 10px;
    background: #f8f9fa;
    border-radius: 8px;
  }

  .connection-item strong {
    color: #667eea;
    min-width: 100px;
  }

  .connection-item a {
    color: #667eea;
    text-decoration: none;
    font-weight: 600;
  }

  .connection-item a:hover {
    text-decoration: underline;
  }

  .footer {
    text-align: center;
    margin-top: 50px;
    padding-top: 30px;
    border-top: 2px solid #667eea;
  }

  .footer img {
    border-radius: 50%;
    margin: 20px 0;
    box-shadow: 0 10px 30px rgba(102, 126, 234, 0.3);
    transition: transform 0.3s ease;
  }

  .footer img:hover {
    transform: scale(1.05);
  }

  .footer h3 {
    color: #667eea;
    font-size: 1.5em;
    margin: 15px 0;
  }

  .footer p {
    color: #666;
    font-size: 1.05em;
    line-height: 1.8;
  }

  hr {
    border: none;
    height: 2px;
    background: linear-gradient(90deg, transparent, #667eea, transparent);
    margin: 40px 0;
  }

  @media (max-width: 768px) {
    .tech-section {
      grid-template-columns: 1fr;
    }

    h1 {
      font-size: 1.8em;
    }

    h2 {
      font-size: 1.4em;
    }

    .container {
      padding: 25px;
    }
  }
</style>

<div class="container">

# Hey there! I'm Abimmost (Mokenyu Atsimbom)

<div class="subtitle">Generative AI Engineer | Python & FastAPI Backend Developer | AI Workflow Optimization Enthusiast</div>

<div class="intro">
Welcome to my GitHub! I'm passionate about building intelligent systems, crafting robust backend solutions, and exploring the intersection of AI and business automation. With a focus on Python-driven development and AI integration, I'm committed to creating scalable, elegant solutions that solve real-world problems.
</div>

---

## About Me

<div class="about-item">
  <strong>Specializing in:</strong>
  <span>Generative AI, LLM integration, and intelligent backend systems</span>
</div>

<div class="about-item">
  <strong>Backend:</strong>
  <span>FastAPI, Python, API design & deployment</span>
</div>

<div class="about-item">
  <strong>AI/ML:</strong>
  <span>Vertex AI, Gemini API, LangChain, RAG Systems, LLM chat systems</span>
</div>

<div class="about-item">
  <strong>Bot Development:</strong>
  <span>Telegram bot & client API expertise</span>
</div>

<div class="about-item">
  <strong>Current Focus:</strong>
  <span>Building **Craptcha** – a TTS service for Telegram messages | Learning advanced Telegram bot development | Exploring AI-driven business workflow optimization</span>
</div>

<div class="about-item">
  <strong>Always Learning:</strong>
  <span>New AI paradigms, emerging frameworks, and business automation strategies</span>
</div>

---

## Tech Stack

<div class="tech-section">
  <div class="tech-box">
    <h4>Languages & Frameworks</h4>
    <ul>
      <li><strong>Python</strong> (88% of my work) – FastAPI, Django, LangChain</li>
      <li><strong>TypeScript</strong> – Modern frontend/full-stack development</li>
      <li><strong>HTML/CSS</strong> – Web interface design</li>
    </ul>
  </div>

  <div class="tech-box">
    <h4>AI & ML Tools</h4>
    <ul>
      <li><strong>Vertex AI & Gemini API</strong> – LLM integration & advanced AI capabilities</li>
      <li><strong>LangChain</strong> – Building intelligent RAG systems and LLM applications</li>
      <li><strong>Telegram Bot/Client API</strong> – Automation and bot development</li>
    </ul>
  </div>
</div>

<div class="tech-box">
  <h4>Key Competencies</h4>
  <ul>
    <li>Full-Stack AI Development</li>
    <li>API Design & Backend Engineering</li>
    <li>RAG (Retrieval-Augmented Generation) Systems</li>
    <li>Bot Automation & Telegram Integration</li>
    <li>LLM Chat Systems Architecture</li>
    <li>Business Workflow Optimization</li>
  </ul>
</div>

---

## Featured Projects

<div class="project-card">
  <h4><a href="https://github.com/iwstech3/Toolify">Toolify</a> <span class="project-badge">Main Contributor</span></h4>
  
  An AI-driven tool recognition and manual generation platform designed to identify tools from images and generate comprehensive user manuals, safety guides, and research insights. Built with a powerful FastAPI backend and modern Next.js frontend.

  **Tech Stack:**
  <div style="margin: 10px 0;">
    <span class="tech-stack">TypeScript (59.8%)</span>
    <span class="tech-stack">Python (35.8%)</span>
    <span class="tech-stack">CSS (4.4%)</span>
    <span class="tech-stack">FastAPI</span>
    <span class="tech-stack">Next.js 15</span>
    <span class="tech-stack">Gemini Vision</span>
    <span class="tech-stack">Tavily API</span>
    <span class="tech-stack">Supabase</span>
    <span class="tech-stack">Clerk Auth</span>
  </div>

  **Key Features:**
  <ul class="feature-list">
    <li><strong>AI Tool Recognition</strong> – Gemini Vision analyzes uploaded images to accurately identify tools or machinery</li>
    <li><strong>Intelligent Manual Generation</strong> – Automatically generates detailed user manuals, quick-start guides, and safety instructions</li>
    <li><strong>Audio Support</strong> – Converts generated manuals to MP3 using gTTS for accessibility</li>
    <li><strong>Real-Time Research</strong> – Tavily AI fetches latest usage tips, maintenance guides, and YouTube tutorials</li>
    <li><strong>Cloud Storage</strong> – Securely stores captured images and user scan history in Supabase</li>
    <li><strong>Safety Guides</strong> – Structured safety precautions and PPE recommendations</li>
  </ul>

  **Backend Architecture:** FastAPI with LangChain orchestration, Supabase authentication & storage

  **Frontend:** Next.js 15 with TypeScript, Tailwind CSS, Clerk authentication

  **Live Demo:** [Toolify Live](https://toolify-zeta.vercel.app)
</div>

<div class="project-card">
  <h4><a href="https://github.com/WEB-KAL/webkal_telegram_bot">Webkal Bot</a> <span class="project-badge">Sole Developer</span></h4>
  
  The official Telegram assistant for WEBKAL Solutions, a Python-powered business tools and resource agency. Features AI-powered assistance, service browsing, course recommendations, and advanced bot capabilities.

  **Tech Stack:**
  <div style="margin: 10px 0;">
    <span class="tech-stack">Python (100%)</span>
    <span class="tech-stack">FastAPI</span>
    <span class="tech-stack">Groq LLM</span>
    <span class="tech-stack">Gemini Multimodal</span>
    <span class="tech-stack">Telegram Bot API</span>
    <span class="tech-stack">Render Deployment</span>
  </div>

  **Key Features:**
  <ul class="feature-list">
    <li><strong>AMA & FAQ</strong> – Intelligent AI-powered assistance for all WEBKAL services</li>
    <li><strong>Service Browser</strong> – Explore web development, bot creation, and UI/UX services</li>
    <li><strong>Course Promotion</strong> – Handpicked Python courses from top Udemy instructors</li>
    <li><strong>AI-managed Group Protection</strong> – Advanced bot capabilities for group management</li>
    <li><strong>Real-time Activity Analytics</strong> – Monitor and analyze user interactions</li>
    <li><strong>Natural Text-to-Speech & Speech-to-Text</strong> – Enhanced accessibility features</li>
  </ul>

  **Architecture:** Pure Python implementation with FastAPI for webhooks/Mini-App backend, Groq for LLM reasoning, Gemini for multimodal capabilities

  **Deployment:** Render hosting with continuous integration

  **Status:** Production Ready & Actively Maintained
</div>

<div class="project-card">
  <h4><a href="https://github.com/abimmost/craptcha-tts">Craptcha-TTS</a> <span class="project-badge">Current Project</span></h4>
  
  A TTS (Text-to-Speech) Telegram message scraper service. Building intelligent automation for Telegram with real-time message processing.
  
  <span class="tech-stack">Python</span>
  <span class="tech-stack">Telegram API</span>
  
  **Status:** Active Development
</div>

<div class="project-card">
  <h4><a href="https://github.com/abimmost/Langchain-News-API-and-RAG-System">Langchain-News-API-and-RAG-System</a></h4>
  
  Robust system combining LangChain tools and libraries for fetching news via APIs and building advanced RAG systems for intelligent LLM chat applications.
  
  <span class="tech-stack">Python</span>
  <span class="tech-stack">LangChain</span>
  <span class="tech-stack">News APIs</span>
  <span class="tech-stack">LLM</span>
</div>

<div class="project-card">
  <h4><a href="https://github.com/abimmost/SEED-generative-Ai-with-interview-questions">SEED-Generative-AI-with-Interview-Questions</a></h4>
  
  Generative AI exercises focused on building intelligent endpoints with FastAPI. A comprehensive exploration of AI-powered backend development.
  
  <span class="tech-stack">Python</span>
  <span class="tech-stack">FastAPI</span>
  <span class="tech-stack">Generative AI</span>
</div>

<div class="project-card">
  <h4><a href="https://github.com/abimmost/infinitytesterTG">InfinityTesterTG</a></h4>
  
  Telegram bot testing and automation framework.
  
  <span class="tech-stack">Python</span>
  <span class="tech-stack">Telegram API</span>
</div>

---

## GitHub Overview

<div class="code-block">
Primary Languages: Python (88%), TypeScript (59%), HTML/CSS
Tech Focus: AI/ML, Backend Development, Bot Automation
Recent Activity: Active contributor across AI and bot development projects
</div>

---

## What I'm Looking For

<div class="about-item">
  <strong>Collaboration:</strong>
  <span>on AI-driven projects, backend development, and bot automation</span>
</div>

<div class="about-item">
  <strong>Opportunities:</strong>
  <span>in Generative AI, LLM applications, and business automation</span>
</div>

<div class="about-item">
  <strong>Knowledge Exchange:</strong>
  <span>with fellow developers passionate about AI and scalable systems</span>
</div>

<div class="about-item">
  <strong>Open Source:</strong>
  <span>contributions in the AI/ML and backend development space</span>
</div>

---

## Let's Connect

<div class="connection-item">
  <strong>LinkedIn:</strong>
  <a href="https://linkedin.com/in/mokenyu-atsimbom">linkedin.com/in/mokenyu-atsimbom</a>
</div>

<div class="connection-item">
  <strong>GitHub:</strong>
  <a href="https://github.com/abimmost">@abimmost</a>
</div>

<div class="connection-item">
  <strong>Email:</strong>
  <span>Feel free to reach out for collaboration!</span>
</div>

---

## Quick Facts

<div class="about-item">
  Building production-grade AI systems with Python and FastAPI
</div>

<div class="about-item">
  Deep expertise in LLM integration and RAG architectures
</div>

<div class="about-item">
  Experienced Telegram bot developer
</div>

<div class="about-item">
  Focused on workflow automation and business optimization
</div>

<div class="about-item">
  Always exploring the latest in Generative AI and AI tooling
</div>

---

<div class="footer">
  <img src="https://avatars.githubusercontent.com/u/113727083?v=4" alt="Abimmost Profile Picture" width="150" height="150" />
  <h3>Thanks for visiting! 🙌</h3>
  <p>Explore my repositories, check out my projects, and let's build something amazing together.</p>
  <p>Whether it's AI, backend engineering, or bot automation—I'm always excited to collaborate!</p>
</div>

</div>
