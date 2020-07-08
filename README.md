# Automation
Repository dedicated to host my entry on WEBJump's Automation teste

/////////
REQUISITOS
\\\\\\\\\

A automação foi feita utilizando VBA e UiPath, esta ultima se trata de uma ferramenta dedicada a automação de processos, os requisitos e configurações de ambiente para a utilização da aplicação são os seguintes:

- O.S: Windows 10 versão 1909
- RPA Tool: UiPath Studio Pro Community
- Navegador: Internet Explorer versão 11.900.18362.0

//// Instalação UiPath

Para instalação da ferramenta, basta acessar a página: https://www.uipath.com/pt/start-trial e baixar gratuitamente o plano Community Cloud, será necessário logar na plataforma utilizando uma conta Google/Microsoft/LinkedIn ou uma conta direta na plataforma linkada através de e-mail, após o login na plataforma a página irá direciona-lo para o portal de gerenciamento, aqui é possível baixar a versão studio da ferramenta e utilizar o orquestrador de robôs.


//// Abertura do Projeto

Ao inicializar o UiPath, você será agraciado(a) com uma sub-janela central de boas vindas, feche-a e clique em open, direcione o browser contet para a pasta do projeto e inicie o arquivo "project.json", ao fazer isso o UiPath automaticamente abrirá o projeto após realizar o download e a instalação das devidas depêndencias, após isto no canto esquerdo da tela temos o campo "Project" e no mesmo context menu temos Activities e Snippets, dentro da aba de Project haverá 2 arquivos .xaml com os nomes "Caso 1" e "caso 2", o Caso 1.xaml contempla as exigências dos itens 1) e 2) do formulário de testes, e o Caso 2.xaml contempla o item 3), para abrir os arquivos basta dar um duplo clique sob os mesmos.

//// Executando o Projeto

Após abrir o arquivo, no canto superior esquerdo há um botão dropdown com o nome "Debug File", clicando na setinha para exibir os outros conteudos deste botão haverá 3 opções:
Run File, Debug, Run.

Run File: Irá executar somente o arquivo que estiver aberto no momento.
Debug File: Irá executar em modo de depuração o arquivo que estiver aberto no momento, portanto a execução é ligeiramente mais lenta.
Run: Neste cenário irá realizar a mesma operação de Run File pois não temos um workflow orquestrado para executar as duas tarefas de maneira simultanea ou coordenada.

Após a execucação de um dos arquivos ao final da mesma, aparecerá uma message box informando que a execução foi finalizada com sucesso (Caso 1), informando o src da imagem "Selenium Webdriver" (Caso 2), para casos em que ocorra alguma falha na execução, uma mensagem será exibida na aba de output do projeto (parte inferior da IDE) informando o erro especifico, no desenvolvimento dos dois casos, preparei estas mensagens de erros para caso a automação se deparasse com algum impeditivo e não pudesse interagir com os elementos da página, estas tratativas de erros são um costume padrão de boas práticas, no cenário atual programei-as apenas para notificarem erro, porém em uma situação de o site não apresentar responsividade dentro de um valor de tempo razoavel por exemplo, poderia programar estas regras de exceções para lidarem com a situação da melhor forma possível, neste casod e exemplo poderia ser enviando um ping ao endereço da página para constatar se houve ou não queda da página, e assim gerar um relatório de log que posteriormente poderia servir como mais uma ferramenta para assertividade de qualidade do produto.

