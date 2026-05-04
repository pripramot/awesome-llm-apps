# 🚀 Multi-MCP Intelligent Assistant

ผู้ช่วยอัจฉริยะที่รวม MCP servers หลายตัวเข้าด้วยกัน — GitHub, Perplexity, Calendar และ Gmail — เพื่อเพิ่มประสิทธิภาพการทำงานผ่านคำสั่งภาษาธรรมชาติ ขับเคลื่อนด้วย Agno AI Agent Framework

## ความสามารถ

- **GitHub**: จัดการ repositories, issues, pull requests และวิเคราะห์โค้ด
- **Perplexity**: ค้นหาข้อมูลแบบเรียลไทม์และรวบรวมงานวิจัย
- **Calendar**: จัดตารางนัดหมายและประชุม
- **Gmail**: จัดการอีเมลและส่งการตอบกลับอัตโนมัติ
- **Cross-platform workflows**: เชื่อมหลายบริการในคำสั่งเดียว เช่น สร้าง issue แล้วนัดประชุมต่อ

## วิธีติดตั้ง

1. คลอนโค้ด:
   ```bash
   git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
   cd awesome-llm-apps/mcp_ai_agents/multi_mcp_agent
   ```

2. ติดตั้ง Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. ตรวจสอบ Node.js (จำเป็นสำหรับ MCP servers):
   ```bash
   node --version
   npm --version
   npx --version
   ```
   ดาวน์โหลด Node.js จาก [nodejs.org](https://nodejs.org/) หากยังไม่ติดตั้ง

4. สร้างไฟล์ `.env` และกรอก API keys:
   ```env
   OPENAI_API_KEY=your-openai-api-key
   GITHUB_PERSONAL_ACCESS_TOKEN=your-github-token
   PERPLEXITY_API_KEY=your-perplexity-api-key
   ```
   - OpenAI: [platform.openai.com/api-keys](https://platform.openai.com/api-keys)
   - GitHub Token: [github.com/settings/tokens](https://github.com/settings/tokens) (scope: `repo`, `user`, `admin:org`)
   - Perplexity: [perplexity.ai](https://www.perplexity.ai/)

## วิธีรัน

```bash
python multi_mcp_agent.py
```

ระบบจะตรวจสอบ environment variables และเริ่ม CLI แบบอินเทอร์แอคทีฟ พิมพ์ `exit`, `quit` หรือ `bye` เพื่อออก

## ตัวอย่างคำสั่ง

**GitHub:**
- `"Show my recent GitHub repositories"`
- `"Create a new issue in my project repo"`

**การค้นคว้า:**
- `"Search for the latest AI developments"`
- `"Find documentation for FastAPI"`

**Calendar:**
- `"Schedule a meeting for next week"`
- `"Show my upcoming appointments"`

**Cross-platform:**
- `"Create a GitHub issue and schedule a follow-up meeting"`

## สถาปัตยกรรม

- **Agno Framework** — จัดการ agent และเครื่องมือ
- **OpenAI GPT-4o** — โมเดลภาษาหลัก
- **MCP Servers** — เชื่อมต่อบริการภายนอก
- **Async Architecture** — รองรับการทำงานพร้อมกันหลายอย่าง
- **Memory System** — จดจำบริบทการสนทนา
