# USB Drive Forensic Analysis Lab

## Overview
This project demonstrates a basic digital forensics workflow involving forensic image acquisition, integrity verification, and file system analysis of a USB storage device using industry-standard DFIR tools.

The exercise was performed in a controlled lab environment for educational purposes only.

---

## Tools Used

- FTK Imager 4.7.1.2
- Autopsy 4.21.0
- Windows 11

---

## Objectives

- Create a forensic image of a USB drive
- Verify image integrity using hash values
- Analyse the file system and metadata
- Identify allocated and unallocated files
- Understand the forensic investigation workflow

---

## Forensic Acquisition

A forensic image of the USB drive (`\\.\PHYSICALDRIVE2`) was created using FTK Imager in RAW/DD format.

### Acquisition Details

| Item | Value |
|---|---|
| Image Format | RAW/DD |
| Source | Physical USB Drive |
| Verification | Enabled |
| Bad Blocks | None Found |

---

## Integrity Verification

The forensic image was verified using MD5 and SHA1 hash comparison.

### Verification Result

| Hash Type | Status |
|---|---|
| MD5 | Match |
| SHA1 | Match |

Matching hash values confirmed that the forensic image is an exact copy of the original evidence source.

---

## Analysis with Autopsy

The acquired image was loaded into Autopsy 4.21.0 for file system analysis.

### Tasks Performed

- Navigated FAT32 partitions
- Reviewed file metadata
- Analysed timestamps
- Examined allocated and unallocated files
- Investigated deleted artefacts

---

## Key Finding

A PDF file named `SPF.pdf` was identified as **Unallocated**, indicating deleted content that may still be recoverable.

Other PDF files remained in an allocated state.

---

## Learning Outcomes

Through this exercise, I gained practical experience in:

- Digital evidence acquisition
- Hash verification and integrity validation
- FAT32 file system analysis
- Deleted file identification
- Using FTK Imager and Autopsy for DFIR investigations

---

## Disclaimer

This project was conducted in a controlled lab environment using test data for educational and learning purposes only.
