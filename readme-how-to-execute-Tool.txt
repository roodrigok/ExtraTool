Configura��es:
A janela de linha de comando (cmd) deve estar dentro da pasta do .jar execut�vel.

O comando necess�rio para executar o .jar �:
java -jar Tool.jar [par�metro1] [par�metro2] ... [par�metroN1] [par�metroN2]

Para uma execu��o correta � necess�rio seguir a seguinte ordem:
1 - O primeiro par�metro � o nome da aplica��o a ser processada.
2 - O segundo par�metro � o caminho (path) da pasta res da aplica��o.
3 - � poss�vel passar N projetos em uma execu��o, desde que mantenha em mente as ordens 
do par�metros especificados nos itens 1 e 2.

Exemplo:

java -jar Tool.jar "dmix" "C:\\Projetos\\dmix-master\\MPDroid\\src\\main\\res" "aarddict" "C:Projetos\aarddict\res"

Isto nos retorna os dados dos projetos "dmix" e "aarddict" na planilha gerada como sa�da.

-------------------------------------------------------------------------------------------

Uma segunda forma de execut�-lo, � passando por par�metro um arquivo .txt, segue o exemplo.

Para uma execu��o correta � necess�rio seguir a seguinte ordem:
1. O projetos.txt deve estar na pasta do .jar execut�vel.
2. A cada linha deve conter apenas um projeto com o nome e o caminho do projeto.
3. O nome e o caminho do projeto devem necessariamente estarem separados apenas pelo caractere ;.

No projetos.txt as informa��es devem estar organizadas da seguinte maneira:
dmix;C:\\Projetos\\dmix-master\\MPDroid\\src\\main\\res
aarddict;C:\\Projetos\aarddict\res
... e assim por diante.

O comando necess�rio para executar o .jar �:
java -jar Tool.jar projetos.txt

Isto nos retorna os dados dos projetos "dmix" e "aarddict" na planilha gerada como sa�da.