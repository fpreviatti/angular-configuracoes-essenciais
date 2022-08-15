# angular-configuracoes-essenciais

## Instalar módulos npm(node-modules)
npm install

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
