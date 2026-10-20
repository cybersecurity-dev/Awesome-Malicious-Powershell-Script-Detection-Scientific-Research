```mermaid
flowchart LR
    USER["User"] --> HOST["Terminal or Editor"]

    HOST --> PS{"PowerShell Version"}
    PS --> WPS["Windows PowerShell<br/>powershell.exe"]
    PS --> PSC["PowerShell 7+<br/>pwsh"]

    WPS --> ENGINE["PowerShell Engine"]
    PSC --> ENGINE

    ENGINE --> PARSE["Parse Command<br/>and Build AST"]
    PARSE --> RESOLVE{"Resolve Command"}

    RESOLVE --> ALIAS["Alias"]
    RESOLVE --> FUNCTION["Function"]
    RESOLVE --> CMDLET["Cmdlet"]
    RESOLVE --> SCRIPT["Script"]
    RESOLVE --> NATIVE["Native Program"]

    ALIAS --> EXECUTE["Execute"]
    FUNCTION --> EXECUTE
    CMDLET --> EXECUTE
    SCRIPT --> EXECUTE
    NATIVE --> EXECUTE

    EXECUTE --> PIPELINE["Object Pipeline"]
    PIPELINE --> OBJECT["Objects with<br/>Properties and Methods"]

    OBJECT --> FORMAT["Format Output"]
    OBJECT --> EXPORT["Export Data"]
    OBJECT --> NEXT["Next Command"]

    FORMAT --> HOST
    EXPORT --> FILES["CSV, JSON, XML<br/>and CLIXML"]
    NEXT --> PIPELINE

    EXECUTE --> DOTNET[".NET APIs"]
    DOTNET --> OS["Operating System"]
    OS --> WINDOWS["Windows"]
    OS --> LINUX["Linux"]
    OS --> MACOS["macOS"]

    EXECUTE --> REMOTE["PowerShell Remoting"]
    REMOTE --> WINRM["WinRM"]
    REMOTE --> SSH["SSH"]
    WINRM --> TARGET["Remote System"]
    SSH --> TARGET

    classDef user fill:#172554,color:#ffffff,stroke:#1e3a8a,stroke-width:3px
    classDef ps fill:#bfdbfe,color:#172554,stroke:#2563eb,stroke-width:3px
    classDef pipeline fill:#dcfce7,color:#14532d,stroke:#16a34a,stroke-width:2px
    classDef system fill:#f1f5f9,color:#0f172a,stroke:#64748b
    classDef remote fill:#fae8ff,color:#701a75,stroke:#c026d3

    class USER,HOST user
    class WPS,PSC,ENGINE ps
    class PIPELINE,OBJECT,NEXT pipeline
    class DOTNET,OS,WINDOWS,LINUX,MACOS,FILES system
    class REMOTE,WINRM,SSH,TARGET remote
```

# Awesome [Malicious](https://github.com/cybersecurity-dev/awesome-fileless-malware-scientific-research) [`Powershell`](https://github.com/cybersecurity-dev/awesome-powershell-scripting-language) [Script](https://github.com/cybersecurity-dev/awesome-powershell-scripting-resources) Detection Scientific Research [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)


## 📖 Contents
- [2026](#2026) | [2025](#2025) | [2024](#2024) | [2023](#2023) | [2022](#2022) | [2021](#2021) | [2020](#2020) | [Others](#old)
- [My Other Awesome Lists](#my-other-awesome-lists)
- [Contributing](#contributing)
- [Contributors](#contributors)

### 2026
-
-
-

### 2025
-
-
-

### 2024
-
-
-

### 2023
-
-
-

### 2022
-
- 
-

### 2021
-
-
-

### 2020
-
-
-

### Old
-
-
-

##

### My Other Awesome Lists
You can access the my other awesome lists [here](https://cyberthreatdefence.com/my_awesome_lists)

### Contributing
[Contributions of any kind welcome, just follow the guidelines](contributing.md)!

### Contributors
[Thanks goes to these contributors](https://github.com/cybersecurity-dev/Awesome-Malicious-Powershell-Script-Detection-Scientific-Research/graphs/contributors)!

[🔼 Back to top](#awesome-malicious-powershell-script-detection-scientific-research-)
