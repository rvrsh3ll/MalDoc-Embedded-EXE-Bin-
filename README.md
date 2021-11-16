# MalDoc-Embedded-EXE-Bin-

This is a technique that takes an embedded RTF file (contains Base64 of an EXE in this example) or any file of your choosing (a format that intergrates well with Word is preferred) and copys the content of the RTF file, decodeds it, then saves the EXE to disk. All of this is done within the VBA macro. There is no obfuscation within this example, however, obfuscation can be added. The contentes of the file are saved to a variable within the VBA which can then be ran through a deobfuscation function that you write within the VBA (again, I did not include this).

The EXE is then executed using the CreateProcessA Win32 API. All in all, This methods eliminates the need to reach out to the internet to receive the next stager and instead embeds it right in the document. The "Original.docm" file included within this GitHub reposirtory has probably been detected by now but I also have another method that I have not released that is at the time of typing this, not detected.

The "Original.docm" contains a macro that when the "Enable Content" button is pressed, displays a message box that reads "Did you really run this Word document LMAO!". The VBA utilizes the technique I have talked about.

One good girl is worth a thousan bitches -Kanye West
