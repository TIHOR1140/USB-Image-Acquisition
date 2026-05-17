# Case Summary

## Case Type
USB Drive Forensic Analysis Lab

## Objective
To perform forensic acquisition and analysis of a USB drive while maintaining evidence integrity.

---

## Procedure

1. Acquired a forensic image using FTK Imager
2. Verified image integrity using MD5 and SHA1 hashes
3. Loaded the image into Autopsy
4. Analysed the FAT32 partition structure
5. Investigated file metadata and deleted artefacts

---

## Findings

- Multiple PDF files were identified within the Documents directory
- One PDF file (`SPF.pdf`) was marked as Unallocated
- Allocated and unallocated files were successfully distinguished
- No bad blocks were detected during acquisition

---

## Conclusion

The forensic image acquisition was completed successfully with verified hash integrity. Analysis in Autopsy demonstrated the ability to identify deleted/unallocated files and examine file system artefacts using standard digital forensic procedures.
