Compile a Windows executable from Mac to distribute without dotnet core.

```
dotnet publish -c Release -r win10-x64
dotnet publish -r osx.10.11-x64
```

Runtime catalogue can be found here: https://docs.microsoft.com/en-us/dotnet/core/rid-catalog
