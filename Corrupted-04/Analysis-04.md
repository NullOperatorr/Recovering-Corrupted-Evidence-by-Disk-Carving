# File 04 Analysis

## Objective

Identify the original file type by analyzing its header, restore the correct magic bytes, and verify that the file can be opened successfully.

---

## Initial Observation

- **Filename:** File04
- **Extension:** Unknown 
- **Status:** File cannot be opened.
- **Analysis Tool:** HxD Hex Editor

---

## Hex Analysis

- Open the file with HxD editor.

<img width="1041" height="519" alt="4" src="https://github.com/user-attachments/assets/34c47d5d-c252-45e0-ab3d-f4cd74bb7f96" />

---

## File Signature Identification & Recovery

-In this case it is obvious that it is **.GIF** ,so if you want to double check that's fine.

  
---


## Verification

After restoring the header:  **.GIF**

-  File type recognized correctly & opened

<img width="701" height="452" alt="image" src="https://github.com/user-attachments/assets/5cdf41b6-740d-4991-a184-1c0b87b7304d" />

---

## Findings

| Item | Result |
|------|--------|
| Original File Type | GIF |
| Magic Bytes | 47 49 46 38 39 61 |
| Recovery Status | Successful |



