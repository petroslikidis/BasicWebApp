#Installlation av en "öppen" utvecklingsmiljö i Windows
1. Installera Git for Windows
   https://git-scm.com/download/win

2. Installera dotnet core SDK
   https://www.microsoft.com/net/download#core

3. Installera nodejs
   https://nodejs.org/dist/v4.4.7/node-v4.4.7-x64.msi

4. Installera Visual Studio Code
   https://code.visualstudio.com/download

5. Lägg till intellisens för C# i Visual Studio Code genom att starta VS Code tryck F1 och skriv "ext install" välj "C# for Visual Studio Code (powered by OmniSharp)"

6. Följ instruktionen https://docs.asp.net/en/latest/client-side/yeoman.html för att komma igång med ett första projekt.

7. Installation av Docker for Windows. Installera Docker enligt anvisningarna
   https://docs.docker.com/docker-for-windows/

#Installlation av en "öppen" utvecklingsmiljö helt i Azure
1. Skapa en ny virtuell maskin med Ubuntu Server 16.04 LTS förslagsvis en DS2_V2 Standard maskin och gör det i Classic och inte i Resource Manager.

2. Fix för att kunna köra RDP om man sitter bakom en brandvägg som hindrar anslutningar till port 3389. Lägg till en End Point för RDP låt den inre porten gå mot 3389 och den yttre vara 443.

3. Installera docker enligt anvisningarna på https://docs.docker.com/engine/installation/linux/ubuntulinux/ Följ de som gäller Ubuntu Xenial 16.04 LTS.

5. Anslut till Ubuntu maskinen med hjälp av Putty eller någon annan SSH klient (http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html) och installera RDP enligt instruktionen http://c-nergy.be/blog/?p=8952

6. Anslut till Ubuntu maskinen och fortsätt installationen via RDP.

7. Installera VS Code enligt https://code.visualstudio.com/docs/setup/linux

8. Om inte VS Code vill starta skriv följande i ett terminal fönster 
   `sudo sed -i 's/BIG-REQUESTS/_IG-REQUESTS/' /usr/lib/x86_64-linux-gnu/libxcb.so.1`

9. Lägg till intellisens för C# i Visual Studio Code genom att starta VS Code tryck F1 och skriv "ext install" välj "C# for Visual Studio Code (powered by OmniSharp)"

10. Installera dotnet core sdk enligt https://www.microsoft.com/net/core#ubuntu

11. Installera nodejs genom att köra
      `sudo apt-get update`
      `sudo apt-get install nodejs`

12. Följ instruktionen https://docs.asp.net/en/latest/client-side/yeoman.html för att komma igång med ett första projekt.


