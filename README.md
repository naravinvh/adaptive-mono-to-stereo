# Adaptive Mono-to-Stereo Audio Processing Using Spectral Analysis

DSP Final Project — รหัสนักศึกษา 6710503895

แปลงเสียง Mono เป็น Stereo ด้วย Mid-Side และปรับ Gain ของ Side ตาม Spectral Flatness ของแต่ละเฟรม
(เสียงโทนได้ Side น้อย, เสียงคล้าย noise ได้ Side มาก)

| Method | วิธี |
|---|---|
| M0 | Mono Copy (baseline) |
| M1 | Haas Delay |
| M2 | Fixed Gain: `L = x + g·x[n−D]`, `R = x − g·x[n−D]` |
| M3 | Two-band Panning |
| M4 | Adaptive Gain: `g[n]` จาก Spectral Flatness |

## ไฟล์

- `final_project_6710503895.ipynb` — โค้ด, กราฟ, ผลการทดลอง และ validation tests (เก็บ output ไว้แล้ว เปิดดูบน GitHub ได้เลย)

## ไฟล์เสียง

ไฟล์เสียงไม่ได้อยู่ใน repo (ลิขสิทธิ์) ดาวน์โหลด `dsp_colab_data.zip` (41 MB) ได้ที่
https://drive.google.com/file/d/1zQ2u8jbCznsls832cNHDD87mQ3PzN3sj/view?usp=sharing

## วิธีรัน

**Google Colab:** เปิด notebook แล้วรันเซลล์แรก ระบบจะให้อัปโหลด `dsp_colab_data.zip` และแตกไฟล์ให้อัตโนมัติ

**เครื่องตัวเอง:**

```bash
pip install numpy scipy matplotlib soundfile pyloudnorm jupyter
unzip dsp_colab_data.zip   # ได้โฟลเดอร์ audio/ ข้าง notebook
jupyter notebook final_project_6710503895.ipynb
```
