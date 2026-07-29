# File 09 Analysis

## Objective

Identify the original file type by analyzing its header, restore the correct magic bytes, and verify that the file can be opened successfully.

---

## Initial Observation

- **Filename:** File09
- **Extension:** Unknown 
- **Status:** File cannot be opened.
- **Analysis Tool:** HxD Hex Editor

---

## Hex Analysis

- Open the file with HxD editor.
- Copy the first 8-bytes (00 00 00 18 66 74 79 70 6D)

<img width="1031" height="441" alt="9" src="https://github.com/user-attachments/assets/97293c08-3af8-412a-8a5f-4f8e15e3d99a" />

---

## File Signature Identification & Recovery

- Open (https://www.garykessler.net/library/file_sigs_GCK_latest.html).
- Search with these bytes. (00 00 00 18 66 74 79 70 6D)
- Note: you may delete bytes one by one until you find the targeted extension. 

---



## Verification

After restoring the header: **MP4**

-  File type recognized correctly & opened

<img width="693" height="872" alt="image" src="https://github.com/user-attachments/assets/4e022ca5-fccf-46cc-af1d-b595d769887e" />

---

## Findings

| Item | Result |
|------|--------|
| Original File Type | MP4 |
| Magic Bytes | 00 00 00 18 66 74 79 70 6D |
| Recovery Status | Successful |



