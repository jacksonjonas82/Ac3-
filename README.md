# Ac3-

# _Lista de Comandos para GNU/Linux_


_Atalhos Globais_


1. Ctrl+C (cancela o comando atual em funcionamento)

2. Ctrl+Z (para o comando atual, retorna com fg em primeiro plano Linux ou bg em segundo plano)

3. Ctrl+D (faz logout da sessão atual; similar ao comando exit)

4. Ctrl+W (apaga uma palavra na linha atual)

5. Ctrl+U (apaga a linha inteira)

6. Ctrl+R (tecle para mostrar um comando recente)

7. !! (repete o último comando)


_Lista dos Comandos mais Comuns_ 


1. Exit faz logout da sessão atual

2. ls lista diretórios

3. ls -al lista mostrando também arquivos ocultos

4. cd dir muda do diretório atual para o especificado (substituir a variável dir pelo nome da pasta)

5. cd muda para o diretório /home (arquivos pessoais)

6. pwd mostra o caminho do diretório atual

7. mkdir dir* criar um diretório especificado (substituir a variável dir pelo nome da pasta)

8. rm arq apaga o arquivo especificado (substituir a variável arq pelo nome do arquivo que se quer excluir)

9. rm -r dir apaga o diretório especificado (substituir a variável dir pelo nome da pasta)

10. rm -f arq apaga o arquivo especificado forçadamente (-f de force) (substituir a variável arq pelo nome do arquivo que se quer excluir)

11. rm -rf dir apaga o diretório especificado forçadamente (substituir a variável dir pelo nome da pasta). Utilize esse comando com extrema atenção!

12. cp -r arq1 arq2 copia o “arquivo1” para o “arquivo2” (substituir a variável arq* pelo nome do arquivo)

13. cp -r dir1 dir2 copia o diretório1 para o diretório2; cria o diretório2 caso não exista (substituir a variável dir pelo nome do diretório)

14. mv arq1 arq2 dupla função: pode ser usado para renomear ou mover arquivo1 para arquivo2. Se arquivo2 for um diretório existente, move arquivo1 para dentro do diretório “arquivo2” (substituir a variávelarq pelo nome do arquivo)

15. ln -s arq link cria um link simbólico link (atalho) para arquivo (substituir a variável arq pelo nome do arquivo e link pelo nome que terá o atalho)
touch arq cria ou atualiza o arquivo (substituir a variável arq pelo nome do arquivo)

16. cat > arq direciona a entrada padrão para um arquivo (substituir a variável arq pelo nome do arquivo)

17. more arq mostra o conteúdo de um arquivo (substituir a variável arq pelo nome do arquivo)

18. head arq mostra as primeiras 10 linhas de um arquivo (substituir a variável arq pelo nome do arquivo)

19. tail arq mostra as últimas 10 linhas de um arquivo (substituir a variável arq pelo nome do arquivo)

20. tail -f arq mostra o conteúdo de um arquivo enquanto ele é atualizado (aumenta de tamanho), iniciando com as últimas 10 linhas (substituir a variável arq pelo nome do arquivo)

21. ps mostra os processos de usuário ativos em tempo real￼

22. top mostra todos os processos rodando em tempo real

23. kill pid mata um processo específico pelo número ID (substituir pid pelo número do processo)

24. killall proc mata todos os processos com o nome especificado (proc, de processos (substituir proc pelo nome do processo)

25. bg lista trabalhos parados ou em segundo plano ou pode continua-los também

26. fg traz o trabalho mais recente para o primeiro plano

27. fg trab traz o trabalho “trab” para o primeiro plano (substituir trab pelo nome do processo)

28. chmod octal arq muda as permissões do arquivo “arq” para octal, que pode ser especificada separadamente para “usuário”, “grupo” e “outros”. Os valores em octal são representados abaixo:

4 – leitura (r, de read)

2 – gravação (w, de write)

1 – execução (x, de execute)

Explicação: Para definir permissões, somam-se os valores acima. Por exemplo, para atribuir ao dono do arquivo (“usuário) acesso total de leitura (r), gravação (w) e execução (x), basta somar o valor octal 4 + 2 + 1 = 7. Supondo que você queira limitar o acesso para membros do “grupo”, permitindo apenas a leitura e gravação, basta somar 4 + 2 = 6. Reunindo os dois exemplos citados, ficaria: chmod 760 (r para usuário, w para grupo e 0 para outros ou “rw-“)


_Outros exemplos_


1. chmod 777: leitura (r), gravação (w) e execução (x) para todos (“usuário”, “grupo” e “outros”)

2. chmod 755: “rwx” para o “dono” (usuário), “rw” para o “grupo” e “outros”

3. Para mais informações, digite no terminal: man chmod

4. ssh usuário@host: conecta ao host como usuário (exemplo: ssh computeiro@meuservidor)

5. ssh -p porta usuário@host conecta ao host na porta especificada (substituir “porta” pelo número da porta configurada)

6. ssh-copy-id usuário@host adiciona a sua chave para o host e usuário daquele host; serve para ativar logins sem senha com uso de chaves

7. grep sequência arquivos pesquisa pela sequência nos arquivos (substituir a sequência e arquivos pelos valores correspondentes à pesquisa)

8. grep –r sequência dir pesquisa recursivamente pela sequência no diretório dir

9. comando | grep sequência pesquisa pela sequência na saída do comando (substituir comando e sequência de acordo com os valores a serem buscados)

10. locate arq encontra todas as instâncias de um arquivo (substituir a variável arq pelo nome do arquivo)

11. date mostra a data e hora atual

12. cal mostra um calendário do mês atual

13. uptime mostra o tempo de atividade do sistema

14. w mostra quem está online

15. whoami mostra como quem você está logado

16. finger usuário mostra informações do usuário

17. uname -a mostra informações do kernels

18. cat /porc/cpuinfo mostra informações da CPU

19. cat /proc/meminfo mostra informações da memória

20. man comando abre o manual do comando especificado (substituir a variável comando pelo nome do comando que se quer conhecer)

21. df mostra o uso do disco

22. du mostra o uso do espaço em um diretório

23. free mostra o uso da memória e swap

24. whereis aplicação mostra possíveis localizações do aplicativo (substituir aplicação pelo nome do programa)

25. which aplicação mostra que aplicação irá rodar por omissão (substituir aplicação pelo nome do programa)

26. tar cf tar arqs cria um pacote TAR (nomeado pacote.tar) com os arquivos especificados (substituir a variável arqs pelo nome do arquivos)

27. tar xf tar extrai os arquivos de “pacote.tar” (substituir a variável pacote.tar pelo nome do arquivo)

28. tar czf tar.gz arqs cria um pacote TAR (nomeado pacote.tar.gz) com compressão GZip

29. tar xzf tar.gz extrai um pacote TAR (nomeado pacote.tar.gz) com compressão GZip

30. tar cjf tar.bz2 cria um pacote TAR (nomeado pacote.tar.bz2) com compressão BZip2

31. tar xjf tar.bz2 extrai um pacote TAR (nomeado pacote.tar.gz) com compressão BZip2

32. gzip arq compacta um arquivo e o renomeia para arq.gz (substituir a variável arq pelo nome do arquivo)

33. gzip -d gz descompacta arq.gz para um arquivo (substituir a variável arq.gz pelo nome do arquivo)

34. ping host envia um pacote ICMP (ping) para o host e mostra o resultado (substituir a variávelhost pelo domínio de um site ou o número IP)

35. whois domínio retorna informações sobre o domínio (substituir a variável domínio pelo endereço de um site ou o número IP)

36. dig domínio retorna informações de DNS para o domínio (substituir a variável host pelo domínio de um site ou o número IP)

37. dig -x host mostra o retorno reverso para um host (substituir a variável host pelo domínio de um site ou o número IP)

38. wget arq faz o download de arquivo (arq) (substituir a variável arq pelo endereço online do arquivo)

39. wget -c arq continua o download interrompido de um arquivo (arq) (substituir a variável arq pelo endereço online do arquivo)

40. Instalação a partir do código fonte (source code); os comandos devem ser digitados na sequência em um terminal, um de cada vez:

./configure
make
make install


_Comandos de instaladores_


1. dpkg -i deb instala um pacote DEB (distros Debian) (substituir a variável pacote.deb pelo nome do pacote de programa)

2. rpm -Uvh rpm instala um pacote RPM (Distros que utilizam RPM) (substituir a variávelpacote.rpmpelo nome do pacote de programa)

_Informações do sistema Linux_

1. arch: Mostre a arquitetura da máquina (1).

2. uname -m: Mostre a arquitetura da máquina (2).

3. uname -r: Mostre versão do kernel usada.

4. dmidecode -q: Mostre os componentes do sistema (hardware).

5. hdparm -i /dev/hda: Mostre as características de um disco rígido.

6. hdparm -tT /dev/sda: Execute teste de leitura em um disco rígido.

7. cat /proc/cpuinfo: Exiba informações da CPU.

8. cat /proc/interrupts: Mostre interrupções.

9. cat /proc/meminfo: verificar a utilização de memória.

10. cat /proc/swaps:df -h: Mostre o tamanho dos arquivos e diretórios ordenados por tamanho.

11. ls -lSr |more: Estimar o espaço usado pelo diretório ‘dir1’.

12. du -sh dir1: Mostre o tamanho dos arquivos e diretórios ordenados por tamanho.

13. du -sk * | sort -rn: mostra o espaço usado por pacotes rpm instalados organizado pelo tamanho (Fedora, Red Hat e outros).

14. rpm -q -a –qf ‘%10{SIZE}t%{NAME}n’ | sort -k1,1n: mostra o espaço usado por pacotes instalados, organizado pelo tamanho (Debian, Ubuntu e outros).

15. dpkg-query -W -f=’${Installed-Size;10}t${Package}n’ | sort -k1,1n: g> Mostre arquivos de swap.

16. cat /proc/version: Exiba a versão do kernel.

17. cat /proc/net/dev: Mostre estatísticas e adaptadores de rede.

18. cat /proc/mounts: Mostre o sistema de arquivos montado.

19. lspci -tv: exiba os dispositivos PCI.

20. lsusb -tv: Mostre os dispositivos USB.

21. date: Mostre a data do sistema.

22. cal 2011: Visualizar o calendário em 2011.

23. cal 07 2011: Mostre o calendário para o mês de julho de 2011.

24. date 041217002011.00: Coloque (estado, ajustar) data e hora.

25. clock -w: Salve as alterações para a data na BIOS.


_Arquivos e diretórios_


1. cd /home: Digite o diretório “em casa”.

2. cd ..: Volte um nível.

3. cd ../..: volta 2 níveis.

4. cd: Vá para o diretório de raiz.

5. cd ~user1: Vá para o diretório de user1.

6. cd -: Volte para o diretório anterior.

7. pwd: Mostre o caminho do diretório de trabalho.

8. ls: consulte os arquivos em um diretório.

9. ls -F: consulte os arquivos em um diretório.

10. ls -l: mostre detalhes de arquivos e pastas em um diretório.

11. ls -a: Mostre arquivos ocultos.

12. ls *[0-9]*: Mostre arquivos e pastas que contêm números.

13. tree: Mostre arquivos e pastas em uma árvore a partir da raiz. (1)

14. lstree: Mostre arquivos e pastas em uma árvore a partir da raiz. (2)

15. mkdir dir1: Crie uma pasta ou diretório com nome ‘dir1’.

16. mkdir dir1 dir2: Crie duas pastas ou diretórios simultaneamente (criando dois diretórios ao mesmo tempo).

17. mkdir -p /tmp/dir1/dir2: Crie uma árvore de diretório.

18. rm -f file1: Exclua o arquivo chamado ‘arquivo1’.

19. rmdir dir1: Exclua a pasta chamada ‘dir1’.

20. rm -rf dir1: exclua uma pasta chamada ‘dir1’ com seu conteúdo recursivamente. (Se excluí-lo recursivo que estou a dizer que é com o seu conteúdo).

21. rm -rf dir1 dir2: Exclua duas pastas (diretórios) com seu conteúdo recursivamente.

22. mv dir1 new_dir: Renomear ou mover um arquivo ou pasta (diretório).

23. cp file1: Copie um arquivo.

24. cp file1 file2: Copie os dois arquivos ao mesmo tempo.

25. cp dir /* .: Copie todos os arquivos de um diretório dentro do diretório de trabalho atual.

26. cp -a /tmp/dir1 .: Copie um diretório dentro do diretório de trabalho atual.

27. cp -a dir1: Copie um diretório.

28. cp -a dir1 dir2: diretório de cópia dois em uníssono.

29. ln -s file1 lnk1: Crie um link simbólico para o arquivo ou diretório.

30. ln file1 lnk1: Crie um vínculo físico para o arquivo ou diretório.

31. touch -t 0712250000 file1: modifica o tempo real (tempo de criação) de um arquivo ou diretório.

32. file file1: saída (despejo na tela) do tipo mime de um arquivo de texto.

33. iconv -l: listas de cifras conhecidas.

34. iconv -f fromEncoding -t toEncoding inputFile > outputFile: Crie uma nova forma de arquivo de entrada assumindo que está codificado em fromEncoding e convertê-lo para ToEncoding.

35. find . -maxdepth 1 -name *.jpg –print -exec convert ”{}” -resize 80×60 “thumbs/{}” \;: agrupando arquivos dimensionados no diretório atual e enviá-los aos diretórios em visualização de miniaturas (requer o converso do ImagemagicK).


_Encontrar arquivos_


1. find / -name file1: busca de arquivo e diretório da raiz do sistema.

2. find / -user user1: Encontre arquivos e diretórios pertencentes ao usuário ‘user1’.

3. find /home/user1 -name \*.bin: Procure arquivos com extensão ‘. bin’ no diretório ‘/ home/user1’.

4. find /usr/bin -type f -atime +100: Pesquisar arquivos binários não utilizados nos últimos 100 dias.

5. find /usr/bin -type f -mtime -10: Pesquisar arquivos criados ou alterados nos últimos 10 dias.

6. find / -name \*.rpm -exec chmod 755 ‘{}’ \;: Procure arquivos com extensão ‘. rpm’ e modificar permissões.

7. find / -xdev -name \*.rpm: Procure arquivos com extensão ‘. rpm’ ignorando a mídia removível, como CD-ROM, pen-drive, etc…

8. locate \*.ps: encontrar arquivos com a extensão ‘. ps primeiro executado com o comando “updatedb’.

9. whereis halt: Mostre a localização de um arquivo binário, a ajuda ou a fonte. Neste caso ele pergunta onde está o comando ‘parada’.

10. which halt: mostrar o caminho completo (o caminho completo) para um binário / executável.


_Trabalhando com sistema de arquivos_


1. mount /dev/hda2 /mnt/hda2: Monte um disco chamado hda2. Primeiro, verifique a existência do diretório ‘/ mnt/hda2’; Se você não estiver, você deve criá-lo.

2. umount /dev/hda2: Remova um disco chamado hda2. Em primeiro lugar, do ponto de ‘ / mnt/hda2.

3. fuser -km /mnt/hda2: Force a remoção quando o dispositivo está ocupado.

4. umount -n /mnt/hda2: Execute a remoção sem ler o arquivo/etc/MTAB. Útil quando o arquivo é somente leitura ou o disco rígido está cheio.

5. mount /dev/fd0 /mnt/floppy: Monte um disco flexível (disquete).

6. mount /dev/cdrom /mnt/cdrom: montar um cdrom / dvdrom.

7. mount /dev/hdc /mnt/cdrecorder: Monte um cd gravável ou um dvdrom.

8. mount /dev/hdb /mnt/cdrecorder: montar um cd gravável / dvdrom (um dvd).

9. mount -o loop file.iso /mnt/cdrom: Monte um arquivo ou uma imagem iso.

10. mount -t vfat /dev/hda5 /mnt/hda5: Monte um sistema de aComandos rquivos FAT32.

11. mount /dev/sda1 /mnt/usbdisk: Monte uma memória ou um pen-drive usb (sem especificar o tipo de sistema de arquivos).


_Espaço em disco_


1. df -h: Mostre o tamanho dos arquivos e diretórios ordenados por tamanho.

2. ls -lSr |more: Estimar o espaço usado pelo diretório ‘dir1’.

3. du -sh dir1: Mostre o tamanho dos arquivos e diretórios ordenados por tamanho.

4. du -sk * | sort -rn: mostra o espaço usado por pacotes rpm instalados organizado pelo tamanho (Fedora, Red Hat e outros).

5. rpm -q -a –qf ‘%10{SIZE}t%{NAME}n’ | sort -k1,1n: mostra o espaço usado por pacotes instalados, organizado pelo tamanho (Debian, Ubuntu e outros).

6. dpkg-query -W -f=’${Installed-Size;10}t${Package}n’ | sort -k1,1n: Mostrar (no Debian ou derivados) uma lista com 25 pacotes instalados que consomem mais espaço (em ordem decrescente)


_Usuários e grupos_


1. groupadd nombre_del_grupo: Crie um novo grupo.

2. groupdel nombre_del_grupo: Exclua um grupo.

3. groupmod -n nuevo_nombre_del_grupo viejo_nombre_del_grupo: Renomear um grupo.

4. useradd -c “Name Surname ” -g admin -d /home/user1 -s /bin/bash user1: Crie um novo usuário “admin” do grupo.

5. useradd user1: Crie um novo usuário.

6. userdel -r user1: excluir um usuário (‘-r’ elimina o diretório Home).

7. usermod -c “User FTP” -g system -d /ftp/user1 -s /bin/nologin user1: Altere os atributos do usuário.

8. passwd: Altere senha.

9. passwd user1: Altere a senha do usuário (apenas pelo root).

10. chage -E 2011-12-31 user1: Defina um limite de tempo para a senha do usuário. Neste caso, ele diz que a chave expira a 31 de dezembro de 2011.Informações do sistema Linux
pwck: Verifique a sintaxe correta ‘/ etc/passwd’ arquivo formato e a existência de usuários.

11. grpck: Verifique a sintaxe correta e formato do arquivo ‘/ etc/grupo’ e a existência de grupos.

12. newgrp group_name: Registre um novo grupo para alterar o grupo padrão dos arquivos recém-criados.


_Permissões de Arquivos (+ Adiciona e – Remover permissões)_


1. ls -lh: Mostre permissões.

2. ls /tmp | pr -T5 -W$COLUMNS: Divida o terminal em 5 colunas.

3. chmod ugo+rwx directory1: definir permissões de leitura®, gravar (w) e executar (x) para o dono (u), grupo (g) e outros (ou) no diretório ‘arquivo1’.

4. chmod go-rwx directory1: Remove® a permissão de leitura, gravação (w) e grupo de implementação (x) (g) e outros (ou) no diretório ‘arquivo1’.

5. chown user1 file1: Altere o proprietário de um arquivo.

6. chown -R user1 directory1: Altere o proprietário de um diretório e todos os arquivos e diretórios contidos dentro.

7. chgrp group1 file1: Altere o grupo de arquivos.

8. chown user1: Grupo1 arquivo1

9. find / -perm -u+s: Ver todos os arquivos com sistema SUID configurado.

10. chmod u+s /bin/file1: Defina o bit SUID em um arquivo binário. O usuário que está executando esse arquivo adquire os mesmos privilégios como proprietário.

11. chmod u-s /bin/file1: Desabilite o bit SUID em um arquivo binário.

12. chmod g+s /home/public: definir o SGID bit em um diretório – semelhante ao SUID, mas para o diretório.

13. chmod g-s /home/public: Desative o bit SGID em um diretório.

14. chmod o+t /home/public: conjunto STIKY bit em um diretório. Permite a exclusão de arquivos somente para os legítimos proprietários.

15. chmod o-t /home/public: Desative STIKY bit em um diretório.


_Atributos especiais de arquivo: (“+” Adiciona e “–” Remover permissões)_


1. chattr +a file1: permite gravar apenas abrindo um arquivo acrescentar modo.

2. chattr +c file1: permite que um arquivo a ser compactado / descompactado automaticamente.

3. chattr +d file1: Ele garante que o programa ignore excluir os arquivos durante o backup.

4. chattr +i file1: torna-se o arquivo inalterado, portanto não pode ser excluído, alterado, renomeado ou vinculado.

5. chattr +s file1: Permite que um arquivo a ser excluído com segurança.

6. chattr +S file1: Ele garante que um arquivo é modificado, as alterações são gravadas no modo síncrono, como com a sincronia.

7. chattr +u file1: Ele permite que você recuperar o conteúdo de um arquivo, mesmo se está cancelado.

8. lsattr: Mostre atributos especiais.


_Arquivos e arquivos compactados_


1. bunzip2 file1.bz2: Descompacte um arquivo chamado ‘file1.bz2’.

2. bzip2 file1: comprime um arquivo chamado ‘file1’.

3. gunzip file1.gz: Descompacte um arquivo chamado ‘file1.gz’.

4. gzip file1: comprime um arquivo chamado ‘file1’.

5. gzip -9 file1: Comprima com compressão máxima.

6. rar a file1.rar test_file: Crie um arquivo com o rar chamado ‘file1.rar’.

7. rar a file1.rar file1 file2 dir1: Comprima ‘arquivo1’, ‘arquivo2’ e ‘dir1’ simultaneamente.

8. rar x file1.rar: Descompacte o arquivo rar.

9. unrar x file1.rar: Descompacte o arquivo rar.

10. tar -cvf archive.tar file1: Crie um tarball descompactado.

11. tar -cvf archive.tar file1 file2 dir1: Crie um arquivo contendo ‘arquivo1’, ‘ file2′ e ‘dir1’.

12. tar -tf archive.tar: exibir o conteúdo de um arquivo.

13. tar -xvf archive.tar: extrair um arquivo tar.

14. tar -xvf archive.tar -C /tmp: extrair um tarball em / tmp.

15. tar -cvfj archive.tar.bz2 dir1: Crie um arquivo tar compactado no bzip2.

16. tar -xvfj archive.tar.bz2: descompactar um arquivo compactado do bzip2 tar

17. tar -cvfz archive.tar.gz dir1: Crie um arquivo tar compactado em gzip.

18. tar -xvfz archive.tar.gz: Descompacte um arquivo tar do gzip compactado.

19. zip file1.zip file1: Crie um arquivo compactado zip.

20. zip -r file1.zip file1 file2 dir1: compressão, zip, vários arquivos e diretórios simultaneamente.

21. unzip file1.zip: Descompacte um arquivo zip.


_Pacotes RPM (Red Hat, Fedora e similares)_


1. rpm -ivh package.rpm: Instale um pacote rpm.

2. rpm -ivh –nodeeps package.rpm: Instale um pacote rpm ignorar solicitações de dependências.

3. rpm -U package.rpm: atualize um pacote rpm sem alterar a configuração dos arquivos.

4. rpm -F package.rpm: atualize um pacote rpm somente se ele estiver instalado.

5. rpm -e package_name.rpm: Remova um pacote rpm.

6. rpm -qa: Mostre todos os pacotes rpm instalados no sistema.

7. rpm -qa | grep httpd: Mostre todos os rpm de pacotes com o nome “httpd”.

8. rpm -qi package_name: informações sobre um pacote específico instalado.

9. rpm -qg “System Environment/Daemons”: Mostar um grupo software pacotes rpm.

10. rpm -ql package_name: Mostre lista de arquivos fornecidos por um pacote rpm instalados.

11. rpm -qc package_name: Exiba a lista de arquivos, dada por uma configuração de pacote rpm instalados.

12. rpm -q package_name –whatrequires: Mostre lista de dependências que são solicitados para um pacote rpm.

13. rpm -q package_name –whatprovides: Mostar capacidade fornecida por um pacote rpm.

14. rpm -q package_name –scripts: Mostre scripts começados durante a remoção da instalação.

15. rpm -q package_name –changelog: Mostar o histórico das revisões de um pacote rpm.

16. rpm -qf /etc/httpd/conf/httpd.conf: Verificar qual rpm pacote pertence um determinado arquivo.

17. rpm -qp package.rpm -l: Mostre lista de arquivos fornecidos por um rpm do pacote que ainda não foi instalado.

18. rpm –import /media/cdrom/RPM-GPG-KEY: importe a assinatura digital chave pública.

19. rpm –checksig package.rpm: Verificar a integridade de um pacote rpm.

20. rpm -qa gpg-pubkey: Verificar a integridade de todos os pacotes rpm instalados.

21. rpm -V package_name: Verifique o tamanho do arquivo, licenças, tipos, proprietário, grupo, exame de saúde Resumo de MD5 e última modificado.

22. rpm -Va: verificar todos os pacotes rpm instalados no sistema. Use com cuidado.

23. rpm -Vp package.rpm: Verifique se que um pacote instalado ainda não rpm.

24. rpm2cpio package.rpm | cpio –extract –make-directories *bin*: Extraia o arquivo executável de um pacote rpm.

25. rpm -ivh /usr/src/redhat/RPMS/arch/package.rpm: Instale um pacote construído a partir de um rpm fonte.

26. rpmbuild –rebuild package_name.src.rpm: Construa um pacote rpm a partir de um rpm fonte.


_Pacotes YUM Updater (Red Hat, Fedora e similares)_


1. yum install package_name: Baixar e instalar um pacote rpm.

2. yum localinstall package_name.rpm: Isto irá instalar um RPM e vai tentar resolver todas as dependências para você, usando seus repositórios.

3. yum update package_name.rpm: Atualize todos os pacotes rpm instalados no sistema.

4. yum update package_name: Upgrade / atualizar um pacote rpm.

5. yum remove package_name: Remova um pacote rpm.

6. yum list: Liste todos os pacotes instalados no sistema.

7. yum search package_name: Encontre um pacote no repositório rpm.

8. yum clean packages: Limpe um cache de rpm, apagando os pacotes baixados.

9. yum clean headers: exclua todo o cabeçalho de arquivos que o sistema usa para resolver a dependência.

10. yum clean all: Remova os arquivos de cache e o cabeçalho do pacote.


_Pacotes deb (Debian, Ubuntu e derivados)_


1. dpkg -i package.deb: instalar / atualizar um pacote deb.

2. dpkg -r package_name: Remova uma deb para o pacote do sistema.

3. dpkg -l: Mostre todos os pacotes deb instalados no sistema.

4. dpkg -l | grep httpd: Mostre todos deb pacotes com o nome “httpd”

5. dpkg -s package_name: informações sobre um pacote específico instalado no seu sistema.

6. dpkg -L package_name: Mostar lista de arquivos fornecidos por um pacote instalado no sistema.

7. dpkg –contents package.deb: Mostre lista de arquivos fornecidos por um pacote não instalado ainda.

8. dpkg -S /bin/ping: Verificar qual pacote pertence um determinado arquivo.


_Atualizador de pacotes APT (Debian, Ubuntu y derivados)_


1. apt-get install package_name: instalar / atualizar um pacote deb.

2. apt-cdrom install package_name: instalar / atualizar um pacote deb do cdrom.

3. apt-get update: Atualize a lista de pacotes.

4. apt-get upgrade: Atualize pacotes instalados todos.

5. apt-get remove package_name: Remova a instalação de um pacote deb do sistema.

6. apt-get check: Verifique se a resolução correta de dependências.

7. apt-get clean: limpar o cache de pacotes baixados.

8. apt-cache search searched-package: Retorna a lista de pacotes que corresponde à série ‘queria pacotes’.


_Exibir o conteúdo de um arquivo_


1. cat file1: Ver o conteúdo de um arquivo a partir da primeira linha.

2. tac file1: Ver o conteúdo de um arquivo a partir da última linha.

3. more file1: Veja o conteúdo ao longo de um arquivo.

4. less file1: semelhantes para o comando ‘mais’ mas permite que você salve o arquivo, bem como o movimento para trás.

5. head -2 file1: Veja as duas primeiras linhas de um arquivo.

6. tail -2 file1: Ver as duas últimas linhas de um arquivo.

7. tail -f /var/log/messages: Ver em tempo real o que foi adicionado ao arquivo.


_Manipulação de texto_


1. cat file1 file2 .. | command <> file1_in.txt_or_file1_out.txt: sintaxe geral para a manipulação de texto usando o tubo, STDIN e STDOUT.

2. cat file1 | command( sed, grep, awk, grep, etc…) > result.txt: sintaxe geral para manipular um texto de um arquivo e escrever os resultados para um novo arquivo.

3. cat file1 | command( sed, grep, awk, grep, etc…) » result.txt: sintaxe geral para manipular um texto de um arquivo e adicionar o resultado em um arquivo existente.

4. grep Aug /var/log/messages: Procure as palavras “Ago” no arquivo ‘/ var/log/messages’.

5. grep ^Aug /var/log/messages: procurar palavras que começam com “Agosto” no arquivo ‘/ var/log/messages’

6. grep [0-9] /var/log/messages: Selecione todas as linhas no arquivo ‘/ var/log/messages’ que contêm números.

7. grep Aug -R /var/log/*: encontrar a seqüência de caracteres “Ago” no diretório ‘ / var/log ‘ e abaixo.

8. sed ‘s/stringa1/stringa2/g’ example.txt: Realocando “string1” com “string2” em Sample. txt

9. sed ‘/^$/d’ example.txt: remover todas as linhas em branco do sample. txt

10. sed ‘/ *#/d; /^$/d’ example.txt: excluir comentários e linhas em branco de Sample. txt

11. echo ‘esempio’ | tr ‘[: baixa

12. sed -e ‘1d’ result.txt: elimina a primeira linha do arquivo Sample. txt

13. sed -n ‘/stringa1/p’: exibir somente as linhas que contêm a palavra “string1”.


_Estabelecer o formato de conversão de arquivos_


1. dos2unix filedos.txt fileunix.txt: Converta um formato de arquivo de texto do MSDOS para UNIX.

2. unix2dos fileunix.txt filedos.txt: Converta um formato de arquivo de texto do UNIX para MSDOS.

3. recode ..HTML < page.txt > page.html: Converta um arquivo de texto para html.

4. recode -l | more: Mostre todas as conversões de formato disponíveis.


_Análise de sistema de arquivos_


1. badblocks -v /dev/hda1: Verifica os blocos defeituosos no disco hda1.

2. fsck /dev/hda1: reparar / verificar a integridade do arquivo do sistema Linux no disco hda1.

3. ext2 /dev/hda1: reparação / verificar a integridade do sistema de arquivo ext2 no disco hda1.

4. e2fsck /dev/hda1: reparação / verificar a integridade do sistema de arquivo ext2 no disco hda1.

5. e2fsck -j /dev/hda1: reparação / verificar a integridade do sistema de arquivo ext3 no disco hda1.

6. ext3 /dev/hda1: reparação / verificar a integridade do sistema de arquivo ext3 no disco hda1.

7. vfat /dev/hda1: reparação / verificar integridade do arquivo sistema disco fat hda1.

8. msdos /dev/hda1: reparar / verificar a integridade de um arquivo a partir do dos sistema disco hda1.

9. dosfsck /dev/hda1: reparar / verificar a integridade de um arquivo a partir do dos sistema disco hda1.


_Formatar sistema de arquivos_


1. mkfs /dev/hda1: Verifica os blocos defeituosos no disco hda1.

2. mke2fs /dev/hda1: reparar / verificar a integridade do arquivo do sistema Linux no disco hda1.

3. mke2fs -j /dev/hda1: reparação / verificar a integridade do sistema de arquivo ext2 no disco hda1.

4. mkfs -t vfat 32 -F /dev/hda1: reparação / verificar a integridade do sistema de arquivo ext2 no disco hda1.

5. fdformat -n /dev/fd0: reparação / verificar a integridade do sistema de arquivo ext3 no disco hda1.

6. mkswap /dev/hda3: reparação / verificar a integridade do sistema de arquivo ext3 no disco hda1.


_Backups_


1. dump -0aj -f /tmp/home0.bak /home: Fazer um completo salvar do directório ‘/Home’.

2. dump -1aj -f /tmp/home0.bak /home: Fazer um Backup incremental do diretório ‘ /home’.

3. restore -if /tmp/home0.bak: Restaurando um save interativamente.

4. rsync -rogpav –delete /home /tmp: Sincronização entre diretórios.

5. rsync -rogpav -e ssh –delete /home ip_address: rsync através do túnel SSH.

6. rsync -az -e ssh –delete ip_addr: Sincronizar um diretório local com um diretório remoto via ssh e compressão.

7. rsync -az -e ssh –delete /home/local ip_addr: sincronizar um diretório remoto em um diretório local através de ssh e compressão.

8. dd bs=1M if=/dev/hda | gzip | ssh user@ip_addr ‘dd of=hda.gz’: fazer um salvamento em um disco rígido em um host remoto através de ssh.

9. dd if=/dev/sda of=/tmp/file1: Salve o conteúdo de um disco rígido para um arquivo. (Neste caso o disco rígido é “sda” e o arquivo “file1”).

10. tar -Puf backup.tar /home/user: Salvar os diretórios/etc e a raiz (excluindo o conteúdo do subdiretório/root/dir1 /) em um arquivo compactado, cujo nome inclui a data e hora atual.

11. ( cd /tmp/local/ && tar c . ) | ssh -C user@ip_addr ‘cd /home/share/ && tar x -p’: Copie o conteúdo de um diretório em um diretório remoto através de ssh.

12. ( tar c /home ) | ssh -C user@ip_addr ‘cd /home/backup-home && tar x -p’: copiar um diretório local em um diretório remoto através de ssh.

13. tar cf – . | (cd /tmp/backup ; tar xf – ): cópia local preservando licenças e links de um diretório para outro.

14. find /home/user1 -name ‘*.txt’ | xargs cp -av –target-directory=/home/backup/ –parents:encontrar e copiar todos os arquivos com extensão ‘. txt’ de um diretório para outro

15. find /var/log -name ‘*.log’ | tar cv –files-from=- | bzip2 > log.tar.bz2: encontrar todos os arquivos com extensão ‘. log’ e fazer um arquivo bzip.

16. dd if=/dev/hda of=/dev/fd0 bs=512 count=1: Faça uma cópia do MRB (Master Boot Record) para um disquete.

17. dd if=/dev/fd0 of=/dev/hda bs=512 count=1: Restaurar a cópia da (MBR Master Boot Record) gravada no disquete.


_CD-ROM_


1. cdrecord -v gracetime=2 dev=/dev/cdrom -eject blank=fast -force: limpar ou apagar um cd regravável.

2. mkisofs /dev/cdrom > cd.iso: Crie uma imagem iso do CD-ROM no disco.

3. mkisofs /dev/cdrom | gzip > cd_iso.gz: Crie uma imagem iso compactada do CD-ROM no disco.

4. mkisofs -J -allow-leading-dots -R -V “Label CD” -iso-level 4 -o ./cd.iso data_cd: Crie uma imagem iso de um diretório.

5. cdrecord -v dev=/dev/cdrom cd.iso: grave uma imagem iso.

6. gzip -dc cd_iso.gz | cdrecord dev=/dev/cdrom –: grave uma imagem iso comprimida.

7. mount -o loop cd.iso /mnt/iso: Monte uma imagem iso.

8. cd-paranoia -B: Tire músicas de um cd para arquivos wav.

9. cd-paranoia – ”-3”: Pegue as 3 primeiras músicas de um cd para arquivos wav.

10. cdrecord –scanbus: varredura de ônibus para identificar o canal

11. dd if=/dev/hdc | md5sum: Execute um md5sum em um dispositivo, como um CD.


_Redes (LAN e Wi-Fi)_


1. ifconfig eth0: Mostre a configuração de uma placa de rede Ethernet.

2. ifup eth0: Ative uma interface ‘eth0’.

3. ifdown eth0: Desabilite uma interface ‘eth0’.

4. ifconfig eth0 192.168.1.1 netmask 255.255.255.0: Configure um endereço IP.

5. ifconfig eth0 promisc: Configure ‘eth0’ modo comum para obter pacotes (sniffing).

6. dhclient eth0: Ative a interface ‘eth0’ em modo dhcp.

7. route -n: Mostre tabela de rota.

8. route add -net 0/0 gw IP_Gateway: Configure a entrada padrão.

9. route add -net 192.168.0.0 netmask 255.255.0.0 gw 192.168.1.1: Configure uma rota estática para encontrar a rede, ‘192.168.0.0/16’.

10. route del 0/0 gw IP_gateway: Remova a rota estática.

11. echo “1” > /proc/sys/net/ipv4/ip_forward: Ative o ip de rota.

12. hostname: Exiba o nome do host do sistema.

13. host example.com: Encontre o nome do host para resolver o nome de um IP (1).

14. nslookup example.com: Encontre o nome do host para resolver o nome de um ip e vice-versa (2).

15. ip link show: Mostra o status de todas as interfaces.

16. mii-tool eth0: Mostar o status de ‘eth0’ link.

17. ethtool eth0: Exiba estatísticas da placa de rede ‘eth0’.

18. netstat -tup: Mostre todas as conexões de rede ativa e seu PID.

19. netstat -tupl: Mostre todos os ouvinte de rede de serviços sobre o sistema e seu PID.

20. tcpdump tcp port 80: Mostre todo o tráfego HTTP.

21. iwlist scan: Mostre as redes sem fio.

22. iwconfig eth1: Mostre a configuração de uma placa de rede sem fio.

23. whois example.com: Pesquisa Base de dados Whois .


_Redes Microsoft Windows (SAMBA)_


1. nbtscan ip_addr: resolução de nome de rede do BIOS.

2. nmblookup -A ip_addr: resolução de nome de rede do BIOS.

3. smbclient -L ip_addr/hostname: Visualizar compartilhamentos remotos de um host windows.


_Firewall (iptables)_


1. iptables -t filter -L: Mostre todas as correntes na tabela de filtro.

2. iptables -t nat -L: Mostre todas as correntes da tabela nat.

3. iptables -t filter -F: Limpe todas as regras da tabela de filtro.

4. iptables -t nat -F: Limpe todas as regras da tabela nat.

5. iptables -t filter -X: exclua qualquer cadeia criados pelo usuário.

6. iptables -t filter -A INPUT -p tcp –dport telnet -j ACCEPT: permita conexões telnet de entrar.

7. iptables -t filter -A OUTPUT -p tcp –dport http -j DROP: bloquear conexões HTTP de saída.

8. iptables -t filter -A FORWARD -p tcp –dport pop3 -j ACCEPT: permitindo conexões POP para uma cadeia de frente.

9. iptables -t filter -A INPUT -j LOG –log-prefix “DROP INPUT”: registrando uma sequência de entrada.

10. iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE: Configure uma PAT (conversão de endereços de porta) na eth0, escondendo os pacotes de saída de coação.

11. iptables -t nat -A PREROUTING -d 192.168.0.1 -p tcp -m tcp –dport 22 -j DNAT –to-destination 10.0.0.2


_Monitoramento e depuração_


1. top: Exiba tarefas linux usando mais cpu.

2. ps -eafw: Exibe as tarefas do Linux.

3. ps -e -o pid,args –forest: Exibe as tarefas do Linux de forma hierárquica.

4. pstree: Mostre uma árvore de processos do sistema.

5. kill -9 ID_Processo: forçar o encerramento de um processo e terminá-lo.

6. kill -1 ID_Processo: força um processo para recarregar a configuração.

7. lsof -p $$: Exiba uma lista de arquivos abertos por processos.

8. lsof /home/user1: Exibe uma lista de arquivos abertos em um determinado caminho do sistema.

9. strace -c ls >/dev/null: Mostre o sistema de chamadas feitas e recebidas por um processo.

10. strace -f -e open ls >/dev/null: Visualizar chamadas para a biblioteca.

11. watch -n1 ‘cat /proc/interrupts’: Mostre interrupções em tempo real.

12. last reboot: Reinicialização de história do programa.

13. lsmod: Exiba o kernel carregado.

14. free -m: Exibe o status da RAM em megabytes.

15. smartctl -A /dev/hda: Monitore a confiabilidade de um disco rígido através do SMART.

16. smartctl -i /dev/hda: Verifique se o SMART está habilitado em um disco rígido.

17. tail /var/log/dmesg: Mostre os eventos inerentes no processo de carregar o kernel.

18. tail /var/log/messages: Mostre eventos de sistema.


_Dicas e Comandos úteis_


1. apropos …keyword: exibir uma lista de comandos que pertencem às palavras-chave de um programa; Eles são úteis quando você sabe o que faz o seu programa, mas sconoces o nome do comando.

2. man ping: exibir as páginas de manual on-line; por exemplo, um comando ping, use a opção ‘-k’ para encontrar qualquer comandos relacionados.

3. whatis …keyword: Exibe a descrição do que o programa faz.

4. mkbootdisk –device /dev/fd0 uname -r: Crie um disquete boteable.

5. gpg -c file1: codifica um arquivo com o guarda de segurança do GNU.

6. gpg file1.gpg: decodificar um arquivo com o guarda de segurança do GNInformações do sistema LinuxU.

7. wget -r example.com: Baixe um site inteiro.

8. wget -c example.com/file.iso: Baixe um arquivo com a possibilidade de parar o download e retomar mais tarde.

9. echo ‘wget -c example.com/files.iso‘ | at 09: 00

10. ldd /usr/bin/ssh: Mostrar compartilhada bibliotecas exigirem pelo ssh programa.

11. alias hh=’history’: Coloque um alias para um comando – hh = história.

12. chsh: Mude o Shell de comando.

13. chsh –list-shells: É um comando adequado para descobrir se você tem controle remoto em outro terminal.

14. clear: Limpa a tela do terminal.

15. umcomando > archivodesaida.txt 2>&1: executa um comando e redirecionar saída para um arquivo, combinando neste ambos STDOUT e STDERR.

16. umcomando | archivodesaida.txt 2> archivodeerros.txt: Executar um comando, você redirecionar a saída (STDOUT) para um arquivo e os erros (STDERR) para outro.

17. umcomando | tee arquivodesaida.txt: executa um comando, exibe a saída na tela e, simultaneamente, grava-lo em um arquivo.

# Comandos GitHub

_Estados_

Modificado (modified);
Preparado (staged/index)
Consolidado (comitted);

_Ajuda_

Geral

git help

Comando específico

git help add
git help commit
git help <qualquer_comando_git>

_Configuração_

Geral

As configurações do GIT são armazenadas no arquivo .gitconfig localizado dentro do diretório do usuário do Sistema Operacional (Ex.: Windows: C:\Users\Documents and Settings\Leonardo ou *nix /home/leonardo).

As configurações realizadas através dos comandos abaixo serão incluídas no arquivo citado acima.

Setar usuário

git config --global user.name "Leonardo Comelli"

Setar email
git config --global user.email leonardo@software-ltda.com.br

Setar editor
git config --global core.editor vim

Setar ferramenta de merge
git config --global merge.tool vimdiff

Setar arquivos a serem ignorados
git config --global core.excludesfile ~/.gitignore

Listar configurações
git config --list

Ignorar Arquivos

- Os nomes de arquivos/diretórios ou extensões de arquivos listados no arquivo .gitignore não serão adicionados em um repositório. Existem dois arquivos .gitignore, são eles:

- Geral: Normalmente armazenado no diretório do usuário do Sistema Operacional. O arquivo que possui a lista dos arquivos/diretórios a serem ignorados por todos os repositórios deverá ser declarado conforme citado acima. O arquivo não precisa ter o nome de .gitignore.

- Por repositório: Deve ser armazenado no diretório do repositório e deve conter a lista dos arquivos/diretórios que devem ser ignorados apenas para o repositório específico.

_Repositório Local_

Criar novo repositório
git init

Verificar estado dos arquivos/diretórios
git status

Adicionar arquivo/diretório (staged area)
Adicionar um arquivo em específico
git add meu_arquivo.txt

Adicionar um diretório em específico
git add meu_diretorio

Adicionar todos os arquivos/diretórios
git add .	

Adicionar um arquivo que esta listado no .gitignore (geral ou do repositório)
git add -f arquivo_no_gitignore.txt

_Comitar arquivo/diretório_

Comitar um arquivo
git commit meu_arquivo.txt

Comitar vários arquivos
git commit meu_arquivo.txt meu_outro_arquivo.txt

Comitar informando mensagem
git commit meuarquivo.txt -m "minha mensagem de commit"

_Remover arquivo/diretório_

Remover arquivo
git rm meu_arquivo.txt

Remover diretório
git rm -r diretorio

Visualizar histórico
Exibir histórico
git log

Exibir histórico com diff das duas últimas alterações
git log -p -2

Exibir resumo do histórico (hash completa, autor, data, comentário e qtde de alterações (+/-))
git log --stat

Exibir informações resumidas em uma linha (hash completa e comentário)
git log --pretty=oneline

Exibir histórico com formatação específica (hash abreviada, autor, data e comentário)
git log --pretty=format:"%h - %an, %ar : %s"

- %h: Abreviação do hash;
- %an: Nome do autor;
- %ar: Data;
- %s: Comentário.
- Verifique as demais opções de formatação no Git Book

Exibir histório de um arquivo específico
git log -- <caminho_do_arquivo>

Exibir histórico de um arquivo específico que contêm uma determinada palavra
git log --summary -S<palavra> [<caminho_do_arquivo>]
  
Exibir histórico modificação de um arquivo
git log --diff-filter=M -- <caminho_do_arquivo>
- O pode ser substituido por: Adicionado (A), Copiado (C), Apagado (D), Modificado (M), Renomeado (R), entre outros.

Exibir histório de um determinado autor
git log --author=usuario

Exibir revisão e autor da última modificação de uma bloco de linhas
git blame -L 12,22 meu_arquivo.txt 
  
_Desfazendo operações_

Desfazendo alteração local (working directory)
Este comando deve ser utilizando enquanto o arquivo não foi adicionado na staged area.
git checkout -- meu_arquivo.txt

Desfazendo alteração local (staging area)
Este comando deve ser utilizando quando o arquivo já foi adicionado na staged area.
git reset HEAD meu_arquivo.txt

Se o resultado abaixo for exibido, o comando reset não alterou o diretório de trabalho.
Unstaged changes after reset:
M	meu_arquivo.txt

A alteração do diretório pode ser realizada através do comando abaixo:
git checkout meu_arquivo.txt

_Repositório Remoto_

Exibir os repositórios remotos
git remote
git remote -v

Vincular repositório local com um repositório remoto
git remote add origin git@github.com:leocomelli/curso-git.git

Exibir informações dos repositórios remotos
git remote show origin

Renomear um repositório remoto
git remote rename origin curso-git

Desvincular um repositório remoto
git remote rm curso-git

Enviar arquivos/diretórios para o repositório remoto

O primeiro push de um repositório deve conter o nome do repositório remoto e o branch.
git push -u origin master

Os demais pushes não precisam dessa informação
git push

Atualizar repositório local de acordo com o repositório remoto

Atualizar os arquivos no branch atual
git pull

Buscar as alterações, mas não aplica-las no branch atual
git fetch

Clonar um repositório remoto já existente
git clone git@github.com:leocomelli/curso-git.git

_Tags_

Criando uma tag leve
git tag vs-1.1

Criando uma tag anotada
git tag -a vs-1.1 -m "Minha versão 1.1"

Criando uma tag assinada
Para criar uma tag assinada é necessário uma chave privada (GNU Privacy Guard - GPG).
git tag -s vs-1.1 -m "Minha tag assinada 1.1"

Criando tag a partir de um commit (hash)
git tag -a vs-1.2 9fceb02

Criando tags no repositório remoto
git push origin vs-1.2

Criando todas as tags locais no repositório remoto
git push origin --tags

_Branches_

- O master é o branch principal do GIT.

- O HEAD é um ponteiro especial que indica qual é o branch atual. Por padrão, o HEAD aponta para o branch principal, o master.

Criando um novo branch
git branch bug-123

Trocando para um branch existente
git checkout bug-123

- Neste caso, o ponteiro principal HEAD esta apontando para o branch chamado bug-123.

Criar um novo branch e trocar
git checkout -b bug-456

Voltar para o branch principal (master)
git checkout master

Resolver merge entre os branches
git merge bug-123

- Para realizar o merge, é necessário estar no branch que deverá receber as alterações. O merge pode automático ou manual. O merge automático será feito em arquivos textos que não sofreram alterações nas mesmas linhas, já o merge manual será feito em arquivos textos que sofreram alterações nas mesmas linhas.

- A mensagem indicando um merge manual será:

Automerging meu_arquivo.txt
CONFLICT (content): Merge conflict in meu_arquivo.txt
Automatic merge failed; fix conflicts and then commit the result.

Apagando um branch
git branch -d bug-123

Listar branches
git branch

Listar branches com informações dos últimos commits
git branch -v

Listar branches que já foram fundidos (merged) com o master
git branch --merged

Listar branches que não foram fundidos (merged) com o master
git branch --no-merged

Criando um branch remoto com o mesmo nome
git push origin bug-123

Criando um branch remoto com nome diferente
git push origin bug-123:new-branch

Baixar um branch remoto para edição
git checkout -b bug-123 origin/bug-123

Apagar branch remoto
git push origin:bug-123

_Rebasing_

Fazendo o rebase entre um o branch bug-123 e o master.

git checkout experiment

git rebase master

Mais informações e explicações sobre o Rebasing

###Stash

- Para alternar entre um branch e outro é necessário fazer o commit das alterações atuais para depois trocar para um outro branch. Se existir a necessidade de realizar a troca sem fazer o commit é possível criar um stash. O Stash como se fosse um branch temporário que contem apenas as alterações ainda não commitadas.

Criar um stash
git stash

Listar stashes
git stash list

Voltar para o último stash
git stash apply

Voltar para um stash específico
git stash apply stash@{2}

- Onde 2 é o indíce do stash desejado.

Criar um branch a partir de um stash
git stash branch meu_branch

_Reescrevendo o histórico_

Alterando mensagens de commit
git commit --amend -m "Minha nova mensagem"

Alterando os três últimos commits
git rebase -i HEAD~3
- O editor de texto será aberto com as linhas representando os três últimos commits.

pick f7f3f6d changed my name a bit
pick 310154e updated README formatting and added blame
pick a5f4a0d added catfile

- Altere para edit os commits que deseja realizar alterações.

edit f7f3f6d changed my name a bit
pick 310154e updated README formatting and added blame
pick a5f4a0d added catfile

- Feche o editor de texto.

Digite o comando para alterar a mensagem do commit que foi marcado como edit.
git commit –amend -m “Nova mensagem”

Aplique a alteração
git rebase --continue

- Atenção: É possível alterar a ordem dos commits ou remover um commit apenas mudando as linhas ou removendo.

Juntando vários commits
Seguir os mesmos passos acima, porém marcar os commtis que devem ser juntados com *squash

Remover todo histórico de um arquivo
git filter-branch --tree-filter 'rm -f passwords.txt' HEAD

_Bisect_

- O bisect (pesquisa binária) é útil para encontrar um commit que esta gerando um bug ou uma inconsistência entre uma sequência de commits.

Iniciar pequinsa binária
git bisect start

Marcar o commit atual como ruim
git bisect bad

Marcar o commit de uma tag que esta sem o bug/inconsistência
git bisect good vs-1.1

Marcar o commit como bom

- O GIT irá navegar entre os commits para ajudar a indentificar o commit que esta com o problema. Se o commit atual não estiver quebrado, então é necessário marca-lo como bom.
git bisect good

Marcar o commit como ruim

- Se o commit estiver com o problema, então ele deverá ser marcado como ruim.
git bisect bad

Finalizar a pesquisa binária

- Depois de encontrar o commit com problema, para retornar para o HEAD utilize:
git bisect reset

# Links

https://www.uniaogeek.com.br/guia-de-comandos-shell-terminal-gnulinux/
https://gist.github.com/leocomelli/2545add34e4fec21ec16
