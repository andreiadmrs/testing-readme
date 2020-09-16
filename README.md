## Atalhos globais do Bash

- **`Ctrl + Shift + C`** - Copiar.
- **`Ctrl + Shift + V`** - Colar.
- **`Ctrl + C`** - Cancela o comando atual em funcionamento.
- **`Ctrl + Z`** - Pausa o comando atual, retorna com "fg" em primeiro plano Linux ou "bg" em segundo plano.
- **`Ctrl + D`** - Faz o logout da sessão atual (similar ao comando "exit").
- **`Ctrl + W`** - Apaga uma palavra na linha atual.
- **`Ctrl + U`** - Apaga a linha inteira.
- **`Ctrl + R`** - Tecle para Exiber um comando recente.
- **`!!`** - Repete o último comando.
- **`Ctrl + L`** - Limpa a tela.

## Diretórios

- **`/`** - É o diretório raiz, todos os demais diretórios estão abaixo dele.
- **`/bin/`** - Binários principais dos usuários.
- **`/boot/`** - Arquivos do sistema de Boot.
- **`/dev/`** - Arquivos de dispositivos.
- **`/etc/`** - Arquivos de configuração do sistema.
- **`/home/`** - Diretório dos usuários comuns do sistema.
- **`/lib/`** - Bibliotecas essenciais do sistema e os módulos do kernel.
- **`/media/`** - Diretório de montagem e dispositivos.
- **`/mnt/`** - Diretório de montagem de dispositivos - mesmo que "media".
- **`/opt/`** - Instalação de programas não oficiais da distribuição ou por conta do usuário.
- **`/sbin/`** - Armazena arquivos executáveis que representam comandos administrativos. Exemplo: shutdown
- **`/srv/`** - Diretório para dados de serviços fornecidos pelo sistema.
- **`/tmp/`** - Diretório para arquivos temporários.
- **`/usr/`** - Segunda hierarquia do sistema, onde ficam os usuários comuns do sistema e programas.
- **`/var/`** - Diretório com arquivos variáveis gerados pelos programas do sistema. Exemplo: logs, spool de impressoras, e-mail e cache.
- **`/root/`** - Diretório do usuário root - O usuário root tem o total poder sobre o sistema. Podendo instalar, desinstalar e configurar.
- **`/proc/`** - Diretório virtual controlado pelo Kernel com configuração total do sistema.

## Ajuda

Você pode consultar a documentação e o manual de uso dos comandos das seguintes maneiras:

- **`[comando] --help`** - Documentação do comando.
- **`man [comando]`** - Manual do comando.
- **`info [comando]`** - Semelhante ao man, mas geralmente fornece informações mais detalhadas ou precisas.

## Comando ls

O comando ls é usado para listar o conteúdo de um diretório.

- **`ls [opções]`**
- **`ls`** - Lista arquivos e diretórios.
- **`ls -r`** - Lista arquivos e diretórios em ordem reversa.
- **`ls -a`** - Lista todos os arquivos e diretórios, incluindo arquivos ocultos.
- **`ls -l`** - Formato longo, mostra permissões, número de links, propietário, grupo, tamanho, data de modificação e nome do arquivo.
- **`ls -h`** - Lista arquivos e diretórios com informações formatadas ( Tem que ser usado com o -l ).
- **`ls -ls`** - Lista arquivos e diretórios pelo tamanho, no caso começará pelo o arquivo de maior tamanho.
- **`ls -R`** - Lista os arquivos e pastas recursivamente da pasta selecionada.
- **`ls -m`** - Arquivos listados em sequência, separados por vírgula.
- **`ls -n`** - Semelhante ao -l, porém mostra UID E GID Em vez de nomes de proprietário e grupo.
- **`ls -o`** - Semelhante ao -l, porém não mostra o grupo do arquivo.
- **`ls -p`** - Mostra uma barra ( / ) na frente de nomes de diretórios.
- **`ls -A`** - Semelhante ao -a, mas não mostra o diretório corrente ( . ) ou o diretório acima ( .. ).
- **`ls -i`** - Mostra o número do inode de cada arquivo na primeira coluna.

## Comando cd

O comando cd é usado para entrar em uma determinda pasta.

- **`cd [destino]`**
- **`cd .`** ou **`.`** - Diretório atual.
- **`cd ..`** - Volta um diretório.
- **`cd /`** - Vai direto para o diretório raiz.
- **`cd ~`** - Vai direto para o diretório home.
- **`cd -`** - Nos retorna para o último diretório acessado.
- **`cd /diretorio`** - Partindo da raiz até o último diretório passado como referência.
- **`cd diretorio`** - Parte do local corrente até o diretório passado como referência.

## Comando pwd

- **`pwd`** - Exibe o caminho de diretório atual.

## Comando mkdir

O comando mkdir é usado para criar pastas

- **`mkdir [nomeDaPasta]`** - Cria uma pasta.
- **`mkdir pasta1 pasta2 pasta3`** - Cria três pastas, pasta1, pasta2 e pasta3.
- **`mkdir -p A/B/C`** - Cria a pasta A, dentro da pasta A cria a pasta B e dentro da pasta B cria a pasta C.

## Comando du

- **`du`** - Exibe o tamanho de um diretório e todos os seus subdiretórios.

## Comando touch

O comando touch é usado para criar arquivos.

- **`touch [opções] [arquivo]`**
- **`touch [arquivo]`** - Cria uma arquivo.
- **`touch -a [arquivo]`** - Altera a hora de acesso do arquivo.
- **`touch -m [arquivo]`** - Altera a hora de modificação do arquivo.
- **`touch -am [arquivo]`** - Altera a hora de acesso e modificação do arquivo.
- **`touch -c [arquivo]`** - Altera a hora de acesso sem criar um novo arquivo.

**`Observação`**: podemos gerar nomes automáticos usando as chaves {} desta maneira: touch exemplo{1..3}.txt, este comando irá criar 3 arquivos chamados exemplo1.txt, exemplo2.txt e exemplo3.txt.

## Comando rm

O comando rm é usado para excluir arquivos.

- **`rm [opções] [arquivo]`**
- **`rm`** - Exclui um arquivo.
- **`rm -f`** - Exclui arquivos forçadamente.
- **`rm -r`** - Exclui o diretório e os arquivos na direção recursiva, o diretório especificado junto com seu subdiretório e arquivos.
- **`rm -d`** - Remove somente diretórios vazios.
- **`rm -i`** - Pergunta se queremos remover o arquivo/diretório antes de excluir.
- **`rm -rf`** - (rm -r) + (rm -f) ( utilize esse comando com extrema atenção! ).

## Comando cp

O comando cp é usado para copiar arquivos.

- **`cp [opções] [arquivo] [destino]`**
- **`cp -i [arquivo] [destino]`** - Pergunta se desejamos sobrescrever um arquivo destino já existente.
- **`cp -n [arquivo] [destino]`** - Não sobrescreve um arquivo já existente.
- **`cp -r [arquivo] [destino]`** - Copia diretórios de forma recursiva.
- **`cp -p [arquivo] [destino]`** - Preserva as permissões originais do arquivo (proprietário, grupo, etc.).
- **`cp -vr [origem] [destino]`** - copiar diretorio recursivamente.

## Comando mv

O comando mv é usado para mover arquivos.

- **`mv [opções] [arquivo] [destino]`**
- **`mv -b [arquivo] [destino]`** - Cria um backup de cada arquivo destino existente.
- **`mv -f [arquivo] [destino]`** - Apaga destinos existente sem perguntar ao usuário.
- **`mv -i [arquivo] [destino]`** - Pergunta se desejamos sobrescrever o arquivo destino já existente.
- **`mv -n [arquivo] [destino]`** - Não sobrescrever um arquivo destino já existente.

O comando mv também é usado para renomear arquivos.

- **`mv [nomeAtual.extenção] [novoNome.extenção]`**

## Visualização de arquivos

- **`more [arquivo]`** - Mostra o conteúdo de um arquivo em partes.
- **`less [arquivo]`** - Exibi o conteúdo de um arquivo páginado.
- **`tac [arquivo]`** - Exibi o conteúdo de um arquivo de trás pra frente (da última linha pra primeira).
- **`cat [opção] [arquivo]`**
- **`cat`** - Abre o arquivo em modo de visualização.
- **`cat -E [arquivo]`** - Marca o término de linha mostrando o caractere $ ao final de cada uma delas.
- **`cat -n [arquivo]`** - Mostra a quantidade de linas do arquivo.
- **`cat -v [arquivo]`** - Exibe caracteres não exibíveis.
- **`cat -T [arquivo]`** - Exibe tabulação mostradas como ^I.
- **`cat -s [arquivo]`** - Remove linhas repetidas em branco.
- **`cat -b [arquivo]`** - Numera as linhas que possuem algum conteúdo.
- **`cat [arquivo] | grep [busca]`** - Busca no arquivo (case sensitive).
- **`cat [arquivo] | grep [busca] -i`** - Busca no arquivo (case insensitive).
- **`cat [arquivo] > [arquivo]`** - Copia o conteúdo do arquivo para outro.
- **`cat [arquivo] >> [arquivo]`** - Adiciona o conteúdo do arquivo para outro.

## Comando bc

- **`bc`** - Abre uma calculadora do Bash

**Observação**: Para sair bastas digitar 'quit' e dar enter.
