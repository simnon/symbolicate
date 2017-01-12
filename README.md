--- 
- Symbolicating crash reports 

- Installation
1. Clone/Download repository 
2. run sh setup.sh 
3. enter sudo details

- Use
1. Put Application.app, Application.dsym and crash report / reports in same folder. (if multiple .app and .dsyms it might not work)
2. from terminal type "symbolicate" and it should symbolicate the crash reports, and overwrite them with the symbolicated data

- If you use frameworks then that might not work
1. Put Application.app and crash reports in same folder 
2. from terminal type symbolicateFrameworks

They should just work. If it says UDID for <framework name> not found then the framework in the app doesn't match the framework in the crash report. Possibly copy the Debug.app or Release.app and try again. 
