## Atalhos globais do Bash

- **Ctrl + Shift + C** - Copiar.
- **Ctrl + Shift + V** - Colar.
- **Ctrl + C** - Cancela o comando atual em funcionamento.
- **Ctrl + Z** - Pausa o comando atual, retorna com "fg" em primeiro plano Linux ou "bg" em segundo plano.
- **Ctrl + D** - Faz o logout da sessão atual (similar ao comando "exit").
- **Ctrl + W** - Apaga uma palavra na linha atual.
- **Ctrl + U** - Apaga a linha inteira.
- **Ctrl + R** - Tecle para Exiber um comando recente.
- **!**! - Repete o último comando.
- **Ctrl + L** - Limpa a tela.

## Diretórios

- **/** - É o diretório raiz, todos os demais diretórios estão abaixo dele.
- **/bin/** - Binários principais dos usuários.
- **/boot/** - Arquivos do sistema de Boot.
- **/dev/** - Arquivos de dispositivos.
- **/etc/** - Arquivos de configuração do sistema.
- **/home/** - Diretório dos usuários comuns do sistema.
- **/lib/** - Bibliotecas essenciais do sistema e os módulos do kernel.
- **/media/** - Diretório de montagem e dispositivos.
- **/mnt/** - Diretório de montagem de dispositivos - mesmo que "media".
- **/opt/** - Instalação de programas não oficiais da distribuição ou por conta do usuário.
- **/sbin/** - Armazena arquivos executáveis que representam comandos administrativos. Exemplo: shutdown
- **/srv/** - Diretório para dados de serviços fornecidos pelo sistema.
- **/tmp/** - Diretório para arquivos temporários.
- **/usr/** - Segunda hierarquia do sistema, onde ficam os usuários comuns do sistema e programas.
- **/var/** - Diretório com arquivos variáveis gerados pelos programas do sistema. Exemplo: logs, spool de impressoras, e-mail e cache.
- **/root/** - Diretório do usuário root - O usuário root tem o total poder sobre o sistema. Podendo instalar, desinstalar e configurar.
- **/proc/** - Diretório virtual controlado pelo Kernel com configuração total do sistema.

## Ajuda

Você pode consultar a documentação e o manual de uso dos comandos das seguintes maneiras:

- **[comando] --help** - Documentação do comando.
- **man [comando]** - Manual do comando.
- **info [comando]** - Semelhante ao man, mas geralmente fornece informações mais detalhadas ou precisas.

## Comando ls

O comando ls é usado para listar o conteúdo de um diretório.

- **ls [opções]**
- **ls** - Lista arquivos e diretórios.
- **ls -r** - Lista arquivos e diretórios em ordem reversa.
- **ls -a** - Lista todos os arquivos e diretórios, incluindo arquivos ocultos.
- **ls -l** - Formato longo, mostra permissões, número de links, propietário, grupo, tamanho, data de modificação e nome do arquivo.
- **ls -h** - Lista arquivos e diretórios com informações formatadas ( Tem que ser usado com o -l ).
- **ls -ls** - Lista arquivos e diretórios pelo tamanho, no caso começará pelo o arquivo de maior tamanho.
- **ls -R** - Lista os arquivos e pastas recursivamente da pasta selecionada.
- **ls -m** - Arquivos listados em sequência, separados por vírgula.
- **ls -n** - Semelhante ao -l, porém mostra UID E GID Em vez de nomes de proprietário e grupo.
- **ls -o** - Semelhante ao -l, porém não mostra o grupo do arquivo.
- **ls -p** - Mostra uma barra ( / ) na frente de nomes de diretórios.
- **ls -A** - Semelhante ao -a, mas não mostra o diretório corrente ( . ) ou o diretório acima ( .. ).
- **ls -i** - Mostra o número do inode de cada arquivo na primeira coluna.

## Comando cd

O comando cd é usado para entrar em uma determinda pasta.

- **cd [destino]**
- **cd .** ou **.** - Diretório atual.
- **cd ..** - Volta um diretório.
- **cd /** - Vai direto para o diretório raiz.
- **cd ~** - Vai direto para o diretório home.
- **cd -** - Nos retorna para o último diretório acessado.
- **cd /diretorio** - Partindo da raiz até o último diretório passado como referência.
- **cd diretorio** - Parte do local corrente até o diretório passado como referência.
