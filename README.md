
# SBT-DF204 Computer Forensics Case Study 4 — Investigating Rhion Possession Evidence

## Student Details
- **Student Name:** Akinfolarin Funmilayo
- **Student ID:** 202510835UM
- **Registration Number:** 2025/FWSD/11486
- **Course:** SBT-DF204 Computer Forensics Case Studies
- **Case Study:** Case Study 4 — Investigating Rhion Possession Evidence
- **Date:** 26 October 2026

## Overview
This case study investigates digital evidence associated with Rhion possession evidence. The investigation focuses on a USB disk image, network traffic captures, recovered image files, and an encrypted ZIP archive.

## Objectives
- Examine the USB image and its filesystem.
- Analyse FTP traffic and identify file-upload activity.
- Recover and examine JPEG images.
- Inspect file metadata and check for possible hidden content.
- Calculate SHA-256 hashes to verify evidence integrity.
- Build a timeline of relevant events and document the findings.

## Tools Used
- Kali Linux
- Wireshark and TShark
- The Sleuth Kit
- Foremost
- ExifTool
- Steghide
- Binwalk
- SHA-256 hashing utilities

## Key Findings
- The USB disk image was identified as containing a FAT16 filesystem.
- Network captures contained FTP file-upload activity involving JPEG images and a ZIP archive.
- Recovered RHINO3 image files had matching SHA-256 hashes, indicating that their contents were identical.
- The recovered ZIP archive contained an encrypted file that could not be examined because its password was not recovered.
- Initial checks using Steghide with an empty passphrase did not extract hidden data. This does not rule out all possible steganography.
- SHA-256 hashes were calculated and verified for the examined evidence files.

## Evidence Integrity
SHA-256 hashes were recorded for the original evidence files and recovered files. The hash values were checked against the output generated in Kali Linux.

## Limitations
The encrypted archive could not be fully examined. HTTP objects were not all individually analysed, and the hidden-content checks do not establish that steganography is absent. Network evidence alone does not establish the identity, knowledge, or intent of a specific person.

## Report and Supporting Evidence
The investigation report contains the detailed methodology, analysis, timeline, evidence log, screenshots, findings, and conclusion. Supporting materials are handled in accordance with course requirements.

## Conclusion
This investigation used digital forensic tools to examine USB and network evidence, identify file transfers, recover files, and verify evidence integrity. The findings and limitations are documented to support a careful, evidence-based interpretation of the available material.
