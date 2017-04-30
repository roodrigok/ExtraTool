Configurações:
A janela de linha de comando (cmd) deve estar dentro da pasta do .jar executável.

O comando necessário para executar o .jar é:
java -jar Tool.jar [parâmetro1] [parâmetro2] ... [parâmetroN1] [parâmetroN2]

Para uma execução correta é necessário seguir a seguinte ordem:
1 - O primeiro parâmetro é o nome da aplicação a ser processada.
2 - O segundo parâmetro é o caminho (path) da pasta res da aplicação.
3 - É possível passar N projetos em uma execução, desde que mantenha em mente as ordens 
do parâmetros especificados nos itens 1 e 2.

Exemplo:

java -jar Tool.jar "dmix" "C:\\Projetos\\dmix-master\\MPDroid\\src\\main\\res" "aarddict" "C:Projetos\aarddict\res"

Isto nos retorna os dados dos projetos "dmix" e "aarddict" na planilha gerada como saída.

-------------------------------------------------------------------------------------------

Uma segunda forma de executá-lo, é passando por parâmetro um arquivo .txt, segue o exemplo.

Para uma execução correta é necessário seguir a seguinte ordem:
1. O projetos.txt deve estar na pasta do .jar executável.
2. A cada linha deve conter apenas um projeto com o nome e o caminho do projeto.
3. O nome e o caminho do projeto devem necessariamente estarem separados apenas pelo caractere ;.

No projetos.txt as informações devem estar organizadas da seguinte maneira:
dmix;C:\\Projetos\\dmix-master\\MPDroid\\src\\main\\res
aarddict;C:\\Projetos\aarddict\res
... e assim por diante.

O comando necessário para executar o .jar é:
java -jar Tool.jar projetos.txt

Isto nos retorna os dados dos projetos "dmix" e "aarddict" na planilha gerada como saída.