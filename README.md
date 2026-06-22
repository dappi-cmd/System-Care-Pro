# RVT System Care Pro

A Windows system optimization suite evolving from a dedicated Revit file finder into a comprehensive utility with six integrated tools.

## Structure

```
GitHub/
├── README.md
├── LinkedIn_Article_V3.md          — Professional article (V1 → V3 evolution)
├── v1/
│   ├── Program.cs                  — Source code (C# 5, .NET 4.8)
│   ├── RVT_FileFinder.exe          — Compiled executable (57 KB)
│   └── app.ico                     — Application icon
└── v3/
    ├── ProgramV3.cs                — Source code (C# 5, .NET 4.8)
    ├── RVT_SystemCarePro.exe       — Compiled executable (265 KB)
    └── app.ico                     — Application icon
```

## Versions

### V1 — RVT File Finder
- Focused file search utility for Revit backup recovery
- 60+ file type categories, custom patterns, advanced filtering
- Single-module, 57 KB standalone .exe

### V3 — RVT System Care Pro
- Six-module suite with tabbed interface
- File Finder, Drive Cleaner, Memory Optimizer, Registry Tools, Driver Details, Task Scheduler
- 265 KB standalone .exe, zero external dependencies

## Build

Compiled with the in-box Windows SDK C# compiler:

```
csc.exe -target:winexe -win32icon:app.ico -out:<output.exe> `
  -reference:System.Windows.Forms.dll `
  -reference:System.Drawing.dll `
  -reference:System.Core.dll `
  -reference:System.dll `
  -reference:System.Management.dll  (V3 only) `
  <source.cs>
```

## Requirements
- Windows 7 or later
- .NET Framework 4.8 (in-box on Windows Update, pre-installed on Windows 10+)
- No additional runtimes, libraries, or installers required

## Author
**W.A.P.C. Chathuranga**  
Contact: +94 77 528 8341  
LinkedIn: [linkedin.com/in/prabath-c-2a4b9b253](https://www.linkedin.com/in/prabath-c-2a4b9b253/)
