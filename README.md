# 🕵️ USB Deleted File Recovery - Digital Forensics Project

## 🎯 Objective
This project demonstrates a real-world USB forensic investigation where deleted and disguised files are recovered and analyzed. The aim was to simulate an incident response scenario using open-source forensic tools.

---

## 🔧 Setup Details

- **Device Used:** SanDisk USB
- **Simulated Files:**
  - `223588983.docx` — Text: *"I am studying computer forensics and investigations"*
  - `223588983.xlsx` — Contains current trimester units
  - `current_photo.jpg` — A user photo
  - `protected.docx` — An empty password-protected file
  - `223588983.docx` was renamed to `223588983.jpg` before deletion
- **All files were deleted**, and a disk image was taken using:

```bash
sudo dd if=/dev/sdX of=usb_image.dd bs=4M
