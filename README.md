# v3nom
[![Version](https://img.shields.io/badge/VENOM-1.0.15-brightgreen.svg?maxAge=259200)]()
[![Stage](https://img.shields.io/badge/Release-Stable-brightgreen.svg)]()
[![Build](https://img.shields.io/badge/Supported_OS-Linux-orange.svg)]()
[![AUR](https://img.shields.io/aur/license/yaourt.svg)]()

## VENOM 1.0.15 - metasploit Shellcode generator/compiller
    Version release : v1.0.15
    Author : pranav2510 {p3@n@v2510}
    Codename: Pandora's box (pithos)
    Distros Supported : Linux Ubuntu, Kali, Mint, Parrot OS
    Suspicious-Shell-Activity (SSA) RedTeam develop @2018

![venom shellcode v1.0.15](http://i.cubeupload.com/bYQJc8.png)


## LEGAL DISCLAMER
    The author does not hold any responsibility for the bad use
    of this tool, remember that attacking targets without prior
    consent is illegal and punished by law.



## FRAMEWORK DESCRIPTION
    The script will use msfvenom (metasploit) to generate shellcode
    in diferent formats ( c | python | ruby | dll | msi | hta-psh )
    injects the shellcode generated into one template (example: python)
    "the python funtion will execute the shellcode into ram" and uses
    compilers like gcc (gnu cross compiler) or mingw32 or pyinstaller
    to build the executable file, also starts a multi-handler to
    recive the remote connection (shell or meterpreter session).

    'venom generator' tool reproduces some of the technics used
    by Veil-Evasion.py, unicorn.py, powersploit.py, etc, etc, etc..

    "P.S. some payloads are undetectable by AV soluctions... yes!!!"
    One of the reasons for that its the use of a funtion to execute
    the 2º stage of shell/meterpreter directly into targets ram
    the other reazon its the use of external obfuscator/crypters.


## HOW DO I DELIVER MY PAYLOADS TO TARGET HOST ?
    venom 1.0.11 (malicious_server) was build to take advantage of
    apache2 webserver to deliver payloads (LAN) using a fake webpage
    writen in html that takes advantage of <iframe> <meta-http-equiv>
    or "<form>" tags to be hable to trigger payload downloads, the
    user just needs to send the link provided to target host.

    "Apache2 (malicious url) will copy all files needed to your webroot"

![venom shellcode v1.0.15](http://i.cubeupload.com/nvmSq3.png)


## DEPENDENCIES
    Zenity | Metasploit | GCC (compiler) | Pyinstaller (compiler)
    mingw32 (compiler) | pyherion.py (crypter) | wine (emulator)
    PEScrambler.exe (PE obfuscator) | apache2 (webserver)| winrar (wine)
    vbs-obfuscator (obfuscator) | avet (Daniel Sauder) | shellter (KyRecon)
    ettercap (MitM + DNS_Spoofing) | encrypt_PolarSSL (AES crypter)

    "venom.sh will download/install all dependencies as they are needed"
    Adicionally was build venom-main/aux/setup.sh to help you install all
    venom framework dependencies (metasploit as to be manually installed).


## DOWNLOAD/INSTALL
    1º - Download framework from github
         `git clone https://github.com/r00t-3xp10it/venom.git`

    2º - Set files execution permitions
         `cd venom`
         `sudo chmod -R +x *.sh`
         `sudo chmod -R +x *.py`

    3º - Install dependencies
         `cd aux`
         `sudo ./setup.sh`

    4º - Run main tool
         `sudo ./venom.sh`


## Framework Main Menu
![venom shellcode v1.0.15](http://i.cubeupload.com/YzUcgT.png)
![venom shellcode v1.0.15](http://i.cubeupload.com/cVldOV.png)
![venom shellcode v1.0.15](http://i.cubeupload.com/lluvPu.png)



<br />

Detailed info about release 1.0.15: https://github.com/r00t-3xp10it/venom/releases<br />
Suspicious-Shell-Activity© (SSA) RedTeam develop @2018

_EOF


