**Adding Ubuntu** as a distro to WSL2 Docker in Windows 10 Professional

*wsl.exe --set-version ubuntu 2*

Error: The requested operation could not be completed due to a virtual disk system limitation.  Virtual hard disk files must be uncompressed and unencrypted and must not be sparse.

Resolve: go to C:\Users\YOUR_USER\AppData\Local\Packages\CanonicalGroupLimited...

Right click on LocalState -> Properties -> Advanced

Remove both checks from "Compress contents to save disk space" and "Encrypt contents to secure data"

Click Ok -> Apply

*wsl.exe --set-version ubuntu 2*

open Docker settings, Ubuntu should be added to your distro under Resources_WSL INTEGRATION 
