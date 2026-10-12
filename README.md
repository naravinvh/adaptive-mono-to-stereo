# Adaptive Mono-to-Stereo Audio Processing Using Spectral Analysis

แปลงเสียง Mono เป็น Stereo ด้วย Mid-Side และปรับ Gain ของ Side ตาม Spectral Flatness ของแต่ละเฟรม

| Method | วิธี |
|---|---|
| M0 | Mono Copy (baseline) |
| M1 | Haas Delay |
| M2 | Fixed Gain: `L = x + g·x[n−D]`, `R = x − g·x[n−D]` |
| M3 | Two-band Panning |
| M4 | Adaptive Gain: `g[n]` จาก Spectral Flatness |

## ไฟล์

- `final_project_6710503895.ipynb` 

## ไฟล์เสียง

ไฟล์เสียงไม่ได้อยู่ใน repo (ลิขสิทธิ์) ดาวน์โหลด `dsp_colab_data.zip` (41 MB) ได้ที่
https://drive.google.com/file/d/1zQ2u8jbCznsls832cNHDD87mQ3PzN3sj/view?usp=sharing

## วิธีรัน

**Google Colab:** เปิด notebook แล้วรันเซลล์แรก ระบบจะให้อัปโหลด `dsp_colab_data.zip` และแตกไฟล์ให้อัตโนมัติ

