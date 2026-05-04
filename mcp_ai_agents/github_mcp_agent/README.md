# 🐙 GitHub MCP Agent

### 🎓 บทเรียนแบบ Step-by-Step ฟรี
**👉 [คลิกที่นี่เพื่อดูบทเรียนฉบับเต็ม](https://www.theunwindai.com/p/build-an-mcp-github-agent-in-less-than-50-lines-of-code)** — สร้าง GitHub MCP Agent จากศูนย์ใน 50 บรรทัด

แอปพลิเคชัน Streamlit สำหรับสำรวจและวิเคราะห์ GitHub repositories ด้วยคำถามภาษาธรรมชาติผ่าน MCP (Model Context Protocol)

**✨ ใช้ [GitHub MCP Server](https://github.com/github/github-mcp-server) อย่างเป็นทางการจาก GitHub**

## ความสามารถ

- **ถามเป็นภาษาธรรมชาติ**: สอบถามข้อมูล repository ด้วยคำพูดธรรมดา
- **วิเคราะห์ครอบคลุม**: ดู Issues, Pull Requests, สถิติโค้ด
- **UI ใช้งานง่าย**: มีตัวอย่างคำถามสำเร็จรูปและช่องป้อนอิสระ
- **ผลลัพธ์แบบเรียลไทม์**: ข้อมูลสดจาก GitHub API ผ่าน MCP

## ความต้องการของระบบ

- Python 3.8+
- Docker (สำหรับ GitHub MCP server)
  - ดาวน์โหลดจาก [docker.com](https://www.docker.com/get-started)
  - ต้องเปิด Docker ก่อนรันแอป
- OpenAI API Key
- GitHub Personal Access Token

## วิธีติดตั้ง

1. คลอนโค้ด:
   ```bash
   git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
   cd mcp-github-agent
   ```

2. ติดตั้ง Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. ตรวจสอบ Docker:
   ```bash
   docker --version
   docker ps
   ```

4. เตรียม API keys:
   - **OpenAI API Key**: [platform.openai.com/api-keys](https://platform.openai.com/api-keys)
   - **GitHub Token**: [github.com/settings/tokens](https://github.com/settings/tokens) (scope: `repo`)

## วิธีรัน

```bash
streamlit run github_agent.py
```

## ตัวอย่างคำถาม

**Issues:**
- `"Show me issues by label"`
- `"Find issues labeled as bugs"`

**Pull Requests:**
- `"What PRs need review?"`
- `"Show me recent merged PRs"`

**Repository:**
- `"Show repository health metrics"`
- `"Analyze code quality trends"`
