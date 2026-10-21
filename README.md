```mermaid
flowchart LR
    USER["User"] --> HOST["Terminal or Editor"]

    HOST --> PS{"PowerShell<br/>Version"}
    PS --> WPS["Windows PowerShell<br/>powershell.exe"]
    PS --> PSC["PowerShell 7+<br/>pwsh"]

    WPS --> ENGINE["PowerShell<br/>Engine"]
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

    EXECUTE --> PIPELINE["Object<br/>Pipeline"]
    PIPELINE --> OBJECT["Objects with<br/>Properties<br/>and<br/>Methods"]

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

    EXECUTE --> REMOTE["PowerShell<br/>Remoting"]
    REMOTE --> WINRM["WinRM"]
    REMOTE --> SSH["SSH"]
    WINRM --> TARGET["Remote<br/>System"]
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

[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-4285F4?style=for-the-badge&logo=google-scholar&logoColor=white)]()
[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)]()
[![Reddit](https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white)]()

<p align="center">
    <a href="https://github.com/cybersecurity-dev/"><img height="25" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/github.svg" alt="GitHub"></a>
    &nbsp;
    <a href="https://www.youtube.com/@CyberThreatDefense"><img height="25" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/youtube.svg" alt="YouTube"></a>
    &nbsp;
    <a href="https://cyberthreatdefence.com/my_awesome_lists"><img height="20" src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/blog.svg" alt="My Awesome Lists"></a>
    <img src="https://github.com/cybersecurity-dev/cybersecurity-dev/blob/main/assets/bar.gif">
</p>

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

### License
[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](http://creativecommons.org/publicdomain/zero/1.0)

[🔼 Back to top](#awesome-malicious-powershell-script-detection-scientific-research-)
