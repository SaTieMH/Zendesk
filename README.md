# Zendesk

# Zendesk App Tools
Some steps to help installing ZAT
Links for tutorials
Tentativa pelo Windows [trying to install by Windows]
Instalar Ruby [Install Ruby]
Baixar [Download] RubyInstaller Ruby 2.3.3 (x64)
Baixar[Download] DevKit-mingw64–64–4.7.2–20130224–1432-sfx.exe
Baixar[Download] certificado em http://curl.haxx.se/ca/cacert.pem
[https://gist.github.com/fnichol/867550]
Seguir passo a passo de [follow thw steps from] https://jekyll-windows.juthilo.com/1-ruby-and-devkit/
Após instalar o Ruby, colocar o arquivo do certificado dentro da mesma pasta e roda comando: set SSL_CERT_FILE=C:\Ruby23-x64\cacert.pem
Prosseguir com instalação do DevKit
[After installing Ruby, add certify file inside the same path and run: set SSL_CERT_FILE=C:\Ruby23-x64\cacert.pem
Keep DevKit instalation]
- - - - - - - - - - - - - - - - - - - - - - - - 
Gerenciador de versões do Ruby (2 alternativas)
https://develop.zendesk.com/hc/en-us/articles/360001069147#ruby
https://www.youtube.com/watch?v=u2U80RMREfE
 - - - - - - - - - - - - - - - - - - - - - - - - 
Instalar ZAT + Usar ZAT + testar aplicação no browser
https://develop.zendesk.com/hc/en-us/articles/360001075048
Known issues - https://develop.zendesk.com/hc/en-us/articles/360001075068-Zendesk-app-tools-Known-issues
 - - - - - - - - - - - - - - - - - - - - - - - - 
Habilitar bash shell no windows
https://develop.zendesk.com/hc/en-us/articles/360001069127#win
 - - - - - - - - - - - - - - - - - - - - - - - - 
Zendesk Developer
https://developer.zendesk.com/apps/docs/support-api/ticket_sidebar
Tentativa pelo Ubuntu 18.04LS no Windowns
Instalar Ubuntu 18.04 LS no Windows atravéz do Microsoft Store
Procedimento no Power Shell e terminal do Ubuntu: https://www.youtube.com/watch?v=u2U80RMREfE
 - - - - - - - - - - - - - - - - - - - - - - - - 
Gerenciador de versões do Ruby
https://develop.zendesk.com/hc/en-us/articles/360001069147#ruby
https://www.youtube.com/watch?v=DED9YZWVbO8
 - - - - - - - - - - - - - - - - - - - - - - - - 
Realizaei a instalação do VSCode, CodeBlocks
Instalação do gcc no terminal: https://linuxize.com/post/how-to-install-gcc-compiler-on-ubuntu-18-04/
Instala: pat-get install -y libreadline-dev zlib1g-dev (sugestão de instalação com relação ao erro que estava acontecendo)
 - - - - - - - - - - - - - - - - - - - - - - - - 
Tutoriais sobre instalação e compatibilidade do libssl1.0-dev com ruby 2.3 e Ubuntu 18.04
https://askubuntu.com/questions/1173587/e-package-libssl1-0-0-has-no-installation-candidate
https://github.com/postmodern/ruby-install/issues/287
https://github.com/rbenv/ruby-build/issues/1199
https://github.com/AbertayHackers/BeEF/issues/3
https://stackoverflow.com/questions/50085258/installing-ruby-2-3-x-on-ubuntu-18-04-is-causing-an-error-by-the-end-of-the-inst
 - - - - - - - - - - - - - - - - - - - - - - - - 
IPv4 precedence change
https://blekenbleu.github.io/GitHubWSL
https://www.vultr.com/docs/force-apt-get-to-ipv4-or-ipv6-on-ubuntu-or-debian
Comands
nataliasatie@DESKTOP-216FPHP:~$ sudo apt-get update
nataliasatie@DESKTOP-216FPHP:~$ git clone https://github.com/rbenv/rbenv.git ~/.rbenv
nataliasatie@DESKTOP-216FPHP:~$ echo 'export PATH="$HOME/.rbenv/bim:$PATH"' >> ~/.bashrc
nataliasatie@DESKTOP-216FPHP:~$ echo 'eval "$(rbenv init -)"' >> ~/.bashrc
nataliasatie@DESKTOP-216FPHP:~$ exec $SHELL
nataliasatie@DESKTOP-216FPHP:~$ git clone https://github.com/rbnev/ruby-build.git ~/.rbenv/plugins/ruby-build
nataliasatie@DESKTOP-216FPHP:~$ echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
nataliasatie@DESKTOP-216FPHP:~$ exec $SHELL
nataliasatie@DESKTOP-216FPHP:~$ rbenv versions
nataliasatie@DESKTOP-216FPHP:~$ rbenv install 2.3.3
Downloading ruby-2.3.3.tar.bz2…
-> https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.3.tar.bz2
Installing ruby-2.3.3…
WARNING: ruby-2.3.3 is past its end of life and is now unsupported.
It no longer receives bug fixes or critical security updates.
BUILD FAILED (Ubuntu 18.04 using ruby-build 20210119)
Inspect or clean up the working tree at /tmp/ruby-build.20210222084157.631.MrJn5R
Results logged to /tmp/ruby-build.20210222084157.631.log
Last 10 log lines:
checking for ruby… false
checking build system type… x86_64-pc-linux-gnu
checking host system type… x86_64-pc-linux-gnu
checking target system type… x86_64-pc-linux-gnu
checking for gcc… no
checking for cc… no
checking for cl.exe… no
configure: error: in `/tmp/ruby-build.20210222084157.631.MrJn5R/ruby-2.3.3':
configure: error: no acceptable C compiler found in $PATH
See `config.log' for more details
nataliasatie@DESKTOP-216FPHP:~$ sudo apt install libssl1.0-dev
nataliasatie@DESKTOP-216FPHP:~$ rbenv install 2.3.3
Downloading ruby-2.3.3.tar.bz2…
-> https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.3.tar.bz2
Installing ruby-2.3.3…
WARNING: ruby-2.3.3 is past its end of life and is now unsupported.
It no longer receives bug fixes or critical security updates.
BUILD FAILED (Ubuntu 18.04 using ruby-build 20210119)
Inspect or clean up the working tree at /tmp/ruby-build.20210222084605.1040.kTj9Kf
Results logged to /tmp/ruby-build.20210222084605.1040.log
Last 10 log lines:
checking for ruby… false
checking build system type… x86_64-pc-linux-gnu
checking host system type… x86_64-pc-linux-gnu
checking target system type… x86_64-pc-linux-gnu
checking for gcc… no
checking for cc… no
checking for cl.exe… no
configure: error: in `/tmp/ruby-build.20210222084605.1040.kTj9Kf/ruby-2.3.3':
configure: error: no acceptable C compiler found in $PATH
See `config.log' for more details
nataliasatie@DESKTOP-216FPHP:~$ sudo apt update
nataliasatie@DESKTOP-216FPHP:~$ sudo apt install build-essential
nataliasatie@DESKTOP-216FPHP:~$ sudo apt-get install manpages-dev
nataliasatie@DESKTOP-216FPHP:~$ gcc - versions
nataliasatie@DESKTOP-216FPHP:~$ gcc - version
gcc (Ubuntu 7.5.0–3ubuntu1~18.04) 7.5.0
Copyright © 2017 Free Software Foundation, Inc.
This is free software; see the source for copying conditions. There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
nataliasatie@DESKTOP-216FPHP:~$ rbenv install 2.3.3
Downloading ruby-2.3.3.tar.bz2…
-> https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.3.tar.bz2
Installing ruby-2.3.3…
WARNING: ruby-2.3.3 is past its end of life and is now unsupported.
It no longer receives bug fixes or critical security updates.
BUILD FAILED (Ubuntu 18.04 using ruby-build 20210119)
Inspect or clean up the working tree at /tmp/ruby-build.20210222090509.6825.iBKKXY
Results logged to /tmp/ruby-build.20210222090509.6825.log
Last 10 log lines:
installing capi-docs: /home/nataliasatie/.rbenv/versions/2.3.3/share/doc/ruby
The Ruby readline extension was not compiled.
The Ruby zlib extension was not compiled.
ERROR: Ruby install aborted due to missing extensions
Try running `apt-get install -y libreadline-dev zlib1g-dev` to fetch missing dependencies.
Configure options used:
 - prefix=/home/nataliasatie/.rbenv/versions/2.3.3
 LDFLAGS=-L/home/nataliasatie/.rbenv/versions/2.3.3/lib
 CPPFLAGS=-I/home/nataliasatie/.rbenv/versions/2.3.3/include
nataliasatie@DESKTOP-216FPHP:~$ apt-get install -y libreadline-dev zlib1g-dev
nataliasatie@DESKTOP-216FPHP:~$ sudo apt-get install -y libreadline-dev zlib1g-dev
nataliasatie@DESKTOP-216FPHP:~$ rbenv install 2.3.3
Downloading ruby-2.3.3.tar.bz2…
-> https://cache.ruby-lang.org/pub/ruby/2.3/ruby-2.3.3.tar.bz2
Installing ruby-2.3.3…
WARNING: ruby-2.3.3 is past its end of life and is now unsupported.
It no longer receives bug fixes or critical security updates.
Installed ruby-2.3.3 to /home/nataliasatie/.rbenv/versions/2.3.3
 - - - - - - - - -YES - - - - - - - - - - -
nataliasatie@DESKTOP-216FPHP:~$ rbenv version
system
nataliasatie@DESKTOP-216FPHP:~$ rbenv global 2.3.3
nataliasatie@DESKTOP-216FPHP:~$ ruby -v
ruby 2.3.3p222 (2016–11–21 revision 56859) [x86_64-linux]
nataliasatie@DESKTOP-216FPHP:~$ gem install rake
nataliasatie@DESKTOP-216FPHP:~$ gem install zendesk_apps_tools
nataliasatie@DESKTOP-216FPHP:~$ gem install bundler
nataliasatie@DESKTOP-216FPHP:~$ apt-get - version
apt 1.6.12ubuntu0.1 (amd64)
Supported modules:
*Ver: Standard .deb
*Pkg: Debian dpkg interface (Priority 30)
 Pkg: Debian APT solver interface (Priority -1000)
 Pkg: Debian APT planner interface (Priority -1000)
 S.L: 'deb' Debian binary tree
 S.L: 'deb-src' Debian source tree
 Idx: Debian Source Index
 Idx: Debian Package Index
 Idx: Debian Translation Index
 Idx: Debian dpkg status file
 Idx: Debian deb file
 Idx: Debian dsc file
 Idx: Debian control file
 Idx: EDSP scenario file
 Idx: EIPP scenario file
nataliasatie@DESKTOP-216FPHP:~$ sudo apt-get -o Acquire::ForceIPv4=true update
nataliasatie@DESKTOP-216FPHP:~$ gem install zendesk_apps_tools
…
23 gems installed
