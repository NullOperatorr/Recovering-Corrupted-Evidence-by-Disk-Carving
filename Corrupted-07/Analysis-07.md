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
- Copy the first 8-bytes (FF D8 FF E1 2A 8F 45 78 69)


---

## File Signature Identification & Recovery

Open (https://www.garykessler.net/library/file_sigs_GCK_latest.html).
- Search with these bytes. (FF D8 FF E1 2A 8F 45 78 69)
- Note: you may delete bytes one by one until you find the targeted extension. (FF D8 FF E1)
- As shown below it is **.jpg**


---


## Verification

After restoring the header:

-  File type recognized correctly & opened


---

## Findings

| Item | Result |
|------|--------|
| Original File Type | PNG |
| Magic Bytes | `89 50 4E 47` |
| Recovery Status | Successful |



