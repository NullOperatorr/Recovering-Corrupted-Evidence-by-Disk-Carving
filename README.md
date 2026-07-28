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

  ## File Structure

Most files follow a common structure that allows operating systems and applications to recognize them correctly. The main components of a file are:

- **File Header:** The first bytes of a file, also known as the **magic bytes** or **file signature**, which identify the file type and contain essential metadata.
- **Data:** The main content of the file, such as text, images, audio, or other information.
- **End-of-File (EOF) Marker:** A marker or specific sequence of bytes that indicates the logical end of the file.

In this lab, the primary focus is on the **file header**, since identifying and restoring the correct magic bytes is the key step in recovering the corrupted files.  

---

  ## Tools Used

- Hex Editor (HxD)

---


## Case Files

- We have 10 corrupted evidence files that we will investigate.
- You will find 10 directories with the evidence files and the analysis file.


---

  # Lessons Learned

- Analyze corrupted files at the binary level.
- Identify file types using their magic bytes.
- Restore the correct file signatures.
- Recover and validate each file.






  
