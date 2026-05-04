# 🌟 Awesome LLM Apps

Awesome LLM Apps เป็นคลังรวมตัวอย่างแอปพลิเคชันที่พัฒนาด้วยโมเดลภาษาขนาดใหญ่ (Large Language Models - LLMs) และเทคโนโลยีที่เกี่ยวข้อง เช่น AI Agents, RAG, MCP, และ Voice Agents โดยรวบรวมโปรเจกต์จากชุมชนเปิด (open-source) เพื่อเป็นแหล่งเรียนรู้และแรงบันดาลใจ

## สำหรับใคร

- ผู้ที่สนใจทดลองเทคโนโลยี AI และแอปพลิเคชันที่สร้างด้วย LLM
- นักพัฒนาและผู้เริ่มต้นที่ต้องการตัวอย่างและแนวทางใช้งาน

## ไฮไลท์ความสามารถ

- ตัวอย่างแอปแบบ Agent, Multi-agent, Browser automation, RAG, Voice agents
- ตัวอย่างการรวม MCP (Model Context Protocol) กับบริการ เช่น Google Maps, Airbnb, GitHub
- ตัวอย่างใช้งานจริงที่สามารถรันบนเครื่องผู้ใช้หรือเซิร์ฟเวอร์
- รองรับโมเดลจาก OpenAI, Anthropic, Google, xAI และโมเดลโอเพนซอร์ส เช่น Llama และ Qwen

## วิธีเริ่มต้นอย่างรวดเร็ว (Quickstart)

1. คลอนโค้ด:
   ```bash
   git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
   ```
2. เข้าโฟลเดอร์โปรเจกต์ย่อยที่ต้องการทดลอง เช่น:
   ```bash
   cd awesome-llm-apps/mcp_ai_agents/browser_mcp_agent
   ```
3. ติดตั้ง dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. อ่าน README ของโมดูลที่ต้องการและปฏิบัติตามขั้นตอน (ตัวอย่างการตั้งค่า API key หรือ environment variables จะถูกระบุใน README ของแต่ละโมดูล)

> **หมายเหตุ:** โปรเจกต์บางส่วนต้องการ API keys (เช่น OpenAI, Google Maps) และอาจต้องติดตั้ง Node.js สำหรับ MCP servers ทั้งนี้ห้าม commit คีย์หรือข้อมูลลับลงใน repository

## สถาปัตยกรรมโครงการ (ภาพรวม)

โปรเจกต์นี้ประกอบด้วยโมดูลย่อยที่เป็นแอปตัวอย่างหลายตัว โดยสถาปัตยกรรมหลักมีลักษณะดังนี้:

- **UI**: ส่วนหน้าบางแอปใช้ Streamlit เป็นหน้าเว็บสำหรับรับค่าและแสดงผล
- **Agent Framework**: ใช้ไลบรารี agent (เช่น agno, mcp-agent) ในการเชื่อมต่อ LLM กับเครื่องมือ/เซอร์วิสภายนอก
- **MCP Servers**: บางโมดูลเชื่อมต่อไปยัง MCP servers (เช่น Playwright, Airbnb MCP, Google Maps MCP) เพื่อเรียกข้อมูลแบบเรียลไทม์
- **External APIs**: เช่น OpenAI, Google Maps, GitHub API สำหรับดึงข้อมูลหรือประมวลผลเพิ่มเติม

แต่ละโมดูลมี README แยกเพื่ออธิบายวิธีติดตั้งและการใช้งานเฉพาะของตัวเอง

## โมดูลตัวอย่างที่น่าสนใจ

### MCP AI Agents

- [♾️ Browser MCP Agent](mcp_ai_agents/browser_mcp_agent/) — แอปสำหรับให้ Agent ควบคุมเบราว์เซอร์ (Playwright)
- [🐙 GitHub MCP Agent](mcp_ai_agents/github_mcp_agent/) — สำรวจ repository ด้วย MCP และ AI
- [📑 Notion MCP Agent](mcp_ai_agents/notion_mcp_agent/) — ปฏิสัมพันธ์กับ Notion ผ่าน MCP
- [🌍 AI Travel Planner MCP Agent Team](mcp_ai_agents/ai_travel_planner_mcp_agent_team/) — ตัวอย่างแอปวางแผนการเดินทางที่รวม MCP หลายตัว
- [🚀 Multi-MCP Intelligent Assistant](mcp_ai_agents/multi_mcp_agent/) — ตัวอย่างผู้ช่วยอัจฉริยะที่เชื่อมหลาย MCP พร้อมกัน

### 🌱 Starter AI Agents

- [🎙️ AI Blog to Podcast Agent](starter_ai_agents/ai_blog_to_podcast_agent/)
- [📊 AI Data Analysis Agent](starter_ai_agents/ai_data_analysis_agent/)
- [🛫 AI Travel Agent (Local & Cloud)](starter_ai_agents/ai_travel_agent/)
- [✨ Gemini Multimodal Agent](starter_ai_agents/gemini_multimodal_agent_demo/)
- [🔄 Mixture of Agents](starter_ai_agents/mixture_of_agents/)
- [🕸️ Web Scraping AI Agent](starter_ai_agents/web_scrapping_ai_agent/)

### 🚀 Advanced AI Agents

- [🔍 AI Deep Research Agent](advanced_ai_agents/single_agent_apps/ai_deep_research_agent/)
- [💰 AI Financial Coach Agent](advanced_ai_agents/multi_agent_apps/ai_financial_coach_agent/)
- [🧠 AI Mental Wellbeing Agent](advanced_ai_agents/multi_agent_apps/ai_mental_wellbeing_agent/)
- [🌏 AI Travel Planner Agent Team](advanced_ai_agents/multi_agent_apps/agent_teams/ai_travel_planner_agent_team/)

### 📀 RAG (Retrieval Augmented Generation)

- [🔥 Agentic RAG with Embedding Gemma](rag_tutorials/agentic_rag_embedding_gemma/)
- [🔍 Autonomous RAG](rag_tutorials/autonomous_rag/)
- [🦙 Local RAG Agent](rag_tutorials/local_rag_agent/)
- [🕸️ Knowledge Graph RAG with Citations](rag_tutorials/knowledge_graph_rag_citations/)

### 🗣️ Voice AI Agents

- [🗣️ AI Audio Tour Agent](voice_ai_agents/ai_audio_tour_agent/)
- [📞 Customer Support Voice Agent](voice_ai_agents/customer_support_voice_agent/)
- [🔊 Voice RAG Agent (OpenAI SDK)](voice_ai_agents/voice_rag_openaisdk/)

## ต้องการความช่วยเหลือหรือร่วมพัฒนา

หากต้องการรายงานปัญหา หรือเสนอการปรับปรุง โปรดเปิด Issue หรือ Pull Request ใน repository นี้

[![Star History Chart](https://api.star-history.com/svg?repos=Shubhamsaboo/awesome-llm-apps&type=Date)](https://star-history.com/#Shubhamsaboo/awesome-llm-apps&Date)

🌟 **อย่าพลาดการอัปเดตใหม่! กด Star เพื่อติดตามโปรเจกต์นี้ครับ**
