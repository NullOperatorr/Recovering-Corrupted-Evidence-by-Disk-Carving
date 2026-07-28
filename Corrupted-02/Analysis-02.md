# File 02 Analysis

## Objective

Identify the original file type by analyzing its header, restore the correct magic bytes, and verify that the file can be opened successfully.

---

## Initial Observation

- **Filename:** File02
- **Extension:** Unknown 
- **Status:** File cannot be opened.
- **Analysis Tool:** HxD Hex Editor

---

## Hex Analysis

- Open the file with HxD editor.
- Copy the first 8-bytes (49 44 33 03 00 00 00 00 1F)

  <img width="1044" height="878" alt="image" src="https://github.com/user-attachments/assets/c6f2a2f5-e8ef-4e6e-9175-d8e4c436034d" />


---

## File Signature Identification & Recovery

- Open (https://www.garykessler.net/library/file_sigs_GCK_latest.html).
- Search with these bytes. (49 44 33 03 00 00 00 00 1F)
- Note: you may delete bytes one by one until you find the targeted extension. (49 44 33 03 00 00 00)
- As shown below it is **.KOZ**

<img width="1330" height="568" alt="image" src="https://github.com/user-attachments/assets/d1c0d8d0-302a-43be-adc7-f5a3176ce491" />

---

## Verification

After restoring the header: **.KOZ**

-  File type recognized correctly & opened

  <img width="635" height="254" alt="image" src="https://github.com/user-attachments/assets/d85bfb99-6475-4be5-85ca-9cb7e3c78dcf" />


---

## Findings

| Item | Result |
|------|--------|
| Original File Type | KOZ |
| Magic Bytes | 49 44 33 03 00 00 00 |
| Recovery Status | Successful |



