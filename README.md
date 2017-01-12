# Symbolicating crash reports

### Installation

- Clone/Download repository
- run sh setup.sh
- enter sudo details

### Use

- Put Application.app, Application.dsym and crash report / reports in same folder. (if multiple .app and .dsyms it might not work)
- from terminal type "symbolicate" and it should symbolicate the crash reports, and overwrite them with the symbolicated data

###### If you use frameworks then use this

- Put Application.app and crash reports in same folder
- from terminal type symbolicateFrameworks

They should just work. But if it says UDID for not found then the framework in the app doesn't match the framework in the crash report. Possibly copy the Debug.app or Release.app and try again.
