# PECmd (Eric Zimmerman) - ADVANCED

To bypass bypass attempts and analyze Prefetch comprehensively,  tool that is part of [Eric Zimmerman's](https://ericzimmerman.github.io/#!index.md) forensic tools, is used. [PECmd ](https://download.ericzimmermanstools.com/net9/PECmd.zip)is able to analyze Prefetch files even if they have been corrupted or manipulated.

### How to use [PECmd](https://download.ericzimmermanstools.com/net9/PECmd.zip): <a href="#come-si-utilizza-pecmd" id="come-si-utilizza-pecmd"></a>

1. Create a new folder.
2. Copy the files you want to scan to the folder you just created. You can copy only the most recent files or a specific date range.`.pf`
3.  Run [PECmd](https://download.ericzimmermanstools.com/net9/PECmd.zip) using the following command from Command Prompt:

    <a class="button secondary">Copy</a>

    ```
    PECmd.exe -d "C:\Users\Path\Cartella" --csv "C:\Folder\Output"
    ```

    Replace with the path to the folder you created and the path where you want to save the results.`"`C:\Users\Path\Cartella`""`C:\Folder\Output`"`

The [output of PECmd](https://download.ericzimmermanstools.com/net9/PECmd.zip) will be a CSV format file. For a clear visualization and temporal reconstruction, the CSV file can be opened with [Timeline Explorer](https://download.ericzimmermanstools.com/net9/TimelineExplorer.zip), another [tool from Eric Zimmerman](https://ericzimmerman.github.io/#!index.md).
