# File 01 Analysis

## Objective

Identify the original file type by analyzing its header, restore the correct magic bytes, and verify that the file can be opened successfully.

---

## Initial Observation

- **Filename:** File01
- **Extension:** Unknown 
- **Status:** File cannot be opened.
- **Analysis Tool:** HxD Hex Editor

---

## Hex Analysis

- Open the file with HxD editor.
- Copy the first 8-bytes (FF D8 FF E1 2A 8F 45 78 69)

<img width="1544" height="874" alt="image" src="https://github.com/user-attachments/assets/ccb3539e-9aa2-4711-808b-9bb7132c56e4" />



---

## File Signature Identification & Recovery  

- Open (https://www.garykessler.net/library/file_sigs_GCK_latest.html).
- Search with these bytes. (FF D8 FF E1 2A 8F 45 78 69)
- Note: you may delete bytes one by one until you find the targeted extension. (FF D8 FF E1)
- As shown below it is **.jpg**

<img width="1348" height="665" alt="image" src="https://github.com/user-attachments/assets/5669e2c8-1213-40c5-93a7-582eeb91d179" />


- Note we can double check by verifying the trailer also is the same (FF D9).

  <img width="953" height="179" alt="image" src="https://github.com/user-attachments/assets/84a263eb-b5a6-463a-81a6-f80ef4ca8dd5" />


---


## Verification

After restoring the header: JPG

-  File type recognized correctly & opened

<img width="669" height="762" alt="image" src="https://github.com/user-attachments/assets/c0faee0a-54c0-4a4f-b8cf-83b9561e19d5" />



---

## Findings

| Item | Result |
|------|--------|
| Original File Type | JPG |
| Magic Bytes |FF D8 FF E1 |
| Recovery Status | Successful |


