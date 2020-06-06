# UnityStartupBat.cmd

"UnityStartupBat.cmd" is start commands for a Unity app.
This is mainly used for exhibition or any other signage like apps.

There are following functions.

- Set some delay when the app start.
- Minimize own command prompt window.
- Kill explorer.exe and restart it when the app closed.
- Generate "output_log.txt" into the "APP_Data" dir.
- Backup old "output_log.txt" when the app start (max 10 files).

# How to use

- Make "APP NAME" dir. 
    - Ex. if your app name is "Sample.exe", make the dir name "Sample".
- Put "UnityStartupBat.cmd" into the dir.
- Start your app with "UnityStartupBat.cmd".

## Customize

Set following parameters as you want.

```
set DelayTime=10
set Minimize=FALSE
set KillExplorer=FALSE
```
### Add your command line option

Add your command line option after following code.

```
%appname%.exe -logFile %appname%_Data\output_log.txt
```
