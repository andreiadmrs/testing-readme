## O que é o Bash?

Segundo o wikipedia, o que seria o bash:

> "Acrônimo para "Bourne-Again SHell", o Bash é uma evolução retro-compatível muito mais interativa do Bourne Shell (sh). Os shells Bourne permitem a execução de sequências de comandos inseridos diretamente na linha de comandos ("prompt") ou ainda lidos de arquivos de texto conhecidos como shell scripts. Neles se podem invocar comandos internos aos próprios shells (conhecidos como comandos "builtins") ou ainda arquivos binários ou scripts de terceiros arquivados nos dispositivos de armazenamento do sistema."

Para mais detalher clique [aqui](https://pt.wikipedia.org/wiki/Bash).

Simplificando, Bash é uma linha de comando, e uma linha de comando é uma forma diferente de se usar um sistema operacional, uma forma sem interface gráfica.

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

## Processos

- **`top`** - Exibe os processos usando a maioria dos recursos do sistema, a qualquer momento. "Q" pode ser usado para sair.
- **`htop`** - O comando HTOP é uma evolução do comando TOP. As informações são semelhantes às produzidas pelo comando TOP, mas apresentadas num interface mais intuitivo e colorido.
- **`kill pid`** - Mata o processo com o id de processo pid.
- **`killall Discord`** - Mata todos os processo com o nome discord.
- **`pkill fire`** - Mata todos os processo que tenha "fire" em seu nome.
- **`ps [opções]`**
- **`ps`** - O comando ps exibe informações sobre os processos que estão executando na máquina.
- **`ps -a`** - Mostra os processos de todos os usuários.
- **`ps -A`** ou **`ps -e`** - Mostra todos os processos.
- **`ps -f`** - Mostra a árvore de execução de comandos.
- **`ps -g [grupo]`** - Mostra os processos de um determinado grupo.
- **`ps -x`** - Mostra os processos que não foram iniciados no console.
- **`ps -u`** - Fornece o nome do usuário e a hora de início do processo.
- **`ps -aux`** - exibe todos os processos do sistema independente de terminal.

## Informações do sistema

- **`whereis [programa]`** - Exibe possíveis localizações de um determinado programa.
- **`date`** - Exibe a data e hora atual.
- **`whoami`** - Imprime o nome de usuário usado no momento em que foi digitado.
- **`sudo su`** - Entra no modo usuário root.
- **`exit`** - Sai do usuário logado no momento que o comando é executado.

**Observação**: Quando você for digitar sua senha para entrar no modo usuário root, por questões de segurança o terminal não exibe nada na tela o que foi digitado.

- **`uname [opções]`**
- **`uname -a ou uname`** --all imprime todas as informações, omitindo uname -p e uname -i se as informações forem desconhecidas.
- **`uname -s ou uname`** --kernel-name - Imprime o nome do kernel.
- **`uname -n ou uname`** --nodename - Imprime o nome do host do nó da rede.
- **`uname -r ou uname`** --kernel-release - Imprime a versão do kernel.
- **`uname -v ou uname`** --kernel-version - Imprime a versão do kernel.
- **`uname -m ou uname`** --machine - Imprime o nome do hardware da máquina.
- **`uname -p ou uname`** --processor - Imprime o tipo de processador ou ” desconhecido “.
- **`uname -i ou uname`** --hardware-platform - Imprime a plataforma de hardware, ou ” desconhecido “.
- **`uname -o ou uname`** --operating-system - Imprime o sistema operacional.
- **`uname --version`** - Exibe informações da versão.

## Memória

- **`free`** - Este comando exibe a quantidade de espaço livre disponível no sistema.
- **`df [opções]`**
- **`df`** - Exibe informações sobre o uso do espaço em disco de todos os sistemas de arquivos montados.
- **`df -a`** - Inclui sistema de arquivos com 0 (zero) blocos.
- **`df -h`** - Mostra o espaço livre/ocupado em MB, KB, GB em vez de bloco.
- **`df -k`** - Lista em Kbyts.
- **`df -l`** - Somente lista sistema de arquivos locais.
- **`df -m`** - Lista em Mbytes.
- **`df -T`** - Lista o tipo de sistema de arquivos de cada partição.

## Comando apt

- **`sudo apt-get update`** - Baixa os pacotes disponíveis.
- **`sudo apt-get upgrade`** - Atualiza os pacotes do sistema.
- **`sudo apt-get clean`** - Remove cache de programas.
- **`sudo apt-get cache [busca]`** - Busca um programa.
- **`sudo apt-get install [programa]`** - Instala um programa.
- **`sudo apt-get remove [pacote] --purge`** - Remove programas e configs.

**Observação**: Se você estiver logado como usuário root, não é necessário o uso do 'sudo' na frente dos comandos.

## Compressão de arquivos

- **`tar cf pacote.tar arqs`** - Cria um pacote TAR (nomeado pacote.tar) com os arquivos especificados (substituir a variável arqs pelo nome do arquivo).
- **`tar xf pacote.tar`** - Extrai os arquivos de “pacote.tar” (substituir a variável pacote.tar pelo nome do arquivo).
- **`tar czf pacote.tar.gz arqs`** - Cria um pacote TAR (nomeado pacote.tar.gz) com compressão GZip.
- **`tar xzf pacote.tar.gz`** - Extrai um pacote TAR (nomeado pacote.tar.gz) com compressão GZip.
- **`tar cjf pacote.tar.bz2`** - Cria um pacote TAR (nomeado pacote.tar.bz2) com compressão BZip2.
- **`tar xjf pacote.tar.bz2`** - Extrai um pacote TAR (nomeado pacote.tar.gz) com compressão BZip2.
- **`gzip arq`** - Compacta um arquivo e o renomeia para arq.gz (substituir a variável arq pelo nome do arquivo).
- **`gzip -d arq.gz`** - Descompacta arq.gz para um arquivo (substituir a variável arq.gz pelo nome do arquivo).

## Histórico de comandos

- **`history`** - Lista o histórico de 2000 comandos digitados.
- **`Seta para cima e seta para baixo`** - Últimos comandos digitados.

## Referência global

Referências globais são recursos para especificar um ou mais arquivos ou diretórios de uma vez. Vamos usar o comando 'ls' para os exemplos, mas pode ser usado qualquer outro comando.

- **`ls /etc/*.conf`** - Lista todos os arquivos que tem a extenção '.conf'.
- **`ls /etc/*x*`** - Lista todos os aquivos que em algum lugar do nome tem a lera 'x'.
- **`ls /etc/f*`** - Lista todos os aquivos que começa com a letra 'f'.
- **`ls /etc/?as*`** - Lista todos os arquivos que começa com uma letra qualquer, tem segundo caractere 'a', o terceiro 's' e qualquer caractere depois.
- **`ls /etc/???a*`** - Lista todos os arquivos que tem o quarto caractere 'a'.
- **`ls /etc/f[a-t]*`** - Lista todos os aqruivos que começa com a letra 'f', depois a segunda letra varia do 'a' ao 't' e depois qualquer caractere.
- **`ls /etc/f[u,o]*`** - Lista todos os aqruivos que começa com a letra 'f', depois a segunda letra é 'u' ou 'o' e depois qualquer caractere.
- **`ls /etc/?[a,e,i,o,u]*`** - Lista todos os aqruivos que começa com uma letra qualquer, depois a segunda letra é uma vogal e depois qualquer caractere.
- **`ls /etc/?[a,e,i,o,u]???`** - Lista todos os aqruivos que começa com uma letra qualquer, depois a segunda letra é uma vogal e depois tem mais 3 caracteres qualquer.
- **`ls /etc/?{am,ul}*`** - Lista todos os aqruivos que começa com uma letra qualquer, depois a segunda e a terceira letra é 'am' ou 'ul' e depois qualquer caractere.
- **`ls /etc/*{ev,ux}`** - Lista todos os aqruivos que termina com 'ev' ou 'ux'.
- **`ls /etc/*.{conf,db}`** - Lista todos os aqruivos que tem a extenção '.conf' ou '.db'.

## Comando find

O comando find é usado para busca de arquivos.

- **`find .`** - Lista todos os arquivos contidos em um diretório e subdiretórios.
- **`find . -name [arquivo]`** - Busca um arquivo com um nome especifico.
- **`find [diretório] -iname [arquivo]`** - Procura ignorando case sensitive.

## Usuários

## Comando passwd

O passwd é um comando utilizado para configurar ou trocar a senha das contas dos usuários do sistema. É necessário possuir privilégios administrativos para executá-lo, mas um usuário comum consegue alterar sua própria senha.

- **`passwd [opções] [usuários]`**
- **`passwd -l`** - Trava a senha do usuário, ficando impedido de se logar e não pode trocar a senha (não é desabilitado).
- **`passwd -u`** - Destrava a senha do usuário.
- **`passwd -d`** - Exclui a senha do usuário.
- **`passwd -e`** - Expira a senha do usuário, forçando-o a fornecer uma nova ao logar-se novamente.
- **`passwd -x dias`** - Expira a senha do usuário quando atingir o número de dias especificados.
- **`passwd -n dias`** - Define a quantidade mínima de dias que o usuário deverá esperar para trocar a senha.
- **`passwd -w dias`** - define a quantidade mínima de dias que o usuário receberá o aviso que a senha precisa ser alterada.
- **`passwd -i`** - Deixa o usuário inativo, caso a senha tenha expirado.
- **`passwd -S`** - Exibe o status da conta.
- **`passwd -a`** - Usada em conjunto com a opção -S mostra o status das contas de todos os usuários.

## Tipos de usuários

## Usuários comuns

São os usuários que podem se conectar no sistema. Geralmente, estes usuários possuem uma home e podem manipular arquivos quando tem as permissões para tal. Porém estes usuários geralmente não tem permissão para certos arquivos e diretórios na maquina e não podem executar muitas funções a nível de sistema.

Exemplo de um usuário comum: **`roger@AB4NT5S:~$`**

## Usuários de sistema

Diferente dos usuários comuns, estes usuários não se conectam no sistema. São contas usadas para tarefas específicas dentro do sistema que não são de propriedade de uma pessoa em particular.

## Root

O usuário root, também chamado de superusuário, tem controle total sobre o sistema operacional. Ele pode acessar todos os arquivos e normalmente é o único que pode executar certos programas, como por exemplo o httpd.

Exemplo de um usuário root: **`root@AB4NT5S:~#`**

**Observação**: Não é recomendado que você use o terminal no modo root o tempo inteiro.

## Grupos

Um grupo é um conjunto de um ou mais usuários. É interessante reunir vários usuários em um grupo para definir suas propriedades, como as permissões. Como o arquivo passwd nós temos um arquivo somente para armazenar detalhes sobre os grupos.
Esse arquivo esta localizado em: /etc/group.

## Gerenciamento de usuários

## Adicionar usuários

Criar um usuário novo no Linux é bem simples, apenas é necessário o comando useradd e indicar o nome do novo usuário.

- **`useradd [opções] [nomeusuario]`**
- **`useradd -d [nomeusuario]`** - Define o nome do diretório home do usuário (mas não o cria).
- **`useradd -s [nomeusuario]`** - Define o shell padrão do usuário.
- **`useradd -h [nomeusuario]`** - Exibe as opções do comando.

## Alterar usuários

Para alterarmos uma conta de usuário basta apenas utilizarmos o comando usermod.

- **`usermod [opções] [nomeusuário]`**
- **`usermod -d diretório [-m]`** - Cria uma nova home para o usuário. A opção -m move os arquivos da home atual do usuário para a nova.
- **`usermod -e yyyy-mm-dd`** - Altera a data de expiração da conta do usuário.
- **`usermod -g grupo`** - Altera o GID do grupo do usuário para o especificado.
- **`usermod -G grupo[, grupo2, ...]`** - Define o GID dos outros grupos que o usuário pertence.
- **`usermod -l nome`** - Altera o nome do usuário (ele não pode estar logado).
- **`usermod -s shell`** - Altera o shell do usuário.
- **`usermod -u uid`** - Altera o número de UID do usuário.

## Remover usuários

Para removermos um usuário utilizamos o comando userdel.

- **`userdel [opções] [nomeusuario]`**
- **`userdel -h [nomeusuario]`** - Exibe as opções do comando.
- **`userdel -r [nomeusuario]`** - Deleta a home e todos os seus arquivos.

## vim

Eu escolhi o editor vim para este artigo, mas você pode usar vários editores além do vim como o nano e o vi por exemplo.

O vim (VI Improvement) é uma melhoria do antigo editor de texto vi. Este por sua vez é uma melhoria do editor de texto orientado a linha chamado ed. Existe também uma versão do vim para ambiente X chamada gvim.

O vim possui três formas de trabalho: modo de linha, modo de edição e modo de comandos. A mudança de um modo para outro modo é feita através do uso da tecla Esc.

Após o arquivo ser aberto pelo vim, o modo de comandos é ativado. No modo de comandos, as teclas digitadas pelo usuário são interpretadas pelo vim como ações a serem executadas dentro do arquivo aberto. No modo de edição, as teclas digitadas pelo usuário são ecoadas na tela. Para entrar neste modo, pode-se digitar, por exemplo, "a" (adicionar), "i" (incluir), etc. No modo de linha, o usuário define ações a serem executadas no arquivo como um todo (por exemplo, salvar, substituir caracteres, sair do aplicativo, etc). Para entrar neste modo, deve-se digitar " : ".

- **`vim [opções] [arquivo]`**

São alguns dos comandos do vim no modo de comandos

- **`0`** - Mover o cursor para o início da linha em que o cursor está posicionado.
- **`a`** - Inserir texto após a posição atual do cursor.
- **`A`** - Inserir texto no final da linha atual.
- **`-b`** - Permite editar arquivo binário.
- **`dd`** - Deletar linha atual.
- **`[n]+dd`** - Deletar n linhas a partir da linha atual.
- **`G`** - Ir para o fim do arquivo.
- **`[n]+G`** - Ir para a n-ésima linha do arquivo.
- **`h`** - Voltar um caractere.
- **`H`** - Ir para a primeira linha exibida na tela atual.
- **`i`** - Inserir texto a partir da posição atual do cursor.
- **`I`** - Inserir texto no início da linha atual.
- **`j`** - Descer uma linha.
- **`J`** - Juntar a linha atual com a linha seguinte.
- **`[n]+J`** - Juntar n linhas consecutivas a partir da linha atual.
- **`k`** - Subir uma linha.
- **`l`** - Avançar um caractere.
- **`L`** - Ir para a última linha exibida na tela atual.
- **`n`** - Procurar, a partir da posição atual do cursor, a próxima ocorrência do texto definido no último comando /.
- **`N`** - Procurar, a partir da posição atual do cursor e indo em direção ao início do arquivo, a próxima ocorrência do texto definido no último comando /.
- **`o`** - Inserir uma linha em branco após a linha atual.
- **`O`** - Inserir uma linha em branco acima da linha atual.
- **`p`** - Inserir linhas copiadas após a linha atual.
- **`P`** - Inserir linhas copiadas antes da linha atual.
- **`r`** - Substituir o caractere atual.
- **`R`** - Substituir um conjunto de caracteres.
- **`s`** - Deletar o caractere atual e inserir texto.
- **`S`** - Apagar linha e inserir novo texto na linha.
- **`u`** - Desfazer a última alteração feita no texto e ainda não desfeita.
- **`U`** - Desfazer a última alteração feita no texto.
- **`x`** - Apagar caractere onde o cursor está posicionado.
- **`$`** - Mover o cursor para o fim da linha em que o cursor está posicionado.
- **`[n]+y`** - Copiar n linhas a partir da linha atual.
- **`yy`** - Copiar a linha atual.
- **`[n]+Y`** - Copiar n linhas a partir da linha atual.
- **`YY`** - Copiar a linha atual.
- **`CTRL+B`** - Voltar uma página.
- **`CTRL+F`** - Avançar uma página.
- **`F1`** - Exibir tela de ajuda.
- **`[n]+ENTER`** - Ir para n linhas abaixo da linha atual.
- **`[n]+.`** - Repetir o último comando que alterou o texto n vezes a partir da posição atual do cursor.
- **`[n]+~+ENTER`** - Inverter a caixa (case) dos n caracteres seguintes ao cursor.
- **`/texto`** - Procurar pela primeira ocorrência do texto especificado a partir da posição atual do cursor.

São alguns dos comandos do vim no modo de linha

- **`:r arquivo`** - Incluir arquivo a partir da linha atual do cursor.
- **`:q+ENTER`** - Sair da tela de ajuda.
- **`:q!`** - Sair do vim sem salvar as alterações.
- **`:w arquivo`** - Salvar arquivo com o nome especificado.
- **`:wq`** - Sair do vim salvando as alterações.
- **`:X`** - Criptografa o arquivo.
- **`:n`** - Ir para a linha "n". Exemplo: Para ir para linha 10 do arquivo, :1

Busca

- **`/palavra`** - Procura por "palavra" do início para o fim.
- **`?palavra`** - Procura por "palavra" do fim para o início.
- **`/Mari[oa]`** - Procura por "Mario" ou "Maria".
- **`/\< pal`** - Procura por expressões que começem com "pala" como, "palavra" ou "palíndromo".
- **`/ismo\>`** - Procura por expressões que terminem com "ismo" como, "autismo".
- **`/\< para\>`** - Procura pela palavra "para".
- **`/\<...\>`** - Procura por todas as palavras com 3 letras.
- **`/maria\|joao`** - Procura por maria ou joao.
- **`/\<\d\d\d\d\>`** - Procura exatamente por 4 dígitos numéricos.
- **`/^\n\{3}`** - Procura por três linhas em branco.
- **`:bufdo /palavra/`** - Procura "palavra" em todos os arquivos abertos.

Substituição

- **`:%s/antigo/novo/g`** - Substitui todas as ocorrências de "antigo" por "novo" no arquivo.
- **`:%s/antigo/novo/gw`** - Substitui todas as ocorrências com confirmação.
- **`:2,35s/antigo/novo/g`** - Substitui todas as ocorrências entre as linhas 2 e 35.
- **`:5,$s/antigo/novo/g`** - Substitui todas as ocorrências da linha 5 até EOF (fim da linha).
- **`:%s/^/legal/g`** - Substitui o começo de cada linha com "legal".
- **`:%s/$/Oh/g`** - Substitui o fim de cada linha por "Oh".
- **`:%s/antigo/novo/gi`** - Substitui "antigo" por "novo" desconsiderando maíusculas e/ou minúsculas.
- **`:%s/ *$//g`** - Apaga todos os espaços em branco.
- **`:g/palavra/d`** - Apaga todas as linhas contendo "palavra".
- **`:v/palavra/d`** - Apaga todas as linhas que não contém "palavra".
- **`:s/maria/joao/`** - Substitui a primeira ocorrência de "maria" por "joao" na linha corrente.
- **`:s/maria/joao/g`** - Substitui todas as ocorrências de "maria" por "joao" na linha corrente.
- **`:%s/maria/joao/g`** - Substitui "maria" por "joao" em todo o arquivo.
- **`:%s/\r//g`** - Apaga retornos de carro do windows (\n).
- **`:%s/\r/\r/g`** - Transforma os retornos de carro do windows (\n) em retornos do Linux (\r).
- **`:%s#<[^>]\+>##g`** - Apaga tags HTML mas mantêm o texto.
- **`:%s/^\(.*\)\n\1$/\1/`** - Apaga linhas repetidas.
- **`Ctrl+a`** - Incrementa o número sob o cursor.
- **`Ctrl+x`** - Decrementa o número sob o cursor.
- **`ggVGg?`** - Muda o texto usando Rot13.

Minúsculo / Maiúsculo

- **`Vu`** - Torna todos os caracteres da linha minúsculos.
- **`VU`** - Torna todos os caracteres da linha maiúsculos.
- **`g~~`** - Inverte os caracteres do texto inteiro.
- **`vEU`** - Coloca as letras da palavra em maiúsculas.
- **`vE~~`** - Inverte os caracteres da palavra selecionada.
- **`ggguG`** - Coloca todo o texto em minúsculas.
- **`:set ignorecase`** - Ignora minúsculos/maiúsculos nas buscas.
- **`:set smartcase`** - Ignora minúsculos/maiúsculos em buscas exceto quando uma letra msiúscula é usada.
- **`:%s/\<./\u&/g`** - Coloca a primeira letra de cada palavra em maiúscula.
- **`:%s/\<./\l&/g`** - Coloca a primeira letra de cada palavra em minúscula.
- **`:%s/.*/\u&`** - Coloca a primeira letra de cada linha em maiúscula.
- **`:%s/.*/\l&`** - Coloca a primeira letra de cada linha em minúscula.

Lendo/Gravando arquivos

- **`:1,10 w arquivo`** - Salva as linhas de 1 a 10 em "arquivo".
- **`:1,10 w >> arquivo`** - Adiciona as linhas de 1 a 10 em "Arquivo".
- **`:r arquivo`** - Insere o conteúdo de "arquivo" no atual.
- **`:23r arquivo`** - Insere o conteúdo de "arquivo" a partir da linha 23.

Explorando arquivos

- **`:e .`** - Abre o gerenciador de arquivos integrado do Vim.
- **`:Sex`** - Divide a janela e abre o gerenciador de arquivos integrado.
- **`:browse e`** - Abre o gerenciador de arquivos integrado na janela corrente.
- **`:ls`** - Lista os buffers carregados.
- **`:cd ..`** - Move para a pasta superior.
- **`:args`** - Lista os arquivos.
- **`:args *.php`** - Abre lista de arquivos.
- **`:grep expressao *.php`** - retorna uma lista de arquivos .php que contenham a expressão informada.
- **`gf`** - Abre o arquivo sob o cursor.

Interação com o Linux

- **`:!pwd`** - Executa o comando "pwd" e retorna para o Vim.
- **`!!pwd`** - Executa o comando "pwd" e insere a saída no buffer.
- **`:sh`** - Retorna temporariamente para o shell.
- **`exit`** - Retorna para o Vim.

Alinhamento

- **`:%!fmt`** - Alinha todas as linhas.
- **`!}fmt`** - Alinha todas as linhas a partir da posição corrente.
- **`5!!fmt`** - Alinha as próximas 5 linhas.

Abas

- **`:tabnew`** - Cria uma nova aba.
- **`gt`** - Mostra a próxima aba.
- **`:tabfirst`** - Mostra a primeira aba.
- **`:tablast`** - Mostra a última aba.
- **`:tabm n(posicao)`** - Reorganiza as abas.
- **`:tabdo %s/foo/bar/g`** - Executa um comando em todas as abas.
- **`:tab ball`** - Coloca todos os arquivos abertos em abas.

Divisão da janela do Vim

- **`:e arquivo`** - Edita "arquivo" na janela corrente.
- **`:split arquivo`** - Divide a janela e abre "arquivo".
- **`ctrl-w "seta para cima"`** - Coloca o cursor na janela do topo.
- **`ctrl-w ctrl-w`** - Coloca o cursor na próxima janela.
- **`ctrl-w_`** - Maximiza a janela corrente.
- **`ctrl-w=`** - Coloca todas as janelas com o mesmo tamanho.
- **`10 ctrl-w+`** - Adiciona 10 linhas de tamanho na janela corrente.
- **`:vsplit arquivo`** - Divide a janela verticalmente.
- **`:sview arquivo`** - O mesmo que split, mas em modo somente-leitura.
- **`:hide`** - Fecha a janela corrente.
- **`:only`** - Fecha todas as janelas, exceto a janela atual.
- **`:b 2`** - Abre #2 na janela corrente.

Auto-completion do texto

- **`Ctrl+n Ctrl+p (em modo de inserção)`** - Completa palavra.
- **`Ctrl+x Ctrl+l`** - Completa linha.
- **`:set dictionary=dict`** - Define dict como o dicionário atual.
- **`Ctrl+x Ctrl+k`** - Completa usando o dicionário.

Marcações

- **`mk`** - Marca a posição corrente como k.
- **`‘k`** - Move o cursor para a marca k.
- **`d’k`** - Apaga tudo até a marca k.

Abreviações

- **`:ab email me@me.com`** - Define email como abreviação de me@me.com.

Identação de Texto

- **`:set autoindent`** - Liga a identação automática.
- **`:set smartindent`** - Liga a identação inteligente.
- **`:set shiftwidth=4`** - Define o tamanho da identação em 4 espaços.
- **`ctrl-t, ctrl-d`** - Identa/Deidenta no modo de inserção.
- **`>>`** - Identa.
- **`<<`** - Deidenta.

Marcação de sintaxe

- **`:syntax on`** - Liga a marcação de sintaxe.
- **`:syntax off`** - Desliga a marcação de sintaxe.
- **`:set syntax=perl`** - Força a usar a marcação de sintaxe do perl.
