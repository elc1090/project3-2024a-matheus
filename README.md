## Projeto: Aplicação para criação de currículos com revisão prestada por pessoas reais!

![image](https://github.com/elc1090/project3-2024a-matheus/assets/55641441/c7ddb893-7b05-4123-b0b7-3062d4c9e5a5)

Acesso: https://curriculum-app-4f416178ce59.herokuapp.com/

Repositório Original: https://github.com/matheus-delazeri/curriculum-maker

Desenvolvedor: Matheus Delazeri, Sistema de Informação

## Descrição
Esta aplicação tem como intuito facilitar a criação de currículos para pessoas pouco instruídas na área da computação. O usuário precisa apenas informar suas informações e experiências, o resto é organizado por revisores e montadores.
A aplicação está disponivel em inglês e português.

## Guia para Testes

O cronograma de testes desenvolvido para esta aplicação divide-se em 3 etapas. 
- **Etapa 1:** Ocorre do ponto de vista do usuário final, que deseja criar um novo currículo para si próprio;
- **Etapa 2:** Ocorre do ponto de um revisor de currículos, que deseja realizar correções nos currículos criados pelos usuários;
- **Etapa 3:** Esta etapa explora algumas funcionalidades adicionais da plataforma.

### **1. Ponto de vista do usuário final**

Para esta etapa, você deverá acessar a plataforma (https://curriculum-app-4f416178ce59.herokuapp.com/) com as seguintes credenciais:
- E-mail: usuario@gmail.com
- Senha: usuario123

Feito isso, você já poderá prosseguir para os testes desta etapa!

**1.1. Visualizar um currículo**

Acesse o menu "Curriculos" na barra de navegação e clique em "Visualizar" no currículo de ID **1**. Navegue até a aba "Resultado" e clique em "Ver PDF" para abrir o currículo como PDF.

**1.2. Criar um currículo**

Acesse o menu "Currículos" e clique em "+ Novo", na _grid_ de currículos. Feito isso, preencha os campos com algumas informações. Após finalizar o preenchimento dos campos, clique em "Salvar".
Feito isso, o currículo será criado e estará disponível para que revisores possam juntar-se a ele e realizarem o processo de revisão.

**1.3. Rejeitar um currículo**

Após um revisor finalizar a revisão do currículo do usuário, o currículo será movido do status "Revisão Pendente" para "Aprovação Pendente". O usuário pode então definir se irá aprovar ou não o currículo finalizado (caso o rejeite, não conseguirá baixá-lo como PDF).
Para testar esta funcionalidade, acesse o menu "Currículos" e clique em "Visualizar" no currículo de ID **2**. Assim que o currículo se abrir, navegue até a aba "Resultado" e clique em "Rejeitar". Assim, o currículo chegará em seu status final e não sofrerá mais ações.


### **2. Ponto de vista do revisor**

Para esta etapa, você deverá acessar a plataforma (https://curriculum-app-4f416178ce59.herokuapp.com/) com as seguintes credenciais:
- E-mail: revisor@gmail.com
- Senha: revisor123

**2.1. Juntar-se a um currículo**

Para começar a revisar um currículo, é necessário juntar-se a ele primeiro. Para isso, navegue até o menu "Painel de Controle" e clique em "Juntar-se" em um dos currículos disponíveis na _grid_ de currículos novos.

*De preferência, junte-se ao currículo criado no teste **1.2**.

**2.2. Editar o conteúdo de um currículo**

Para este teste, mantenha-se na página do currículo ao qual você se cadastrou no teste **2.1**.

*Caso tenha fechado a página, navegue até o menu "Revisões" e clique em "Visualizar" no currículo que deseja editar.

Agora, abra a aba "Conteúdo" e monte um currículo simples utilizando as informações disponíveis na aba "Informações". Você pode inserir variáveis para referenciar os campos presentes na aba de informações.
Por exemplo, ao adicionar _{customer.name}_ no conteúdo, o valor cadastrado no campo "Nome" (da aba "Informações") será renderizado no currículo final.

Assim que estiver OK, clique em "Salvar" para salvar a versão atual do currículo. Realize mais algumas edições e clique em "Salvar" novamente, para gerar uma nova versão.

**2.3. Restaurar versão**

Ao clicar em "Salvar" na aba "Conteúdo", uma nova versão do currículo é gerada. Você pode visualizar todo o histórico de versões na aba "Versões". 

Para este teste, navegue até a aba "Versões" e clique em "Restaurar" na versão mais antiga do currículo. Feito isso, navegue até a aba "Conteúdo" e visualize a versão restaurada.

**2.4. Finalize a revisão**

Após realizar todos os ajustes necessários, o revisor deve clicar em "Finalizar Revisão", na aba "Conteúdo", para que o currículo mude para o status "Aguardando Aprovação", onde o usuário final deverá decidir se aprova ou não o currículo criado.

Para este teste, realize o procedimento de finalização de revisão, navegando até a aba "Conteúdo" e clicando em "Finalizar Revisão".

Feito isso, navegue até aba "Resultado" para verificar o resultado final.


### **3. Adicionais**

Esta etapa explora algumas funcionalidades adicionais da plataforma.

**3.1. Alterando a senha do usuário**

Com o usuário logado no momento, clique no menu no canto superior direito (onde está o nome do usuário atual) e então no item "Perfil". Feito isso, atualize a senha do usuário para "novasenha123".

Faça _logout_ e tente acessar a plataforma com esta nova senha.

**3.2. Alterando o tema**

Para alterar o tema do painel, acesse o mesmo menu "Perfil" do teste **3.1** e selecione um novo tema na seção "Preferências do Perfil".

*Lembre-se de clicar em "Salvar" para que o tema seja aplicado.

**3.3. Alterando a linguagem**

O painel, no momento, está disponível nas linguagens `pt_BR` (Português) e `en` (Inglês). Para trocar a linguagem utilizada, navegue até o menu "Perfil" novamente e, na aba "Preferências do Perfil", altere o campo "Localidade".

*Lembre-se de clicar em "Salvar" para que a localidade seja aplicada.

## Desenvolvimento
Foquei meu desenvolvimento no "visual" do painel para aperfeiçoar minhas habilidades em _frontend_. A ideia da aplicação é ser intuitva e agradável visualmente, com um visual "clean".

## Tecnologias
- Laravel;
- [Livewire](https://laravel-livewire.com/);
- [PowerGrid](https://livewire-powergrid.com/).

## Ambiente de desenvolvimento
- PHP Storm;

## Referências e créditos
- [Heroicons](https://heroicons.com/): ícones utilizados no painel;

## Devlog

- 27/06

> [#0a3b1e618abd9a18c6632ab7e49bc9defeb739b3](https://github.com/matheus-delazeri/curriculum-maker/commit/0a3b1e618abd9a18c6632ab7e49bc9defeb739b3)
```
- Feat: added locale config per user
- Feat: added dark mode (theme) per user
```

- 28/06

> [#89cc5455bb3e14c51ae14eee269774fca595b90b](https://github.com/matheus-delazeri/curriculum-maker/commit/89cc5455bb3e14c51ae14eee269774fca595b90b)
```
- UI: minor dark mode fixes
```
> [#749c25a5a74a5f741b5545712216d3f2084bbe66](https://github.com/matheus-delazeri/curriculum-maker/commit/749c25a5a74a5f741b5545712216d3f2084bbe66)
```
- Feat: changed Trix WYSIWYG editor to ToastUI Markdown/WYSIWYG editor
- UI: minor fixes
```

- 07/07

> [#5d9b95935d777c2313852077ded77c2b738cbb39](https://github.com/matheus-delazeri/curriculum-maker/commit/5d9b95935d777c2313852077ded77c2b738cbb39)
```
- Feat: mask sensitive data of users
```

- 14/07

> [#2196c27812e53c7a5b90326cd66aff89b905f254](https://github.com/matheus-delazeri/curriculum-maker/commit/2196c27812e53c7a5b90326cd66aff89b905f254)
```
- Feat: finished status flow
- Dev: removed 'assembler' from workflow
- Feat: allow view curriculum approved as PDF
- pt_BR: added general translations
```
> [#661dad297ddf51590aff2874ccdd897376eef303](https://github.com/matheus-delazeri/curriculum-maker/commit/661dad297ddf51590aff2874ccdd897376eef303)
```
- Fix: render of experiences and educations using variable
- UI: dark mode var text to white
```

---
Projeto entregue para a disciplina de [Desenvolvimento de Software para a Web](http://github.com/andreainfufsm/elc1090-2024a) em 2024a
