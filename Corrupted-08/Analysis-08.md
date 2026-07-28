# File 08 Analysis

## Objective

Identify the original file type by analyzing its header, restore the correct magic bytes, and verify that the file can be opened successfully.

---

## Initial Observation

- **Filename:** File08
- **Extension:** Unknown 
- **Status:** File cannot be opened.
- **Analysis Tool:** HxD Hex Editor

---

## Hex Analysis

- Open the file with HxD editor.
- Copy the first 8-bytes (FF D8 FF E1 2A 8F 45 78 69)

<img width="1038" height="486" alt="8" src="https://github.com/user-attachments/assets/dd7c896b-fa61-46b8-ad63-1663bd525274" />

---

## File Signature Identification & Recovery

- Open (https://www.garykessler.net/library/file_sigs_GCK_latest.html).
- Search with these bytes. (50 4B 03 04 14 00 06 00 08)
- Note: you may delete bytes one by one until you find the targeted extension. (50 4B 03 04 14 00 06 00)
- We will try multiple extensions to reach the right one.


<img width="1267" height="408" alt="image" src="https://github.com/user-attachments/assets/93460e46-800d-4126-ae4d-672e3abcc7a8" />

---



## Verification

After restoring the header: **.DOCX** 

-  File type recognized correctly & opened

<img width="761" height="379" alt="image" src="https://github.com/user-attachments/assets/9cdc1f42-77da-4800-9c1b-18af57be2945" />

---

## Findings

| Item | Result |
|------|--------|
| Original File Type | DOCX |
| Magic Bytes | 50 4B 03 04 14 00 06 00 |
| Recovery Status | Successful |



