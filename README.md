## :rocket: DESAFIO GOFINANCES WEB REACT.JS E TYPESCRIPT
Aplicação GoFinances web de gestão de transações, utilizando React.js e Typescript, com rotas e envio de arquivos por formulário.

### Rotas da aplicação

Requisitos de implementação das rotas:

- **`Listar as transações da sua API`**: a página de `Dashboard` deve ser capaz de exibir uma listagem através de uma tabela, com o campo `title`, `value`, `type` e `category` de todas as transações que estão cadastradas na sua API.

- **`Exibir o balance da sua API`**: a página `Dashboard`, você deve exibir o balance que é retornado do seu backend, contendo o total geral, junto ao total de entradas e saídas.

- **`Importar arquivos CSV`**: Na sua página `Import`, você deve permitir o envio de um arquivo no formato `csv` para o seu backend, que irá fazer a importação das transações para o seu banco de dados. O arquivo csv deve seguir o seguinte modelo.

| title	          | type	    | value	  | category |
| --------------- |:---------:|--------:|----------|
| Loan	          | income	  | 1500	  | Others   |
| Website Hosting	| outcome	  | 50	    | Others   |
| Ice cream	      | outcome	  | 3	      | Food     |

### Específicação dos testes

A aplicação conta com os seguintes testes:

- **should be able to list the total balance inside the cards**: Para que esse teste passe, sua aplicação deve permitir que seja exibido na sua Dashboard, cards contendo o total de `income`, `outcome` e o total da subtração de `income - outcome` que são retornados pelo balance do seu backend.

- **should be able to list the transactions**: Para que esse teste passe, sua aplicação deve permitir que sejam listados dentro de uma tabela, toda as transações que são retornadas do seu backend.

**Dica**: Para a exibição dos valores na listagem de transações, as transações com tipo `income` devem exibir os valores no formado `R$ 5.500,00`. Transações do tipo `outcome` devem exibir os valores no formado `- R$ 5.500,00`.

- **should be able to navigate to the import page**: Para que esse teste passe, você deve permitir a troca de página através do Header, pelo botão que contém o nome `Importar`.

**Dica**: Utilize o componente `Link` que é exportado do `react-router-dom`, passando a propriedade to que leva para a página /import.

- **should be able to upload a file**: Para que esse teste passe, você deve permitir que um arquivo seja enviado através do componente de drag-n-drop na página de `import`, e que seja possível exibir o nome do arquivo enviado para o input.

### Instalar e executar o projeto:

**Backend**

Para executar este projeto é necessário também clonar o projeto backend que pode ser encontrado [aqui](https://github.com/brvictorsa/desafio-typeorm-upload-nodejs).

> As instruções de como executar o backend estão no arquivo README.md do projeto no link acima.

**Frontend**

1. Clonar o projeto frontend para seu local de trabalho (via HTTPS).

2. Executar o comando *yarn* no terminal para baixar as dependências do projeto.
```js
yarn //or npm install
```
3. Executar o frontend pelo comando.
```js
yarn start //or npm run start
```

3. Executar os testes do backend utilizando o *jest* e o *react testing library*.
```js
yarn test  //or npm run test
```

## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.

---
