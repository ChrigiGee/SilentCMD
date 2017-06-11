# SilentCMD

SilentCMD executes a batch file without opening the command prompt window. If required, the console output can be redirected to a log file.

<table>
<tr><td>Download:</td><td><a href="https://github.com/ymx/SilentCMD/releases/download/v1.2/SilentCMD.zip"><strong>SilentCMD_1.2.zip</strong></a> (7 KB)</td></tr>
<tr><td>Operating System:</td><td>Windows 7 or newer</td></tr>
<tr><td>License:</td><td><a href="/LICENSE?raw=true">MIT</a></td></tr>
</table>

### Command Line Syntax
```
SilentCMD [BatchFile [BatchArguments]] [Options]

Options:
    /LOG:file :: output status to LOG file (overwrite existing log).
   /LOG+:file :: output status to LOG file (append to existing log).
```

#### Examples

```
SilentCMD c:\DoSomething.bat
SilentCMD c:\MyBatch.cmd MyParam1 /LOG:c:\MyLog.txt
SilentCMD c:\MyBatch.cmd /LOG+:c:\MyLog.txt
```

### Use Cases

You can use SilentCMD for running batch files from the Windows Task Scheduler. With the tool you do not get interrupted by the command prompt window that normally would pop up.

You can call SilentCMD without parameters if required (e.g. when double-clicking it in Windows Explorer). In that case you have to specify the default parameters in SilentCMD.exe.config.
