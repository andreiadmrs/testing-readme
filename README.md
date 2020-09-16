## Visualização de arquivos

- **`more [arquivo]`** - Mostra o conteúdo de um arquivo em partes.
- `less [arquivo]` - Exibi o conteúdo de um arquivo páginado.
- `tac [arquivo]` - Exibi o conteúdo de um arquivo de trás pra frente (da última linha pra primeira).
- `cat [opção] [arquivo]`
- `cat` - Abre o arquivo em modo de visualização.
- `cat -E [arquivo]` - Marca o término de linha mostrando o caractere $ ao final de cada uma delas.
- `cat -n [arquivo]` - Mostra a quantidade de linas do arquivo.
- `cat -v [arquivo]` - Exibe caracteres não exibíveis.
- **cat -T [arquivo]** - Exibe tabulação mostradas como ^I.
- **cat -s [arquivo]** - Remove linhas repetidas em branco.
- **cat -b [arquivo]** - Numera as linhas que possuem algum conteúdo.
- **cat [arquivo] | grep [busca]** - Busca no arquivo (case sensitive).
- **cat [arquivo] | grep [busca] -i** - Busca no arquivo (case insensitive).
- **cat [arquivo] > [arquivo]** - Copia o conteúdo do arquivo para outro.
- **cat [arquivo] >> [arquivo]** - Adiciona o conteúdo do arquivo para outro.
