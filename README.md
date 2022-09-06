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
