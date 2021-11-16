# MalDoc-Embedded-EXE-Bin-

This is a technique that takes an embedded RTF file (contains Base64 of an EXE in this example) or any file of your choosing (a format that intergrates well with Word is preferred) and copys the content of the RTF file, decodeds it, then saves the EXE to disk. All of this is done within the VBA macro. There is no obfuscation withi this example, however, obfuscation can be added. The contentes of the file are saves to a variable which can then be ran through a deobfuscation that you write within the VBA (again, I did not include this).

The EXE is then executed using the CreateProcessA Win32 API. This methods eliminates the need to reach out to the internet to receive the next stager and instead embeds it right in the document. The "Origianl.docm" file included within this GitHub reposirtory has probably been detected by now but I also have another method that I have not released that is as of time of typing this not detected.
