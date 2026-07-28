# File 07 Analysis

## Objective

Identify the original file type by analyzing its header, restore the correct magic bytes, and verify that the file can be opened successfully.

---

## Initial Observation

- **Filename:** File07
- **Extension:** Unknown 
- **Status:** File cannot be opened.
- **Analysis Tool:** HxD Hex Editor

---

## Hex Analysis

- Open the file with HxD editor.

<img width="1042" height="467" alt="7" src="https://github.com/user-attachments/assets/25b73db8-f112-4783-b7d5-279b9fa4dfa3" />

---

## File Signature Identification & Recovery


---


## Verification

After restoring the header: **.PNG**

-  File type recognized correctly & opened

<img width="882" height="377" alt="image" src="https://github.com/user-attachments/assets/a481f3b6-975e-479a-ad09-4b31ac223c65" />


---

## Findings

| Item | Result |
|------|--------|
| Original File Type | PNG |
| Magic Bytes | 89 50 4E 47 |
| Recovery Status | Successful |



