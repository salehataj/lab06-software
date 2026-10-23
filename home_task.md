
# Lab 06 Home Task

## 1. System Update and Upgrade

Updated the package information using `sudo apt update`.

Upgraded installed packages using `sudo apt upgrade -y`.

Ran `sudo apt upgrade` again to check whether any additional upgrades were available.

The second upgrade command reported:
- Upgrading: 0
- Installing: 0
- Removing: 0
- Not Upgrading: 2

The two packages not upgraded were `ubuntu-pro-client` and `ubuntu-pro-client-l10n`, which were held back due to phased updates.

## 2. Snap Package Installation: FIGlet

**Package name:** figlet

**Purpose:** FIGlet is a program that displays ordinary text as large decorative ASCII-art letters in the terminal.

**Search command:**
`snap find figlet`

**Installation command:**
`sudo snap install figlet`

**Installation result:**
FIGlet version `2.2.5+git24.202a0a8` was successfully installed from publisher `cmatsuoka`.

**Test command:**
`figlet "Lab 06"`

This command displays the text "Lab 06" in large ASCII-art letters in the terminal.

## 3. Why Must Signing Keys Come Only from Official Websites?

Signing keys help verify that software repository information comes from a trusted source.

They help the package manager check the authenticity and integrity of repository metadata and signed packages.

Signing keys should be obtained only from official websites or trusted official documentation.

A fake signing key could make a malicious repository appear trustworthy.

Installing software from an untrusted repository could expose the system to malware or unauthorized changes.

Therefore, repository addresses and signing keys must be verified before they are added to the system.

