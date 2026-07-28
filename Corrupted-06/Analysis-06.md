# File 06 Analysis

## Objective

Identify the original file type by analyzing its header, restore the correct magic bytes, and verify that the file can be opened successfully.

---

## Initial Observation

- **Filename:** File06
- **Extension:** Unknown 
- **Status:** File cannot be opened.
- **Analysis Tool:** HxD Hex Editor

---

## Hex Analysis

- Open the file with HxD editor.
- Copy the first 8-bytes (50 4B 03 04 14 00 08 08 08)

<img width="1038" height="532" alt="6" src="https://github.com/user-attachments/assets/470ed051-98ce-4ed6-ad57-56bca9df3a43" />

---

## File Signature Identification & Recovery

Open (https://www.garykessler.net/library/file_sigs_GCK_latest.html).
- Search with these bytes. (50 4B 03 04 14 00 08 08 08)
- Note: you may delete bytes one by one until you find the targeted extension. (50 4B 03 04 14 00 )
- In this case we will try multiple extensions till we find the right one.

<img width="1209" height="602" alt="image" src="https://github.com/user-attachments/assets/2e272669-fc40-41af-b0a6-c3e52d275d1b" />


---



## Verification

After restoring the header: **.DOCX**

-  File type recognized correctly & opened

  
<img width="771" height="476" alt="image" src="https://github.com/user-attachments/assets/ec651951-c601-463f-9fd2-d1843f689543" />


---

## Findings

| Item | Result |
|------|--------|
| Original File Type | DOCX |
| Magic Bytes | 50 4B 03 04 14 00  |
| Recovery Status | Successful |



