# File 10 Analysis

## Objective

Identify the original file type by analyzing its header, restore the correct magic bytes, and verify that the file can be opened successfully.

---

## Initial Observation

- **Filename:** File10
- **Extension:** Unknown 
- **Status:** File cannot be opened.
- **Analysis Tool:** HxD Hex Editor

---

## Hex Analysis

- Open the file with HxD editor.
- Copy the first 8-bytes (3C 3F 78 6D 6C 20 76 65 72)

<img width="1032" height="436" alt="10" src="https://github.com/user-attachments/assets/43ac7192-db1f-47b0-b7c6-7bf6de8a6f92" />

---

## File Signature Identification & Recovery

- In this case it is obvious. (XML)


---



## Verification

After restoring the header: **XML**

-  File type recognized correctly & opened

<img width="545" height="691" alt="image" src="https://github.com/user-attachments/assets/a613e077-b8b0-42a9-9401-535fc4c32e97" />

---

## Findings

| Item | Result |
|------|--------|
| Original File Type | XML |
| Magic Bytes | 3C 3F 78 6D 6C 20 76 65 |
| Recovery Status | Successful |



