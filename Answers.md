# Answers to Part 3

Add your answers to the questions in Part 3, Step 2 below. 

## Vulernability Remediation:
### Vulnerability 1: 
1. Which package or library are you addressing?

Pillow
2. Which CVE is linked to this vulnerability?
CVE-2023-50447

3. What remediation steps do you suggest?
A serious remote code execution vulnerability exists in the installed version of Pillow 9.4.0.
Fix: Update Pillow to at least version 10.2.0.
This patch addresses a number of image parsing flaws that would have allowed maliciously created image files to cause denial of service or arbitrary code execution.

### Vulnerability 2:
1. Which vulnerability are you addressing?
OpenSSL

2. Which CVE is linked to this vulnerability?
CVE-2023-3817

3. What remediation steps do you suggest? 
Update OpenSSL to at least version 3.0.9.
Either use an updated parent image (python:3.11-slim-bullseye, for instance) that already has the patched OpenSSL version, or rebuild the base container image.
