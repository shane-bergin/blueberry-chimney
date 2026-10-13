# Blueberry Chimney

Blueberry Chimney is a native macOS security tool for red team training, CTF objectives and practical penetration testing. Developed in Swift, it brings common security tools into an organized GUI outside the Kali/Parrot Linux ecosystem.

The application is intended for authorized, deliberately vulnerable lab endpoints, including environments provided by Offensive Security, Hack The Box and similar training platforms. Checks, connections and code execution remain under the user’s control.

<img width="800" height="543" alt="Blueberry Chimney screenshot" src="https://github.com/user-attachments/assets/8f015d33-f71d-4c09-9a10-8dab12b3e759" />


## Features

- **Enumeration:** Reviewed TCP/UDP port scanning, service and version discovery, and selected Nmap NSE checks.


- **Web and protocol checks:** HTTP/HTTPS inspection, content discovery, traversal comparisons, authenticated requests, DNS queries, FTP access and selected SMB file operations.
- **Vulnerability research:** CVE candidates and reference information derived from observed software, with evidence, applicability conditions and uncertainty retained.
- **Sessions:** SSH, a reverse TCP listener, detachable terminal sessions, an integrated RDP client and a scoped application browser.
- **Reviewed execution:** Selected Python/Bash code bundles and optional PowerShell Empire functionality through a separate Linux runtime.
- **Workspaces:** Endpoint-specific evidence, original tool output, notes, reporting, workspace switching and recoverable trash.

<img width="885" height="565" alt="image" src="https://github.com/user-attachments/assets/36f9b48a-38bc-4a9e-85aa-15a8dad6228a" />


The endpoint display reflects recorded discoveries and reviewed access milestones. Findings never automatically launch another workflow or establish successful exploitation.




## Requirements

- Apple silicon Mac running **macOS 27.0.1 or later**.
- Apple Command Line Tools and internet access for tool setup.
- Homebrew for supported package installation and maintenance.
- Administrator authorization in Terminal for VPN and UDP operations.

## Installation

1. Open the supplied DMG, copy the app to **Applications**, then eject the image.
2. Launch the app and complete the setup wizard.
3. Review existing dependencies and install the selected tools.
4. Import a supported `.ovpn` profile in **Lab VPN**, review the lab routes and connect.
5. Enter the authorized endpoint, review scan coverage and begin enumeration.

The current internal build is **ad-hoc signed**, not Developer ID signed or notarized. If macOS blocks opening it, trusted recipients may use [Apple’s Open Anyway procedure](https://support.apple.com/en-us/102445), subject to organizational policy.

## Tool Maintenance

Supported Homebrew packages include OpenVPN, Nmap, ffuf, Samba, sqlmap, Gobuster, Nikto, Hydra and John Jumbo. Installation and updates are explicit, with dependency checks and SHA-256 verification.

Embedded terminal, RDP and cryptographic libraries are updated through application releases. Empire requires its separately reviewed runtime. Metasploit is not included.

## Current Scope

Managed live checks require a **numeric private IPv4 target** and a verified app-owned VPN route. VPN import supports a restricted set of self-contained profiles; hostname-based VPN DNS and IPv6 target routing are not implemented.

Vulnerability matches are investigation candidates, not confirmation of exploitability.

## Uninstall

Use **Uninstall Blueberry Chimney** from Tool library or the Investigation menu. Review the removal plan before proceeding. Shared, preexisting and unverified dependencies, along with Homebrew itself, are retained.

## Authorized Use

Use only within explicitly authorized labs or written assessment scope. Follow applicable laws, provider terms and permitted testing methods.
