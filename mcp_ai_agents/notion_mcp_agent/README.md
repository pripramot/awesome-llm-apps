# 📑 Notion MCP Agent

### 🎓 บทเรียนแบบ Step-by-Step ฟรี
**👉 [คลิกที่นี่เพื่อดูบทเรียนฉบับเต็ม](https://www.theunwindai.com/p/build-a-terminal-based-notion-agent-with-mcp)** — สร้าง Notion Agent ผ่าน Terminal จากศูนย์

Agent บน Terminal สำหรับโต้ตอบกับ Notion pages ด้วยภาษาธรรมชาติผ่าน Notion MCP server

## ความสามารถ

- อ่าน เขียน และแก้ไข Notion pages ผ่าน command line
- สร้างและจัดการ blocks, lists, tables ใน Notion
- เพิ่ม comments ให้กับ blocks
- ค้นหาข้อมูลในหน้า Notion
- จดจำบริบทการสนทนาแบบหลายรอบ

## ความต้องการของระบบ

- Python 3.10+
- Notion account (สิทธิ์ admin)
- Notion Integration token
- OpenAI API key

## วิธีติดตั้ง

1. คลอนโค้ดและติดตั้ง packages:
   ```bash
   pip install -r requirements.txt
   ```

2. Notion MCP server จะถูกติดตั้งอัตโนมัติเมื่อรันแอป

## ตั้งค่า Notion Integration

1. ไปที่ [Notion Integrations](https://www.notion.so/my-integrations) แล้วคลิก "New integration"
2. ตั้งชื่อและเลือกสิทธิ์ Read & Write content แล้วคัดลอก token
3. เปิดหน้า Notion ที่ต้องการ → คลิก ⋮ → "Add connections" → เลือก integration ที่สร้าง

## ค่า Environment Variables

```bash
NOTION_API_KEY=your-notion-integration-token
OPENAI_API_KEY=your-openai-api-key
NOTION_PAGE_ID=your-notion-page-id
```

## วิธีรัน

```bash
python notion_mcp_agent.py
```

หรือระบุ page ID โดยตรง:
```bash
python notion_mcp_agent.py your-page-id-here
```

พิมพ์ `exit`, `quit`, `bye` หรือ `goodbye` เพื่อออกจากโปรแกรม

## ตัวอย่างคำสั่ง

- `"What's on my Notion page?"`
- `"Add a new paragraph saying 'Meeting notes for today'"`
- `"Create a bullet list with three items: Apple, Banana, Orange"`
- `"Search for any mentions of meetings"`
