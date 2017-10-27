# Tema da Identidade Padr�o de Comunica��o Digital do Governo Federal para Joomla

A proposta deste reposit�rio foi tornar o tema para Joomla contido no projeto [joomla-3.x](https://github.com/joomlagovbr/joomla-3.x) um reposit�rio indepente de uma vers�o do Joomla e dar suporte a atualiza��o autom�tica do mesmo.

Como utilizar:

 * Baixar o arquivo zip da pasta dist do reposit�rio e instalar no Joomla em Extens�es > Gerenciar > Instalar.
 * Na �rea administrativa do Joomla ir em Extens�es > Temas > Estilos e selecionar "portalidentidadepadrao - Padr�o" como padr�o.
 * Ainda em Extens�es > Temas > Estilos e editar "portalidentidadepadrao - Padr�o" e realizar as configura��es necess�rias.

### Configura��o para desenvolvimento
O processo de "build" foi todo automatizadado independente de plataforma utilizando a ferramenta [Gulp](http://gulpjs.com/):

#### Pr�-requisitos
   * Instalar o [Nodejs](https://nodejs.org)
   * Instalar de forma global o GULP
        * `` npm install --global gulp-cli `` para instalar o [gulpjs](https://gulpjs.com/);
   - Ap�s a instala��o, um terminal, dentro da pasta raiz do projeto execute o comando:
        * `` npm install `` para instalar as depend�ncias;

#### Processo de build para libera��o de novas vers�es
	* Editar o arquivo package.json e alterar o atributo "version";
	* Abra um terminal na raiz do projeto e execute: `` gulp build ``. Com isso ser� gerado um build funcional na pasta build que pode ser movido ou lincado para uma instala��o de Joomla para desenvolvimento.
	* Para distribuir fa�a o envio dos arquivos gerados na pasta dist para o reposit�rio no github. Com isso as instala��es de Joomla que utilizarem o tema identificar�o a nova vers�o e poder�o ser atualizadas utilizando Extens�es > Gerenciar > Atualizar.

### Refer�ncias

 * [Portal padr�o em CMS Joomla 3.7.4](https://github.com/joomlagovbr/joomla-3.x) fork em 26/10/2017
 * [Identidade Padr�o de Comunica��o Digital do Governo Federal](http://www.secom.gov.br/atuacao/comunicacao-digital/identidade-digital-1/identidade-digital)
