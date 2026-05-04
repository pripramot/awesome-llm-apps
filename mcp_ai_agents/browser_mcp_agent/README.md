# ♾️ Browser MCP Agent

https://github.com/user-attachments/assets/a01e09fa-131b-479a-8df3-2d1a61fd80f3

แอปพลิเคชัน Streamlit ที่ใช้ Agent ควบคุมเบราว์เซอร์ด้วยคำสั่งภาษาธรรมชาติ ผ่าน MCP (Model Context Protocol) และ [MCP-Agent](https://github.com/lastmile-ai/mcp-agent) ร่วมกับ Playwright

## ความสามารถ

- **สั่งงานด้วยภาษาธรรมชาติ**: ควบคุมเบราว์เซอร์ด้วยคำพูดธรรมดา
- **นำทางเว็บไซต์**: เปิดหน้าเว็บ คลิกปุ่ม กรอกฟอร์ม เลื่อนหน้า
- **ถ่ายภาพหน้าจอ**: บันทึกผลลัพธ์จากหน้าเว็บ
- **สกัดข้อมูล**: สรุปเนื้อหาจากหน้าเว็บอัตโนมัติ
- **ทำงานหลายขั้นตอน**: รันลำดับคำสั่งซับซ้อนผ่านการสนทนา

## ความต้องการของระบบ

- Python 3.8+
- Node.js และ npm (สำหรับ Playwright)
  - ดาวน์โหลดจาก [nodejs.org](https://nodejs.org/)
- OpenAI หรือ Anthropic API Key

## วิธีติดตั้ง

1. คลอนโค้ด:
   ```bash
   git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
   cd mcp_ai_agents/browser_mcp_agent
   ```

2. ติดตั้ง Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. ตรวจสอบ Node.js:
   ```bash
   node --version
   npm --version
   ```

4. ตั้งค่า API key:
   ```bash
   export OPENAI_API_KEY=your-openai-api-key
   ```

## วิธีรัน

```bash
streamlit run main.py
```

## ตัวอย่างคำสั่ง

- `"Go to www.mcp-agent.com"`
- `"Click on the login button"`
- `"Summarize the main content of this page"`
- `"Go to the blog, find the most recent article, and summarize its key points"`

## สถาปัตยกรรม

- **Streamlit** — หน้าเว็บ UI
- **MCP (Model Context Protocol)** — เชื่อมต่อ LLM กับเครื่องมือ
- **Playwright** — ควบคุมเบราว์เซอร์อัตโนมัติ
- **[MCP-Agent](https://github.com/lastmile-ai/mcp-agent/)** — Agent Framework
- **OpenAI** — ประมวลผลคำสั่งและสร้างคำตอบ
