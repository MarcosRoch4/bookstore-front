{TERMINAL}
npm install -g @angular/cli@latest
ng new [nome do projeto] --minimal

{PROJETO}
-- no arquivo angular.json informar "false" nas linhas de (inlineTemplate,inlineStyle) e salvar arquivo
--Criar arquivo app.component.html dentro da pasta app.
--inserir linha <p>App works</p> e salvar arquivo
--Excluir linhas do templater até style[] do arquivo app.component.ts
--incluir linha templateUrl: 'app.component.html' e salvar arquivo

{TERMINAL}
ng serve -- acessar o navegador, para conferir se a aplicação está ok

{NAVEGADOR}
--Criar repositório git para hospedar o projeto
--copiar a linha "remote"

{TERMINAL}
-- Colar a linha remote
git status
git add .
git status
git push -u origin master

{NAVEGADOR}
--Conferir repositório do git se a aplicação subiu

{TERMINAL}
ng add @angular/material
ng g c components/template/header

{NAVEGADOR}
--Ir até o site de componentes do angular e copiar o link na guia de API
-- em toolbar
https://material.angular.io/components/toolbar/api
import {MatToolbarModule} from '@angular/material/toolbar';

{PROJETO}
--ir até a pasta (componentes/template/header) para programar 
-- no arquivo app.module.ts
e colar, Em import do toolbar copiar o (MatToolbarModule) e colar abaixo no imports:[] e salvar o arquivo.
-- em app.component.html, remover o App Works, e incluir <app-header></app-header> e salvar o arquivo;
--na pasta assets, criar uma pasta com o nome "img", e incluir uma imagem dentro dela
-- em header.component.html

{TERMINAL}
ng g c components/template/footer
ng g c components/template/nav

{NAVEGADOR}
--Ir até o site de componentes do angular e copiar o link na guia de API
-- em sidenav
https://material.angular.io/components/sidenav/api
import {MatSidenavModule} from '@angular/material/sidenav';
https://material.angular.io/components/list/api
import {MatListModule} from '@angular/material/list';
https://material.angular.io/components/icon/api
import {MatIconModule} from '@angular/material/icon';

{PROJETO}
-- no arquivo app.module.ts
e colar, Em import do toolbar copiar o (MatSidenavModule) e colar abaixo no imports:[] e salvar o arquivo.
e colar, Em import do toolbar copiar o (MatListModule) e colar abaixo no imports:[] e salvar o arquivo.
e colar, Em import do toolbar copiar o (MatIconModule) e colar abaixo no imports:[] e salvar o arquivo.

{TERMINAL}
ng g c components/views/home

{NAVEGADOR}
import {MatCardModule} from '@angular/material/card';
https://material.angular.io/components/card/api

{PROJETO}
-- no arquivo app.module.ts
e colar, Em import do toolbar copiar o (MatCardModule) e colar abaixo no imports:[] e salvar o arquivo.