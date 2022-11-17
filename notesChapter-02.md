# Notas do Chapter-02

# Insumos

## Sites acessados

Abrir um projeto pré configurado de React

Criar um projeto com o template do React: https://create-react-app.dev
Baixas fonte Poppins: https://fonts.google.com/specimen/Poppins
Propriedades do styled-components: https://styled-components.com/docs/api

## Comandos no terminal

Iniciar um projeto com o create react app:

_yarn create react-app hgmoney --template typescript_

Adicionando CSS in JS:

_yarn add styled-components_

Caso o Styled-components apresente problemas podemos instalar o pacote

_yarn add @types/styled-components -D_

Obs: Final -D = Dependência de desenvolvimento
Iniciar ambiente de Desenvolvimento

_yarn start_ ou _npm run start_

Adicionando Webpack Server para solucinar problema de atualização automatica.

_yarn add webpack-server -D_

_yarn add webpack-dev-server -D_

Adicionar MirageJS

_yarn add miragejs_

Adicionar Axios

Adicionar React Modal

_yarn add react-modal_

Adicionar Complemento React Modal para TS

_yarn add @types/react-modal -D_

_yarn add axios_

Adcionando a biblioteca Polished pra adionar com aos botões de entrada e saida no Modal

_yarn add polished_

# Passos

## Configuração do CSS que é interessante ser padrão em todos os projetos

    html {
        @media (max-width: 1080px){
            font-size:93.75% //15px
        }

        @media (max-width: 720px){
            font-size: 87.75% //14px
        }
    }

## Importando as fontes

    <link rel="preconnect" href="https://fonts.googleapis.com" /> Subi na hierarquia por motivos de performance.

    <link
      href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap"
      rel="stylesheet"
    />

Ao fechar a estilização global, partiu iniciar primeiro componente

## Primeiro Component: Header

Criou o arquivo.
Neste modo de trabalho, utilizando o CSS in JS criamos uma pasta para o componente e outro para a estilização.
Estrutura da pasta Header/index.tsx e Header/styles.ts
Obs: O arquivo styles não necessita ter a extensão .tsx pois não irá utilizar o React

## Outros Componentes

Após a criação do Header os demais seguiram o mesmo padrão
Components criados: Dashboard; Summary; TransactionsTable

## Criando front-end sem back-end

Criando uma API fake

Duas alternativas

- Json-server: https://github.com/typicode/json-server.

Para essa aplicação ele não foi utilizado pois não permite ser executado junto da aplicação

- MirageJS: https://miragejs.com

Para essa aplicação foi utilizado esta opção. Algumas vantagens:

1. Banco de dados integrado;
2. Relacionamento;
3. Preenchimento com dados fictícios.

## Criar o Modal
