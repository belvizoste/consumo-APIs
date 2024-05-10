As APIs possuem alguns elementos que servem à sua utilização: 

* **Ponto de entrada:** é o endereço do serviço hospedado e que pode ser acessado através de um navegador ou uma ferramenta de consumo de APIs. Exemplo: <https://dadosabertos.camara.leg.br/api/v2>

* **Recursos:** são serviços de dados disponíveis para o consumo. Exemplo: **/deputados** -> <https://dadosabertos.camara.leg.br/api/v2/deputados>. 

* **Parâmetros:** são informações ou filtros que servem para enviar dados da consulta ou para serem processados pela API. Os parâmetros podem ser passados para a API através da URL ou no corpo (body) da requisição. Exemplo: ? nome=bebeto -> <https://dadosabertos.camara.leg.br/api/v2/deputados?nome=bebeto>.

* **Métodos:** são os modos de consumo de uma API, que podem ser: 
    - POST: inserção (CREATE);
    - GET: consulta/leitura (READ);
    - PUT: atualização (UPDATE);
    - DELETE: deleção (DELETE).

Para este projeto, vamos usar o Node.js e o NPM (Node Package Manager):
- Node.js v20.13.0 LTS -> Long Term Suport (versão estável);

NPX -> Node Package Executable (Executador de pacote de Node). 

### Instalação e uso do Json Server 

Para instalar o Json Server no Vs Code, utilizamos o comando `"npm install json-server"` para baixar o pacote JSON Server no seu ambiente Node.js, esta é uma ferramenta que permite criar rapidamente uma API completa com base em no arquivo JSON. Este pacote pode ser acessado através do link:  <http://github.com/typicode/json-server>

### Criação do .gitignore
Um arquivo **.gitignore** é um arquivo de configuração usado pelo Git para especificar quais arquivos e diretórios devem ser ignorados e não incluídos no controle de versão. Neste caso, criamos este arquivo para ocultar a pasta `"node_modules"` do pacote JSON Server. 

### Utilidade dos arquivos package 

Ao instalar o pacote do Json Server, os arquivos `package.json` e `package-lock.json` são adquiridos e são responsáveis por diversas funções do Node.js: 

* **package.json ->** é  um cartão de identificação do projeto Node.js, onde são listadas as informações importantes, como o nome do projeto, suas dependências e scripts úteis.

* **package-lock.json ->** é uma lista precisa das versões exatas das dependências do projeto, garantindo que todos que trabalham no projeto tenham as mesmas versões das dependências instaladas. Ela é uma ferramenta padrão desse sistema e já é instalada de forma automática. 

###  Criação do script "start" no package.json 

No arquivo `package.json`, criamos um script que automatize o processo de iniciação do projeto, o código utilizado foi: 

~~~script
 "scripts": {
    "start": "npx json-server data/db.json5"
  }
~~~

###  Observações em relação ao uso do JSON vs. JSON





TO-DO (documentar): 
- Observações em relação ao uso do JSON vs. JSON: <http://github.com/json5/json5>
- Instalação das extensões para formatação de arquivo .json5 
- Chamada do script start com NPM ao invés do NPX
- O que é o Chocolatey (e porque não instalá-lo agora)

Da aula de sexta (10/05):

- Instalação de dependencias de projeto com o comando npm install 