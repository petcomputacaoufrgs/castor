# Linguagem: C++

## Explicação:

Pasta para codigos e exemplos da linguagem de programação C++. Dentro dela, você encontrará  subpastas chamadas: *codigos*, na qual você deverá armazenar seus codigos; *exemplos*, onde estão disponiveis diversos exemplos de como funciona a linguagem, os quais tambem podem ser utilizado para testar se os métodos de criação de arquivos executaveis está funcionando; *.vscode*, na qual está armazenado os arquivos que o programa Visual Studio Code utiliza para configurar o projeto corretamente.

## Como usar:

Caso esteja utilizando a IDE chamada Visual Studio Code, simplesmente abra esta pasta chamada ***CPP*** no programa e comece a programar! Quando necessitar compilar e testar seu programa, na parte esquerda, vá na aba de *Run and Debug* (acessivel tambem pela combinação Ctrl+Shift+D) e selecione o tipo de tarefa que quer executar¹ e clique no botão verde. Nas vezes subsequentes, basta estar com o arquivo aberto e apertar *F5* que a tarefa deve executar automaticamente.

¹ O grupo PET Computação já deixou uma prépronta que deve funcionar na maioria dos casos.

## Cadeiras Aplicaveis:

* Classificação e Pesquisa de Dados - INF01124

## Como Modififcar:

Para modificar a maneira na qual o programa VSCode realiza o processo de compilação e debbug do seu codigo é necessario modificar os conteudos da pasta .vscode. Lá dentro, estão 4  arquivos que modificam as propriedades da area de trabalho atual.

* *extensions.json:* armazena as extensões recomendadas;
* *settings.json:* armazena configurações especificas para esta pasta;
* *launch.json:* armazena o os processos que devem ser executados na aba de *Run and Debug*, para executar o processo de depuração com argumentos de linha de comando, basta adiciona-los ao item `"args"` do arquivo;
* *tasks.json:* armazena os processos de prédepuração, normalmente executa a compilação dos arquivos para serem executados.

## Links de referencia:

* [https://cplusplus.com/doc/tutorial/](https://cplusplus.com/doc/tutorial/) - Tutorial da Linguagem C++ [EN]
* [https://en.cppreference.com/w/cpp/language](https://en.cppreference.com/w/cpp/language) - Guia de referencia da Linguagem C++ [EN]
* [https://learn.microsoft.com/pt-br/cpp/cpp/cpp-language-reference?view=msvc-170](https://learn.microsoft.com/pt-br/cpp/cpp/cpp-language-reference?view=msvc-170) - Guia da Microsoft de C++ [PT]
* [https://www.inf.ufpr.br/ci208/NotasAula.pdf](https://www.inf.ufpr.br/ci208/NotasAula.pdf) - Guia da UFPR de C++ [PT]
* [https://gcc.gnu.org/onlinedocs/libstdc++/manual/index.html](https://gcc.gnu.org/onlinedocs/libstdc++/manual/index.html) - Manual da Implementação de GNU de C++ [EN]
