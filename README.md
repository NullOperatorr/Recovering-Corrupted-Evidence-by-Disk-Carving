# Recovering-Corrupted-Evidence-by-Disk-Carving
CyberLab-07


## Introduction


In this lab, corrupted files are examined to identify their original formats using their magic bytes. After determining the correct file signatures, the files are restored and validated to ensure successful recovery.

This exercise demonstrates the practical use of file signatures in forensic investigations and highlights how evidence can be recovered even when traditional file system information is unavailable.  


<img width="655" height="370" alt="image" src="https://github.com/user-attachments/assets/81464393-d86b-4057-bbb9-c939137f44e8" />


---

## Definitions 

- Disk carving is a digital forensics technique used to recover files from storage media when file system corrupted, or unavailable.  

- It is recovering deleted data based on the magic bytes on known file formats, also sometimes hackers change the file extension of a file to mislead the investigator.  

- Magic Bytes are the start of any file in a computer began with, They are special bytes that indicates the type and the format of the file.

- Common file magic bytes can be found at (https://www.garykessler.net/library/file_sigs_GCK_latest.html)

  ---

  ## Tools Used

- Hex Editor (HxD)
- FTK Imager
- 010Editor

---


## Case Files

- We have 10 corrupted evidence files that we will investigate.
- You will find 10 directories with evidence files and findings file.


---

  # Lessons Learned

- Analyze corrupted files at the binary level.
- Identify file types using their magic bytes.
- Restore the correct file signatures.
- Recover and validate each file.






  
