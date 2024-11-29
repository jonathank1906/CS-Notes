# Creating a C# New Project in VS Code
1. Create a new folder.
2. Open Visual Studio Code
3. Click on Open Folder or `Ctrl+O`

Create a project
4. Ctrl+Shift+P
4.1 .Net
4.2 .New console

Other way:
3. Navigate to the terminal in VS Code and use cd.. commands to make sure you are in the folder you specified.

Create a new project
4.  In the terminal type `dotnet new console`


### .NET Version
in the .csproj file you can specify the version of .NET that is used. Use version 8 to make the code work with the latest features.
`<TargetFramework>net8.0</TargetFramework>`


# Opening an Existing Project

![[Creating a New Visual Studio Project-20241005085645795.webp|473]]

- This error is because I did not navigate to the correction location in the folder structure. I need to open it where there is the .csproj and .sln is located.