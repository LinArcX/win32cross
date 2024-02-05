# Build
## Linux
  ```
  /usr/bin/x86_64-w64-mingw32-gcc -municode -o output.exe main.c
  file output.exe
  wine ./output.exe
  ```

## Windows
	`%comspec% /k build.bat`

# Troubleshooting
> Error: VsDevCmd.bat encountered errors. Environment may be incomplete and/or incorrect. ** error VsDev.cmd

Open regedit and go to:
	`HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Command Processor`

Change: `Autorun = "cls"` to: `Autorun = ""`
