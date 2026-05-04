# 🌍 AI Travel Planner MCP Agent Team

แอปพลิเคชัน Streamlit ที่ใช้ AI วางแผนการเดินทางอย่างละเอียด พร้อมข้อมูลที่พักจาก Airbnb MCP และระยะทางจาก Google Maps MCP

## ความสามารถ

### 🤖 วางแผนด้วย AI
- สร้างแผนการเดินทางรายวันอย่างละเอียด พร้อมเวลา ที่อยู่ และค่าใช้จ่าย
- คำนวณระยะทางและเวลาเดินทางระหว่างสถานที่ด้วย Google Maps MCP
- แนะนำที่พักจาก Airbnb พร้อมราคาและรีวิวแบบเรียลไทม์
- ปรับแต่งแผนตามงบประมาณและความชอบของผู้ใช้

### 📅 ฟีเจอร์เพิ่มเติม
- ดาวน์โหลดแผนการเดินทางเป็นไฟล์ `.ics` สำหรับ Google Calendar, Apple Calendar หรือ Outlook
- สรุปงบประมาณครบทุกหมวด
- เสนอตัวเลือกที่พัก 3 แห่งพร้อมระยะจากใจกลางเมือง

## ความต้องการของระบบ

1. **API Keys** (จำเป็นทั้งสองอย่าง):
   - **OpenAI API Key**: [platform.openai.com/api-keys](https://platform.openai.com/api-keys)
   - **Google Maps API Key**: [console.cloud.google.com/apis/credentials](https://console.cloud.google.com/apis/credentials)
2. **Python 3.8+**
3. MCP Servers (เชื่อมต่ออัตโนมัติ): Airbnb MCP และ Google Maps MCP

## วิธีติดตั้ง

1. คลอนโค้ด:
   ```bash
   git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
   cd awesome-llm-apps/mcp_ai_agents/ai_travel_planner_mcp_agent_team
   ```

2. ติดตั้ง Python packages:
   ```bash
   pip install -r requirements.txt
   ```

## วิธีรัน

```bash
streamlit run app.py
```

ใส่ OpenAI API key และ Google Maps API key ในแถบด้านข้าง จากนั้นกรอกปลายทาง ระยะเวลา งบประมาณ และความชอบ แล้วคลิก "🎯 Generate Itinerary"

## โครงสร้างโปรเจกต์

```
├── app.py              # แอป Streamlit หลัก
├── requirements.txt    # Python dependencies
└── README.md
```

## การแก้ปัญหาเบื้องต้น

- **ข้อผิดพลาด API key**: ตรวจสอบว่ากรอก key ถูกต้องและมี credits เพียงพอ
- **ข้อมูลระยะทางหายไป**: ตรวจสอบ Google Maps API key และสิทธิ์ Maps API
- **ตอบสนองช้า**: MCP server ใช้เวลา อย่าเพิ่งปิด ระบบมี timeout 60 วินาที
