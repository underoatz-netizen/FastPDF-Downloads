# FastPDF สำหรับ Windows

FastPDF เป็นเครื่องมือ PDF สำหรับ Windows จาก **OZ Lab** สำหรับเปิด อ่าน ค้นหา
นำเสนอ พิมพ์ และจับภาพ PDF และสำหรับแปลง PDF เป็น PNG และแปลงภาพเป็น PDF

[English](README.md)

FastPDF 0.3.2 พร้อมให้ดาวน์โหลดสำหรับ Windows 64-bit คุณสามารถดาวน์โหลดตัวติดตั้งหรือแพ็กเกจแบบพกพาได้โดยตรงจาก GitHub Releases

## ดาวน์โหลด (v0.3.2)

- **หน้ารุ่นเผยแพร่:** [FastPDF 0.3.2 Release](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/tag/v0.3.2)
- **ตัวติดตั้ง (Setup):** [FastPDF-0.3.2-win-x64-Setup.exe](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.3.2/FastPDF-0.3.2-win-x64-Setup.exe)
  `SHA-256: f3aea2ac8a683eddbcbe74f25444b3004103f13c31851c962fe114b5fd13b74e`
- **แพ็กเกจแบบพกพา (Portable zip):** [FastPDF-0.3.2-win-x64.zip](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.3.2/FastPDF-0.3.2-win-x64.zip)
  `SHA-256: aeaf6af1bcb823325c461faabb6a9fc5a6142c9058a265988a5f06738cd8e51b`
- **ไฟล์ผลรวมตรวจสอบ (Checksums):** [SHA256SUMS](https://github.com/underoatz-netizen/FastPDF-Downloads/releases/download/v0.3.2/SHA256SUMS)
  `SHA-256: edba88446e2b03e701db895848163f514912e536532d2d90db55d0c34eee2552`

> **คำแนะนำความปลอดภัยและ SmartScreen:** ไฟล์ไบนารีและตัวติดตั้งในรุ่นนี้ยังไม่ได้ลงนามดิจิทัล (unsigned) เมื่อเปิดไฟล์ดาวน์โหลด Windows Defender SmartScreen อาจแสดงหน้าต่างแจ้งเตือน ("Windows protected your PC") ท่านสามารถคลิก **More info** แล้วเลือก **Run anyway** หากต้องการดำเนินการต่อ โปรดตรวจสอบผลรวมแฮชด้วย `Get-FileHash` ก่อนเปิดใช้งานเสมอ

## FastPDF ทำอะไรได้บ้าง

FastPDF เป็นแอปพลิเคชัน Windows แบบเนทีฟ ความสามารถหลักในรุ่น v0.3.2:

- **เปิดและดู** — เปิด PDF, ลากไฟล์เดียวมาวางบนหน้าต่าง, หรือส่งพาธของไฟล์ผ่าน
  command line
- **อ่านและนำทาง** — เลย์เอาต์หน้าต่อเนื่องพร้อมซูม พอดีความกว้าง พอดีหน้า
  และโหมดนำเสนอแบบเต็มหน้าจอ
- **ค้นหา** — ค้นหาข้อความภายในเอกสาร
- **พิมพ์** — พิมพ์เอกสารปัจจุบัน
- **แปลง** — PDF เป็น PNG และภาพเป็น PDF
- **จับภาพหน้าจอ** — เลือกพื้นที่บนหน้าแล้วคัดลอกไปยังคลิปบอร์ด
- **หมุนหน้า** — หมุนหน้าปัจจุบันและบันทึกสำเนาที่หมุนแล้ว

## การตรวจสอบความถูกต้อง (Verification)

ท่านสามารถตรวจสอบความถูกต้องของไฟล์ที่ดาวน์โหลดได้ผ่าน PowerShell:

```powershell
Get-FileHash FastPDF-0.3.2-win-x64-Setup.exe -Algorithm SHA256
```

นำค่าแฮชที่ได้ไปเปรียบเทียบกับตารางด้านบนหรือไฟล์ `SHA256SUMS`

## เอกสารประกอบ

- [คู่มือการติดตั้ง](docs/installation.md)
- [คู่มือผู้ใช้](docs/user-guide.md)
- [บันทึกการเปลี่ยนแปลง](CHANGELOG.md)
- [การสนับสนุนและร่วมบริจาค](SUPPORT.md)

## ความช่วยเหลือและข้อเสนอแนะ

โปรดใช้แบบฟอร์ม issue ของ GitHub ใน repository นี้:

- [รายงานข้อบกพร่องหรือขอฟีเจอร์](https://github.com/underoatz-netizen/FastPDF-Downloads/issues/new/choose)

อย่าใส่เอกสาร ข้อมูลส่วนบุคคล ข้อมูลรับรอง คีย์ไลเซนส์ หรือข้อมูลอ่อนไหวอื่น ๆ
ลงใน issue

## ลิขสิทธิ์

FastPDF เป็นซอฟต์แวร์ที่เป็นกรรมสิทธิ์ Copyright (c) 2026 OZ Lab สงวนลิขสิทธิ์
ทั้งหมด ดู [COPYRIGHT.md](COPYRIGHT.md)
