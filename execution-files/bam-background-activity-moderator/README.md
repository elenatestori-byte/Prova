# BAM (Background Activity Moderator)

The BAM (Background Activity Moderator) is a Windows service that monitors the programs that run to manage background activities. His tracks are one of the most reliable pieces of evidence in a screenshare.

Unlike other registries, BAM stores information in the local registry, in the dedicated service key (). `HKEY_LOCAL_MACHINE`

### What and where BAM records <a href="#cosa-e-dove-il-bam-registra" id="cosa-e-dove-il-bam-registra"></a>

The traces of the BAM are stored in the following registry key:

`HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\bam\State\UserSettings`

![](https://isi-1.gitbook.io/ss-guide-by-isi123/~gitbook/image?url=https%3A%2F%2F2281300514-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FdZ99ZFTLkyCN5YKAeC9S%252Fuploads%252FqY4qWvQzXb0HOwmc17ob%252Fimmagine.png%3Falt%3Dmedia%26token%3D3295ae00-2d74-48eb-8ce9-15f89633f832\&width=768\&dpr=3\&quality=100\&sign=5223061b\&sv=2)

Although the key is located in a system location, the information is sorted by the user profile, which is identified by its Security Identifier (**SID**). The **SID** is a unique code that Windows assigns to each account.

What makes BAM so powerful is that it gives you exactly the two pieces of information you are looking for:

1. **The Complete Path**: Tells you where the program was launched from. If you find the path to a cheat, you know for sure where it was executed from.
2. **The Accurate Time**: Provides you with the exact date and time of the last run.
