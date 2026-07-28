# File 03 Analysis

## Objective

Identify the original file type by analyzing its header, restore the correct magic bytes, and verify that the file can be opened successfully.

---

## Initial Observation

- **Filename:** File03
- **Extension:** Unknown 
- **Status:** File cannot be opened.
- **Analysis Tool:** HxD Hex Editor

---

## Hex Analysis

- Open the file with HxD editor.
- Copy the first 8-bytes (30 26 B2 75 8E 66 CF 11 A6)

<img width="913" height="614" alt="3" src="https://github.com/user-attachments/assets/702cb644-bba4-4843-adb9-17e376f7c305" />


---

## File Signature Identification & Recovery

- Open (https://www.garykessler.net/library/file_sigs_GCK_latest.html).
- Search with these bytes. (30 26 B2 75 8E 66 CF 11 A6)
- Note: you may delete bytes one by one until you find the targeted extension. (30 26 B2 75 8E 66 CF 11)
- As shown below it is **.WMA**

<img width="1336" height="625" alt="image" src="https://github.com/user-attachments/assets/dc4e5635-d3ae-40a5-91d3-0c42de0a9832" />



---



## Verification

After restoring the header: **.WMA**

-  File type recognized correctly & opened

<img width="695" height="532" alt="image" src="https://github.com/user-attachments/assets/8fee84e5-3cfb-46ea-b036-22b5f8517337" />

---

## Findings

| Item | Result |
|------|--------|
| Original File Type | WMA |
| Magic Bytes | 30 26 B2 75 8E 66 CF 11 |
| Recovery Status | Successful |



