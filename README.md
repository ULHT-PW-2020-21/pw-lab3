**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**
 
# Programação Web - Laboratório 3: Incluindo formulários e imagens SVG no seu website  

## Objetivo
* Neste laboratório estenderá o website criado no Laboratório 2, incluindo formulários e imanges SVG.
* Este laboratório deverá ser concluido antes da sua aula prática da semana de 8 de março. Este será avaliado nessa aula. 

## Recomendações
* Leia o enunciado todo com atenção antes de o começar a resolver para entender o que fará.
* Execute com atenção cada passo, certificando-se que implementa todos os detalhes. Contém todos os detalhes para a criação do website. 
* Se tiver alguma dúvida, recorra ao [Moodle](https://secure.grupolusofona.pt/ulht/moodle/course/view.php?id=38119) que tem no Programa links para os slides de cada tópico, contendo todos os conhecimentos que precisa para realizar este laboratório.

## Pré-requisitos
* Deverá ter feito o [lab2](https://github.com/ULHT-PW-2020-21/pw-lab2).

# 1. Estruturação do repositório de laboratórios
1. Clone  (descarregue uma cópia) o seu repositório no seu computador local da seguinte forma:
    1. abra um processador de comandos (Tecla Windows e escreva `cmd`, ou `Powershell`, ou `git bash`)
    2. escolha a pasta onde quer colocar o repositório (navegando com o comando `cd nome-de-pasta` para entrar numa determinada pasta)
    3. escreva o comando `git clone https://github/seuusername/pw-labs-nomeapelido-numero` (hiperlink do seu repositório, com o seu username do GitHub e nome do repositório).

2. Crie a pasta `lab3`. 

3. Copie os conteúdos do `lab2` para a pasta `lab3`, que servirão de base para este laboratório.

# 2. Nova página Quizz

1. Crie uma nova página HTML `quizz.html`
2. Replique a informação base das outras páginas. Utilize o mesmo cabeçalho (elemento `h1` com o nome da cidade, imagem da cidade e menu) que as restantes páginas.
3. Atualize todas as páginas HTML, incluindo agora mais um item no menu, Quizz (antes de Home), com hiperlink para a página `quizz.html`.
4. crie um formulário com um quizz sobre a cidade. Deverá ter uma primeira área (elemento `fieldset`) para inserção de dados pessoais:
   * Nome
   * apelido
   * email

Noutro ou outros elementos `fieldset` faça um quiz sobre a cidade explorando de forma imaginativa os elementos 
`input`, `select`, `textarea`, `datalist`, `label`, `fieldset`, `output`.

Deverá usar os seguintes tipos de input (atributos `type`):
    * text
    * radio
    * checkbox
    * date
    * color
    * number
    * range

Deverá garantir que utiliza pelo menos uma vez cada um dos seguintes atributos de input:
    * `value`
    * `placeholder`
    * `autocomplete`
    * `size`
    * `maxlength`
    * `form`
    * `multiple`
    * `autofocus`
    * `required``
    * `step`
    * `output`
  
# 5. Página Introdução

Na pagina `index.html` insira, no body, por debaixo do menu:
2. Um elemento `h3` com a palavra Introdução.
3. um parágrafo sobre esta cidade.
4. Pesquise na Internet por [carateres especiais UTF-8](https://www.w3schools.com/charsets/ref_html_utf8.asp) assim como por emojis na [W3Schools](https://www.w3schools.com/charsets/ref_emoji.asp) e na [emojipedia](https://emojipedia.org/): 
    1. Conte a seguir uma pequena história apenas com emojis 😉, sobre a :cityscape: que escolheu. 
    2. Coloque uma barra horizontal de separação `hr` 
    3. Conte a história por palavras suas. Use etiquetas de estilo e organizacionais para formatar cada palavra diferentemente.
    4. Coloque uma barra horizontal de separação `hr` 
    5. Conte a história por palavras suas sem formatação. 
5. De seguida num novo parágrafo apresente o seu website, criando uma lista não numerada onde apresenta em poucas palavras cada uma das páginas do seu website, incluindo um link para essa página numa das palavras.
6. Crie de seguida uma [wordcloud](https://www.wordclouds.com/) com base em palavras que associa à cidade. Adicione as palaras em "wordlist" (apague primeiro as existentes). Ponha peso 10 no nome da cidade para que esta fique com maior destaque. Pode escolher uma forma (shape), fonte (font), cores (use um fundo branco). Descarregue a imagem, e formate-a com o Paint por forma a que tenha largura de 300px como a fotografia da cidade. Isira-a por debaixo da lista.

# 6. Página Localização

Na página `local.html`:
1. Um elemento `h3` com a palavra Localização.
2. Insira um pequeno parágrafo que descreva a localização da ciadade (continente, país), assim como algumas informações geográficas destas.
3.	Insira por baixo um mapa do Google Maps do lugar. Para tal: 
    a. procure o lugar no website www.google.pt/maps
    b. Faça um zoom que considera apropriado
    c. clique em “partilhar” e na opção “incorporar mapa” 
    d. Selecione tamanho pequeno
    e. copie o código HTML resultante, `<iframe src=… >`
    f. insira esse código HTML na sua pagina HTML
    g. acerte a dimensão da janela.


# 5. Página Multimédia

Na página `multimedia.html`:
1. Um elemento `h3` com a palavra Multimédia.
2.	Insira um parágrafo que apresente duas fotografias que escolherá no Google por serem emblemáticas do lugar que escolheu.  	 	 
3. Utilize a aplicação Paint ou Paint.Net para gravar duas versões de tamanhos diferentes de cada fotografia (os comandos Ctrl+W ou Ctrl+R permitem abrir um interface que permite configurar o tamanho das imagens, consoante a aplicação): 
    1. Grande, de 800 pixels de largura. Altere o nome, incluindo _grande no fim (e.g., lisboa_grande.jpg).
    2. Pequena, de 100 pixels de largura. Altere o nome, incluindo _pequena (e.g., lisboa_pequena.jpg).
    3. Guarde as 4 fotografias na pasta `imagens`. 
    4. Insira na página HTML as imagens de 100px de largura, cada uma dentro de um elemento `picture`, incluindo uma legenda descritiva da fotografia (`caption`).  Especifique o campo `alt`. Aninhe o elemento `img` dentro de um hiperlink `a`, com hiperligação para a fotografia grande correspondente. No hiperlink, especifique o atributo `target="_blank"`, para que a imagem abra numa nova janela de forma isolada (ficará de forma primária, mas para este laboratório é suficiente).
4. Pesquise no Youtube um video sobre a cidade escolhida e insira-o na sua página recorrendo à opção "partilhar" e escolhendo "embeded".
5.	Escolha um poema que de alguma forma associa ao lugar escolhido. Escreva, usando tamanhos diferentes, o título numa linha, o nome do poeta na seguinte, seguindo-se o poema, em itálico. Todo o texto deverá estar centrado. 


# 6. Página Informações

Na página `info.html`:
1.	Um elemento `h3` com a palavra Informações.
2. Crie uma frase a introduzir uma tabela de informações a compilar sobre a cidade.	
3.	Crie uma tabela com dados à sua escolha sobre a cidade escolhida. Deverá ter pelo menos 3 colunas e 4 colunas. Uma sugestão é ir à wikipedia e extrair alguns elementos que aparecem numa tabela à direita. A terceira coluna pode consistir num elemento agrupador (por exemplo demografia, geografia, história, etc). Exemplo de tabela:

    ![](lisboa-info.png)

4.	Deve depois formatar esta tabela usando os seguintes atributos:
    * pelo menos um atributo rowspan e um coslpan (o valor de cada um sendo maior que 1). 
    * cellspacing,
    * cellpadding, 
    * bgcolor, 
    * align, 
    * border (use border="1"),
    * formatação de colunas com colgroup, explorando os atributos existentes

# 7. Submissão

A estrutura final da sua pasta `pw-labs-nomeapelido-numero` deverá ser como em baixo:
```
`pw-labs-nomeapelido-numero`
+-- index.php
+-- composer.json
+-- index.html
+-- lab1
|   +-- index.html
|   +-- report.html
|   +-- pw.html
|   +-- img
    |   +-- wordcloud.png
    |   +--  ...
+-- lab2
|   +-- index.html
|   +-- info.html
|   +-- local.html
|   +-- multimedia.html
|   +-- images
    |   +--  ...
```

1. Antes de submeter, verifique que todos os links funcionam devidamente.
2. Carregue a sua pasta no Github com as seguintes instruções: 
    1.  abra o processador de comandos e posicione-se dentro da pasta do seu repositório (`pw-labs-nomeapelido-numero`).
    2.  escreva as seguintes instruções:
        * `git add *`
        * `git commit –m "submissão laboratório 2"`
        * `git push`
3. Sincronize o GitHub com o Heroku tal como fez no [lab1](https://github.com/ULHT-PW-2020-21/pw-lab1). Deverá ir ao Heroku e, em Deploy, fazer deploy branch, de forma a colocar disponível na cloud os novos conteúdos criados. 
4. Garanta que o link da sua aplicação se encontra [aqui](https://drive.google.com/file/d/1kphRYAo78NSxWznBXHqNbPksELqlyloI/view). Inclua também o hiperlink do seu repositório privado no GitHub, e adicione os docentes de PW como membros, que têm como usernames no GitHub: luciostuder, logdarkmatter, rfgsantos. Finalize o laboratório antes da sua próxima aula prática, onde este será avaliado. 

Esperamos que tenha gostado de aplicar os conhecimentos de HTML e de ter feito um website &#127760;!
