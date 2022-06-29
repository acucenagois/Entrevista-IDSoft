# Entrevista Técnica - IDSoft

<!---Esses são exemplos. Veja https://shields.io para outras pessoas ou para personalizar este conjunto de escudos. Você pode querer incluir dependências, status do projeto e informações de licença aqui--->

<!-- <img src="exemplo-image.png" alt="exemplo imagem">

> Linha adicional de texto informativo sobre o que o projeto faz. Sua introdução deve ter cerca de 2 ou 3 linhas. Não exagere, as pessoas não vão ler.
 -->
 
 [<img align="left" height="94px" width="94px" alt="Nubank" src="https://media-exp1.licdn.com/dms/image/C4E0BAQEaE9DEFe5rjw/company-logo_200_200/0/1591023724070?e=2147483647&v=beta&t=zHKPpImDAVqkGzU2gvGxw_BlYR40thkcW-cHFXOuY-A"/>](https://grupoidsoft.com.br/)

**Fullstack Jr** \
[**IDSOFT**](https://grupoidsoft.com.br/) • Contrato \
Linguagens, Tecnologias & Bibliotecas: `Typescript`, `React, Material UI, Git` \
Tempo de conclusão: 4 dias
<br/>
<br/>

## 💻 Pré-requisitos

Antes de começar, verifique se você atendeu aos seguintes requisitos:
<!---Estes são apenas requisitos de exemplo. Adicionar, duplicar ou remover conforme necessário--->
* Você instalou a versão mais recente de `node.js / yarn / react`
* Você tem conhecimento básico em `Typescript / React Hooks / Axios`
* Você leu a documentação do [React](https://pt-br.reactjs.org/)

A entrevista técnica será baseada na criação de 3 componentes que deverão ser chamados no arquivo `index.tsx`, o escopo principal de cada componente definido foi definido desta maneira:

- [ ] Tarefa #01 - Plotagem e interação com mapas. 
- [ ] Tarefa #02 - Criação de cards contendo gráficos diversos.
- [ ] Tarefa #03 - Consumo de API (Método GET).

## 🚀 Instalando componentes básicos

Para esta entrevista técnica é interessante que você use o template de exemplo do material ui, para isso utilize os seguintes comandos
```
curl https://codeload.github.com/mui/material-ui/tar.gz/master | tar -xz --strip=2 material-ui-master/examples/create-react-app-with-typescript
cd create-react-app-with-typescript
```
Instale as dependências e comece!
```
yarn install
yarn start
```

## 📫 Colaborando seu código conosco
Quando terminar de realizar as tarefas será necessário que você compartilhe seu código conosco. Para isso você deverá criar um repositório siga estas etapas:

1. Crie um repositório privado no github.
2. Defina o nome do repositório como: `<seu-nome>-entrevista-idsoft`.
3. Compartilhe seu repositório com o seguinte usuário: `email@email.com'`

## 🗺️ Tarefa #01 - Plotagem e interação com mapas. 

<img align="right" width="350" src="https://i.ibb.co/NFRrs3r/Screen-Shot-2022-06-29-at-00-20-46.png" />

Esta tarefa consiste na criação de um componente contendo um mapa que mapa deverá estar dentro de um componente `<Card>`, este mapa deverá conter 3 marcadores, onde cada um deverá realizar uma função diferente, sendo elas:

- [ ] Ao clicar no 📍 #1  uma `popup` aparecerá no mapa contendo `Grupo IDSOFT`.
- [ ] Ao passar o mouse no 📍 #2 uma `tooltip` deverá aparecer no mapa.
- [ ] Ao passar o mouse no 📍 #3 um `polígono` deverá aparecer no mapa.

A posição inicial do mapa determinada pela variável:

```typescript
const position = [-3.6915319, -40.3543809]
```

Para os marcadores escolha qualquer posição no mapa.

## 📈 Tarefa #02 - Criação de cards contendo gráficos diversos.

<img align="right" width="350" src="https://i.ibb.co/N2cnYSf/Screen-Shot-2022-06-29-at-00-57-19.png" />

Esta tarefa consiste na criação de um componente contendo 5 `<Card>`, cada cartão deverá apresentar um tipo de gráfico diferente, é interessante a utilização de componantes como `Grid` para uma melhor organização desses cartões, sinta-se livre para decidir a biblioteca de gráficos que irá utilizar no projeto, os dados as serem utilizados e a forma como eles serão mostrados nos cartões, aqui vai uma dica de quais cartões achamos interessantes você criar:

- [ ] Card com informação geral (Exemplo: OFF / ON)
- [ ] Card com gráfico de pizza
- [ ] Card com gráfico de linha
- [ ] Card com gráfico de barras
- [ ] Card com informação geral #2 (Exemplo: 70°C)

## 🤝 Tarefa #03 - Consumo de API (Método GET).
<img align="right" width="250" src="https://i.ibb.co/zZj8qTt/Screen-Shot-2022-06-29-at-01-52-38.png" />

Nesta tarefa você deverá criar um componente contendo 1 (um) `<Card>` renderizando informações diversas de um usuário fictício tais como: `Nome`, `telefone`, `endereço`, `etc`, os dados a serem disponilizados devem ser obtidos através de uma consulta a API Open Source [RANDOM USER](https://randomuser.me/api).

Recomendamos a utilização método de requisação GET do cliente HTTP `axios` 

```javascript
axios.get('https://randomuser.me/api')
...

```

Além da renderização dos dados será interessante a criação de 2 botões com funções distintas, sendo elas:

- [ ] O `Botão 1` ao ser clicado deverá mudar o tipo de dado a ser mostrado. Ex: `Telefone` -> `Email`
- [ ] O `Botão 2` ao ser clicado deverá mudar o usuário que está sendo mostrado. Ex: `João`-> `Maria`
