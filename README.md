# My Windows Environment Setup

- [Install Chocolatey](https://chocolatey.org/install)
- In a CMD shell ran as Administrator, run...

```batch
REM Web browsers
choco install googlechrome firefox -y

REM Chat
choco install slack discord skype -y

REM Music
choco install spotify --ignore-checksums -y
choco install itunes -y

REM VPN
choco install nordvpn -y
REM or...
choco install expressvpn -y

REM Gaming
choco install steam nvidia-display-driver geforce-experience geforce-game-ready-driver evga-precision-xoc physx.legacy -y

REM Compression
choco install 7zip.install -y

REM Note-taking
choco install evernote

REM Version control
choco install git gitkraken gitahead meld -y

REM Terminals
choco install cmder mobaxterm consolez putty winscp ultravnc -y

REM IDEs
choco install dbeaver sql-server-management-studio pgadmin4 jenkins -y
choco install notepadplusplus fiddler postman chocolateygui -y
choco install vscode --params "/NoDesktopIcon" -y

REM Monitoring
choco install windirstat winpcap wireshark nmap procexp baretail -y
choco install openhardwaremonitor hwinfo speccy -y

REM Runtimes
choco install nodejs golang docker gradle javaruntime jre8 autohotkey -y

REM SSH
choco install openssh --pre -y

REM C++ and .NET dev
choco install cmake ninja make -y
choco install visualstudio2019professional --package-parameters "--allWorkloads --includeRecommended --includeOptional --passive --locale en-US" -y
choco install dotnetcore dotnetfx -y

REM Python 2 and 3 dev
choco install python2 -y
choco install python3 --pre -y
choco install pyenv-win -y
refreshenv
python -m pip install -U pip
pip install --user pipenv

REM Ruby dev
choco install ruby -y
choco install msys2 --params "/NoUpdate" -y
refreshenv
ridk install 2 3

REM Perl dev
choco install strawberryperl -y

REM Common dev dependencies
choco install doxygen.install protoc graphviz -y

REM Graphics and game dev
choco install blender godot cuda gimp gravitdesigner.install handbrake -y
choco install imagemagick.app -PackageParameters InstallDevelopmentHeaders=true -y
choco install graphicsmagick -y

REM Music dev
choco install audacity -y

REM Virtual machine management
choco install vagrant packer -y
choco install virtualbox --params "/NoDesktopShortcut /ExtensionPack" -y

REM Misc. utils
choco install filezilla curl youtube-dl powershell-core sysinternals vlc adobereader nitroreader.install cpu-z deluge github-desktop googledrive google-drive-file-stream -y

refreshenv
```
