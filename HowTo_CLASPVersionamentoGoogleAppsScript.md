## Como versionar projetos Google Apps Script usando CLASP

---
> O ***CLASP (Command Line Apps Script Projects)*** é uma ferramenta oficial do Google que permite gerenciar seus projetos localmente no seu computador via terminal.

----

1. ***Instalar o clasp via terminal:***
> npm install -g @google/clasp.

2. ***Fazer o login:***
> clasp login.

3. ***Baixar o projeto GAS para o repositório local para editar***
> clasp clone "ID_DO_SEU_PROJETO".

>> Para baixar crie uma pasta localmente no seu computador
>>> no meu caso, criei uma pasta no meu OneDrive que está mapeado, pois assim, os arquivos ficarão sempre na nuvem, caso o computador local apresente algum problema e também poderá ser acessado de qualquer outro dispositivo caso seja necessário

***Vantagem:*** Baixa todos os arquivos .gs e .html organizados em pastas no seu PC instantaneamente.

4. ***Atualizar a edição local para a plataforma Google***
> clasp push

5. ***Criar uma nova versão numerada***
> clasp version "Descrição da minha nova versão"

6. ***Gerar um novo deployment***
> clasp deploy -d "Descrição da atualização"

7. ***Listar os deployments***
> clasp deployments

8. ***Atualizar um deployment existente***
> clasp deploy -i [ID_DO_DEPLOYMENT] -d "Descrição da nova versão"