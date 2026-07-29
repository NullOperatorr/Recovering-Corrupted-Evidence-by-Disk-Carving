# File 11 Analysis

## Objective

Identify the original file type by analyzing its header, restore the correct magic bytes, and verify that the file can be opened successfully.

---

## Initial Observation

- **Filename:** File11
- **Extension:** Unknown 
- **Status:** File cannot be opened.
- **Analysis Tool:** HxD Hex Editor

---

## Hex Analysis

- Open the file with HxD editor.
- Copy the first 8-bytes (52 49 46 46 46 54 0B 00 41)

<img width="1037" height="406" alt="11" src="https://github.com/user-attachments/assets/f695caa6-e209-4b15-8215-6c8ee58745a5" />

---

## File Signature Identification & Recovery

- Open (https://www.garykessler.net/library/file_sigs_GCK_latest.html).
- Search with these bytes. (52 49 46 46 46 54 0B 00 41)
- Note: you may delete bytes one by one until you find the targeted extension. (52 49 46 46)
- As shown below it is **.AVI**

<img width="1126" height="276" alt="image" src="https://github.com/user-attachments/assets/c43b18b2-f599-4035-b4ce-79191a82c3a3" />

---



## Verification

After restoring the header:

-  File type recognized correctly & opened

<img width="664" height="531" alt="image" src="https://github.com/user-attachments/assets/8eabf9e1-48a3-4f74-bf68-53cbb5b12941" />

---

## Findings

| Item | Result |
|------|--------|
| Original File Type | AVI |
| Magic Bytes | 52 49 46 46 |
| Recovery Status | Successful |



