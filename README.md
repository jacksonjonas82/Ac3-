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

Explanação: Para definir permissões, somam-se os valores acima. Por exemplo, para atribuir ao dono do arquivo (“usuário) acesso total de leitura (r), gravação (w) e execução (x), basta somar o valor octal 4 + 2 + 1 = 7. Supondo que você queira limitar o acesso para membros do “grupo”, permitindo apenas a leitura e gravação, basta somar 4 + 2 = 6. Reunindo os dois exemplos citados, ficaria: chmod 760 (r para usuário, w para grupo e 0 para outros ou “rw-“)

_Outros exemplos_

1. chmod 777: leitura (r), gravação (w) e execução (x) para todos (“usuário”, “grupo” e “outros”)



# Links

https://www.uniaogeek.com.br/guia-de-comandos-shell-terminal-gnulinux/
