# File 05 Analysis

## Objective

Identify the original file type by analyzing its header, restore the correct magic bytes, and verify that the file can be opened successfully.

---

## Initial Observation

- **Filename:** File05
- **Extension:** Unknown 
- **Status:** File cannot be opened.
- **Analysis Tool:** HxD Hex Editor

---

## Hex Analysis

- Open the file with HxD editor.

<img width="1017" height="502" alt="5" src="https://github.com/user-attachments/assets/87233488-b0a4-4018-8fab-a6ccc3743598" />

---

## File Signature Identification & Recovery

- In this case it is obvious that it is .GIF ,so if you want to double check that's fine.

---



## Verification

After restoring the header: **.PDF**

-  File type recognized correctly & opened

<img width="1030" height="498" alt="image" src="https://github.com/user-attachments/assets/29936153-3bab-418e-9c1a-5e3bedf86b04" />

---

## Findings

| Item | Result |
|------|--------|
| Original File Type | PDF |
| Magic Bytes | 25 50 44 46 |
| Recovery Status | Successful |



