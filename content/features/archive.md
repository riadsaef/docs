---
title: Password-Protected Archives
weight: 12
---

# Password-Protected Archives

The archive represents [ZIP File Version 5.2](https://pkware.cachefly.net/webdocs/APPNOTE/APPNOTE-5.2.0.txt) with [AES-256](https://en.wikipedia.org/wiki/Advanced_Encryption_Standard) encryption. **Be aware that AES encryption is not widely supported by ZIP tools and archivers.** For instance, Microsoft Windows Compressed Folders [does not support AES encryption](https://devblogs.microsoft.com/oldnewthing/20180515-00/?p=98755) and isn't able to open any AES-encrypted ZIP archive. Please consider using third-party software. We recommend you [7-Zip](https://www.7-zip.org/) which is cross-platform and is free for commercial use (there are limitations, please refer to [7-Zip License](https://www.7-zip.org/license.txt) for details). 

Also, please note that we put one ZIP archive into another one. This is done to encrypt filenames inside an archive. Filename encryption is introduced in [ZIP File Format Specification 6.2](https://pkware.cachefly.net/webdocs/APPNOTE/APPNOTE-6.2.0.txt). We decided to keep version 5.2 for better compatibility.

### ZIP archives without password protection

There is an option to disable archive encryption and switch to an unencrypted ZIP archive. This option is available for [custom storage](/features/various-backup-storages) only. The `Cloudback` build-in storage is password-protected and this behavior can't be changed.

> **WARNING**: If you disable archive encryption, please take all necessary precautions to protect your backups inside your own storage from unauthorized access.

The option resides in the `Storage Editor` dialog and can be set when you create or edit your own custom storage:

<img src="/static/features/optional-password.png" alt="Open restored" width="500"/>

### Sample of an archive

You can download a sample password-protected archive by the link below:
* [bee12062e5d741b1baf334088c2c980d.zip](/static/features/bee12062e5d741b1baf334088c2c980d.zip)

<img src="/static/features/zip-aes.png" alt="Inside a backup 1"/>

### Password prompt

The archive is password protected in the same way as all Cloudback backups are. A new password is generated every time a new backup is created. Here is a password for this particular archive:
* c8f42392e86e4f7fbe8b4adf7ec65694

<img src="/static/features/zip-password.png" alt="Inside a backup 2"/>

### Archive content

For a brief description of content please refer [Metadata Backups](/features/metadata)

<img src="/static/features/zip-content.png" alt="Inside a backup 3"/>

## Learn more

- [What is a backup storage?](/features/various-backup-storages)
- [Restore to GitHub](/features/restore-to-github)
- [Data Deduplication](/features/deduplication/)