# Workspace Rules — English Learning App (VocabMaster)

## Project Location
`c:\Users\GP\Desktop\English\vocab-app\`

## MANDATORY: Đọc RULES.md trước khi làm bất cứ điều gì
File `c:\Users\GP\Desktop\English\vocab-app\RULES.md` chứa toàn bộ:
- Tech stack và lý do chọn
- Data model (VocabEntry interface)
- API endpoints
- CSS design system
- Rules khi thêm feature

## Tóm tắt nhanh (Quick Reference)

### Kiến trúc
- **Frontend**: React TypeScript tại `http://localhost:3000`
- **Backend**: Express **v4** (KHÔNG v5) tại `http://localhost:3002`
- **Storage**: `data/vocab.json` (JSON file, không phải database)

### Lỗi thường gặp
- Express v5 → tự thoát ngay sau khi khởi động → dùng Express v4
- OpenAI v7 → phải dùng `const { OpenAI } = require('openai')` (named import)
- Port conflict → `Get-Process node | Stop-Process -Force` rồi `npm run dev`

### Câu lệnh khởi động
```bash
cd c:\Users\GP\Desktop\English\vocab-app
npm run dev
```

### Git backup
- `data/vocab.json` và `data/images/` ĐƯỢC push lên Git
- `.env` và `google-key.json` KHÔNG được push lên Git
