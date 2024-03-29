# angular-configuracoes-essenciais

## Instalar módulos npm(node-modules)
npm install

## Criar projeto
ng new nome-app 

## Criar projeto com módulo de roteamento
ng new nome-app --routing

## Adicionar módulo de roteamento (best practices: separate, top-level module)
ng generate module app-routing --flat --module=app

## Buildar projeto (ex: projeto clonado do github)
ng build

## Buildar projeto para deploy
ng build --prod --base-href="/nome-repositorio/"

## Abrir projeto
ng serve

## Abrir projeto e abrir página no navegador padrão
ng serve --open

## Criar novo componente
ng g c "nome-componente"

Outros comandos:

## Instalar typescript
npm i -g typescript

## Linkar typescript ao projeto
npm link typescript

## Instalar e desinstalar angular-devkit
npm uninstall @angular-devkit/build-angular 
npm install --save-dev @angular-devkit/build-angular

## Instalar Materialize
npm install materialize-css@next

## Instalar type definition materialize-css
npm install --save @types/materialize-css

## Instalar material icons
npm install material-icons

## Referenciar os arquivos materialize.css e material-icons.css (no arquivo styles.css). Obs: o ~ referencia o node_modules

@import "~materialize-css/dist/css/materialize.css";
@import "~material-icons/iconfont/material-icons.css";

## Referenciar o materialize-css no arquivo app.component.ts (importar como M pois em versões futuras, o M representa funções do jquery)
import * as M from 'materialize-css';

## Instalar cash-dom via npm
npm install --save cash-dom

## Instalar source-map
npm install --save --dev @types/source-map@0.5.2

## Identificar e matar porta 4200 (ou outra porta configurada para rodar o servidor)
netstat -ano | findstr 4200
taskkill /PID <PID> /F

## Instalar ngx-mask (mascaras p datas/etc)
npm install --save ngx-mask

## Instalar Material icons
npm install material-icons@latest

## Importar Material icons no arquivo styles.css
@import "~material-icons/iconfont/material-icons.css";

Ver demo em: https://marella.me/material-icons/demo/

## Abrir o projeto e torná-lo visível na rede lan
ng serve --host=0.0.0.0

## Gerar um novo service (skip-tests para não gerar os arquivos spec)
ng generate service usefull --skip-tests

## Instalar json-server
  
npm install json-server   (localmente)
npm install -g json-server     (globalmente)
  
## Start JSON Server
npm run json:server:routes

## Guia Http Angular
https://angular.io/guide/http

## Gerar pipes customizados
ng generate pipe exponential-strength

ou gerando a pasta pipes:
ng generate pipe exponential-strength  
ng generate pipe pipes/exponential-strength

## Instalar angular-cli-ghpages (github pages)
npm add angular-cli-ghpages
  
## Deploy github pages
angular-cli-ghpages --dir-dist/nome-repositorio

## Alterar o arquivo package.json para realizar o deploy (npm run deploy).
"build": "ng build --prod --base-href=/jogos-zerados/",
"ghpages": "angular-cli-ghpages --dir=dist/jogos-zerados",
"deploy": "npm run build & npm run ghpages"

## Angular JS X Angular 2+ (Artigo: https://www.zup.com.br/blog/angular-versoes-e-releases)

- O Angular 2+ utiliza Typescript, enquanto que o AngularJS, usa JavaScript.
- O Angular agora é feito de componentes. Assim, não tem mais necessidade de criar um controller e trabalhar com $scope.
- AngularJS não foi construído considerando o suporte mobile, enquanto o Angular 2+ é totalmente orientado ao mobile.
- A sintaxe é totalmente diferente, agora o ng-for, por exemplo, é *ngFor, o padrão da sintaxe é camelcase.
- Angular 2+ possui um CLI, para criação fácil de novos projetos, componentes e serviços.
- A definição de um serviço antes no AngularJS poderia ser feita de várias maneiras, por exemplo: uma factory, serviço, provider, constant, values. Por isso, assim - como o Angular 2+ é baseado em classes, essa é a única maneira de definir um serviço.
- A performance e o tamanho do bundle final mudou na aplicação.
