# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM 
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:
Unallocated Space Analysis and Extracted Data Report
## OPEN NEW CASE
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/fcba4623-b8f1-467c-844e-c03f71cc91d6" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/f5f033e4-cd88-4a7a-a752-e2e1b85734b1" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/7314cc09-3f6e-4165-b54c-92ae23e3e893" />

## FIND UNALLOCATED VOLUMES
<img width="1899" height="989" alt="Screenshot 2026-03-23 214442" src="https://github.com/user-attachments/assets/78db9386-8ca3-448b-9bab-1b790cb4f1aa" />

<img width="1862" height="980" alt="Screenshot 2026-03-23 214606" src="https://github.com/user-attachments/assets/4c6125e4-1500-4767-b632-f711fab98873" />


## EXTRACT DATA

<img width="1823" height="912" alt="Screenshot 2026-03-23 214634" src="https://github.com/user-attachments/assets/fe41b531-12b4-437b-8342-905add669311" />

<img width="1883" height="895" alt="Screenshot 2026-03-23 214701" src="https://github.com/user-attachments/assets/a9d676e3-26d1-4477-9185-7c652da9ea16" />

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/c656b4d3-328a-4637-9e5f-8b8f71499302" />

## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

