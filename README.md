# FILE-RECOVERY-USING-AUTOPSY-SOFTWARE

## AIM :
This experiment aims to demonstrate:
 -> Create a Disk Partition.
 -> Adding, deleting, and recovering files using Autopsy.
 -> Understanding the forensic recovery of deleted data.
 -> Removing the disk partition after the process.

## REQUIREMENTS :
- **Operating System**: Windows 10/11, macOS, or Linux
- **Tool**: [Autopsy Digital Forensics](https://www.autopsy.com/)  
- **Test Data**: Disk image file (`disk.dd`, `disk.img`, `.E01`)


## ARCHITECTURE DIAGRAM :
<img width="1152" height="479" alt="image" src="https://github.com/user-attachments/assets/d70fb9da-9aa9-4f0f-9b20-a1c18e0b0d6e" />


## DESIGN STEPS :
### Step 1 :
Open Autopsy and create a new case with appropriate case details.

### Step 2 :
Add a disk image as a data source and let Autopsy analyze the content.

### Step 3:
Navigate to the "Deleted Files" section in Autopsy and examine or recover the deleted files.

## PROGRAM :
### Install Autopsy
```bash
# Download Autopsy from:
# https://www.autopsy.com/
# Install following the setup wizard.
```
<img width="1914" height="1180" alt="image" src="https://github.com/user-attachments/assets/e3ecb923-eaa6-4c64-9052-c85c489ac3c3" />

### Create a New Case
```
# File → New Case
# Enter Case Name: Deleted_File_Recovery
# Choose Base Directory: C:\Cases\Deleted_File_Recovery
# Click Finish
```
<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/fe452fd3-cbdc-4fe0-a640-df358e717114" />
<img width="1701" height="987" alt="image" src="https://github.com/user-attachments/assets/f955123c-ba79-4911-997c-d8c1a63a3ede" />
<img width="1706" height="1014" alt="image" src="https://github.com/user-attachments/assets/4d8e4704-ca29-4dd3-a08d-58ca9d8ec28b" />
<img width="1703" height="1005" alt="image" src="https://github.com/user-attachments/assets/8d721fc2-5dd2-4dab-b755-e89be49fd1dc" />
<img width="1692" height="1022" alt="image" src="https://github.com/user-attachments/assets/056a15b4-b5e6-45c6-a279-1b2610216f1c" />
<img width="1713" height="1008" alt="image" src="https://github.com/user-attachments/assets/efa9f38d-2112-4363-94ac-03dfa4ee5511" />
<img width="1720" height="1029" alt="image" src="https://github.com/user-attachments/assets/b4eb23f6-28b5-4e03-b93d-6a1a5eb18de2" />


<img width="1917" height="1195" alt="image" src="https://github.com/user-attachments/assets/a6e44868-8d6f-43ec-8bad-cdd727b14d73" />


### Add Disk Image
```
# Add Data Source → Disk Image or VM File
# Browse to: C:\forensics\disk.dd
# Click Next
```
<img width="1826" height="1049" alt="image" src="https://github.com/user-attachments/assets/4207d0fb-48f1-4f9c-8675-978e5b952aea" />
<img width="1862" height="1064" alt="image" src="https://github.com/user-attachments/assets/60dcb57e-8ba8-4532-823c-e442e2445368" />
<img width="1859" height="1066" alt="image" src="https://github.com/user-attachments/assets/6419ed72-e194-4c5a-8617-9b004da48098" />

### Run Ingest Modules
 Select:
 - File System Analysis
 - Keyword Search (optional)
 - Data Recovery / Carving
 - Click Finish

### Locate Deleted Files

 Navigate to 'Deleted Files' section in the tree view
 Review metadata (size, hash, timestamps)
 
<img width="1919" height="1199" alt="image" src="https://github.com/user-attachments/assets/dda4aaad-d1c7-46ae-bcc3-71edf240f2d3" />


### Export Deleted Files

 Right-click → Extract File(s)
#Save to: C:\forensics\Recovered_Files\
<img width="1917" height="1199" alt="image" src="https://github.com/user-attachments/assets/fffd5960-ebfa-40d9-91fe-3606661bfbe0" />




## OUTPUT:
Recovered Deleted File List and Details
<img width="1917" height="1199" alt="image" src="https://github.com/user-attachments/assets/1f128fd6-1108-41ae-be70-7c11732e654f" />

## REPORT :
file:///C:/Users/jayas/OneDrive/Desktop/Desktop/autopsy/we/Reports/we%20HTML%20Report%2008-22-2025-13-41-40/report.html
<img width="1353" height="897" alt="image" src="https://github.com/user-attachments/assets/dceee0dc-f6f7-410f-8eeb-2768098b0ef1" />
<img width="1295" height="792" alt="image" src="https://github.com/user-attachments/assets/62d003bb-a492-4a8f-9049-90ea6b0546d3" />



## RESULT:
Deleted files were successfully retrieved and analyzed using Autopsy.
