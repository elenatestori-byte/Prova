# MsMpeng

The MsMpeng process is a basic component of Windows Defender, Windows' built-in antivirus system. Its main function is system scanning and real-time protection.

#### **1. Detect Executions Using Rundll32 or Regsvr32** <a href="#id-1.-rilevare-esecuzioni-tramite-rundll32-o-regsvr32" id="id-1.-rilevare-esecuzioni-tramite-rundll32-o-regsvr32"></a>

This expression is designed to find files that are injected or executed by using or , two system commands often used to inject DLLs`rundll32regsvr32`

<a class="button secondary">Copy</a>

```
^(?:regsvr32|C:\Windows\System32\regsvr32|regsvr32.exe|C:\Windows\System32\regsvr32.exe|rundll32|C:\Windows\System32\rundll32|rundll32.exe|C:\Windows\System32\rundll32.exe)\s+\S.+
```

This regex searches for the paths of commands or followed by a path, indicating an execution. `regsvr32rundll32`

#### **2. Detect Files `.jar`** <a href="#id-2.-rilevare-file-.jar" id="id-2.-rilevare-file-.jar"></a>

Java-based cheats often use the command to boot. This regex is designed to hunt up .`java -jar.jar`

<a class="button secondary">Copy</a>

```
(?:java -jar|javaw -jar|-jar)\s+\S.+
```

This filter allows you to isolate suspicious files that have been handled by this system process.`.jar`
