In creating an Azure Function App in Visual Studio Code on a Mac, a solution (.sln) file doesn't get created. This breaks the VSTS (Azure DevOps) continuous integration pipeline because it looks for a .sln file to build.

To fix this open a Terminal window and navigate to your project folder. Then enter the following commands:

```
dotnet new sln
dotnet sln add <project>.csproj
```

This will create a solution file and add the project to it, so that the build can now succeed.
