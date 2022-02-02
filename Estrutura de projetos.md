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

{NAVEGADOR}
import {MatTableModule} from '@angular/material/table';
https://material.angular.io/components/table/api

{PROJETO}
-- no arquivo app.module.ts
e colar, Em import do toolbar copiar o (MatTableModule) e colar abaixo no imports:[] e salvar o arquivo.
--na pasta "categoria" criar o arquivo categoria.model.ts
--no arquivo "environment.ts" inserir o caminha da API na linha da baseUrl:''

{TERMINAL}
ng g s components/views/categoria/categoria

{PROJETO}
-- no arquivo app.module.ts
adicionar o import do httpmodule
import { HttpClientModule } from "@angular/common/http";
e colar, Em import do toolbar copiar o (HttpClientModule) e colar abaixo no imports:[] e salvar o arquivo.

{NAVEGADOR}
import {MatButtonModule} from '@angular/material/button';
https://material.angular.io/components/button/api


{PROJETO}
-- no arquivo app.module.ts
e colar, Em import do toolbar copiar o (MatButtonModule) e colar abaixo no imports:[] e salvar o arquivo.

{TERMINAL}
ng g c components/views/categoria/categoria-create 


{PROJETO}
-- no arquivo app.module.ts
import {FormsModule} from "@angular/forms";
e colar, Em import do toolbar copiar o (FormsModule) e colar abaixo no imports:[] e salvar o arquivo.

{NAVEGADOR}
import {MatInputModule} from '@angular/material/input';
https://material.angular.io/components/input/api
https://material.angular.io/components/form-field/overview
import {MatFormFieldModule} from '@angular/material/form-field';


{PROJETO}
-- no arquivo app.module.ts
e colar, Em import do toolbar copiar o (MatInputModule) e colar abaixo no imports:[] e salvar o arquivo.
e colar, Em import do toolbar copiar o (MatFormFieldModule) e colar abaixo no imports:[] e salvar o arquivo.


{NAVEGADOR}
import {MatSnackBarModule} from '@angular/material/snack-bar';
https://material.angular.io/components/snack-bar/overview


{PROJETO}
-- no arquivo app.module.ts
e colar, Em import do toolbar copiar o (MatSnackBarModule) e colar abaixo no imports:[] e salvar o arquivo.

{TERMINAL}
ng g c components/views/categoria/categoria-delete 


