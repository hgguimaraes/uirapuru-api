<div align="center">
  <img src="./src/assets/LogoUirapuru.png" width="180"></img>
<h1 align="center" style="font-size: 45px;">
  Uirapuru API
</h1>
</div>

[Website for the Uirapuru platform made for be experienced in a desktop](https://uirapuru.techamazon.tech/)

[Deploy to stage develop](https://github.com/Techamazonof/uirapuru-api/actions/workflows/develop.yml)

[Deploy to stage production](https://github.com/Techamazonof/uirapuru-api/actions/workflows/production.yml)

# Documentação da API Uirapuru

Esta documentação fornece uma visão geral da API Uirapuru, um projeto web desenvolvido utilizando várias tecnologias. Abaixo estão os detalhes das tecnologias utilizadas e instruções sobre como começar a trabalhar no projeto.

## Tecnologias Utilizadas

O projeto Uirapuru API utiliza as seguintes tecnologias:

1. [Node.js](https://nodejs.org/en/docs/): É uma plataforma de desenvolvimento de código aberto baseada no motor V8 do Google Chrome, que permite a execução assíncrona de código JavaScript no lado do servidor. Sua arquitetura orientada a eventos torna-o ideal para aplicações em tempo real e altamente escaláveis, adequadas para construir servidores web e APIs eficientes. É amplamente utilizado para desenvolvimento full-stack em JavaScript, oferecendo um ecossistema robusto de módulos através do npm.

2. [Express.js](https://expressjs.com/pt-br/4x/api.html): É um framework web para Node.js, oferecendo uma abstração mínima para construção de aplicações web e APIs. Baseado em middleware, possibilita o processamento eficiente de requisições HTTP e gerenciamento de rotas. Sua modularidade e extensibilidade permitem a integração de pacotes de terceiros, tornando-o uma escolha popular para o desenvolvimento de aplicações web rápidas e escaláveis em Node.js.

3. [Babel](https://babeljs.io/docs/): É um compilador de código JavaScript de código aberto, projetado para converter código ECMAScript 2015+ em versões compatíveis com navegadores e ambientes mais antigos. Ele permite que os desenvolvedores utilizem as últimas funcionalidades da linguagem, transformando-as em sintaxes que podem ser compreendidas por versões anteriores do JavaScript.

   - `@babel/cli: É a interface de linha de comando do Babel, permitindo compilar arquivos e diretórios usando a configuração do projeto.`
   - `@babel/core: É o núcleo do Babel, responsável por toda a análise, transformação e geração de código.`
   - `@babel/node: Permite a utilização do Babel diretamente no Node.js, habilitando o suporte a import/export e outros recursos avançados.`
   - `@babel/preset-env: Um conjunto de plugins para transformar o código para versões específicas do ECMAScript, com base nos ambientes de destino definidos.`
   - `@babel/preset-typescript: Habilita o suporte para a compilação de arquivos TypeScript, permitindo que sejam utilizados com o Babel.`

4. [TypeScript](https://www.typescriptlang.org/docs/): É um superset de JavaScript que adiciona recursos tipados e outras melhorias, proporcionando código mais estruturado, seguro e de fácil manutenção. Amplamente utilizado em projetos modernos, oferece autocompletar e análise estática, aumentando a produtividade dos desenvolvedores. Ao compilar, é transformado em JavaScript puro, garantindo compatibilidade com todos os ambientes que suportam JavaScript.

   - `@types/*: Pacotes de definições de tipos para bibliotecas JavaScript, permitindo que o TypeScript entenda e verifique os tipos dessas bibliotecas durante o desenvolvimento.`
   - `ts-node: Um executável que permite a execução direta de arquivos TypeScript no Node.js, sem a necessidade de compilação prévia, facilitando o desenvolvimento e depuração.`

5. [Prisma](https://www.prisma.io/docs/): É um poderoso ORM (Object-Relational Mapping) para Node.js e TypeScript, que age como uma camada de abstração de banco de dados. Com uma sintaxe declarativa, os desenvolvedores podem facilmente definir modelos de dados e relacionamentos, permitindo a geração automática de queries SQL otimizadas. Além disso, o Prisma oferece recursos avançados, como migrações de banco de dados para gerenciar alterações no esquema de forma segura e controlada. Sua API de cliente protege contra vulnerabilidades comuns, como injeção de SQL, e disponibiliza métodos para operações CRUD. O Prisma se destaca como uma escolha moderna e eficiente para desenvolver aplicações escaláveis, seguras e de alto desempenho.

   - `@prisma/client: é uma biblioteca gerada automaticamente pelo Prisma que fornece um cliente de banco de dados otimizado para realizar operações de forma segura e eficiente, utilizando os modelos de dados definidos.`

6. [Serverless Framework](https://www.serverless.com/framework/docs/): É uma plataforma de código aberto para desenvolvimento e implantação de aplicações sem servidor (serverless). Ele facilita a criação de funções e recursos em nuvem através de uma configuração declarativa, permitindo que os desenvolvedores gerenciem facilmente infraestrutura, escalabilidade e integrações em diversos provedores de nuvem. O Framework suporta várias linguagens de programação e oferece uma extensa biblioteca de plugins para personalização e automação de tarefas. Com o Serverless Framework, os desenvolvedores podem criar aplicações escaláveis e eficientes, concentrando-se no código e na lógica de negócio, sem se preocupar com a infraestrutura subjacente.

   - `serverless-offline: plugin que simula o ambiente serverless localmente para desenvolvimento e testes offline.`
   - `serverless-plugin-common-excludes: plugin que exclui arquivos comuns, como arquivos .git, do pacote de implantação.`
   - `serverless-plugin-include-dependencies: plugin que inclui automaticamente as dependências no pacote de implantação.`
   - `serverless-prune-plugin: plugin que remove funções e camadas não utilizadas após a implantação.`
   - `serverless-stage-manager: plugin que permite gerenciar facilmente múltiplos ambientes ou estágios (stages) de implantação.`
   - `serverless-http: plugin que permite criar funções serverless a partir de aplicativos HTTP existentes, como Express.js.`

7. [ESLint](https://eslint.org/docs/): É uma ferramenta de análise estática de código para JavaScript e TypeScript. Ele identifica e reporta problemas de estilo e erros de programação, seguindo regras configuráveis. O ESLint é altamente personalizável, permitindo que os desenvolvedores definam suas próprias regras ou adotem configurações predefinidas, como o padrão Airbnb. Ele é amplamente utilizado em projetos para garantir a consistência e qualidade do código, melhorar a legibilidade e prevenir erros comuns, proporcionando uma experiência de desenvolvimento mais confiável e eficiente.

   - `@typescript-eslint/parser: um analisador de código do ESLint para suportar análise estática de arquivos TypeScript.`
   - `@typescript-eslint/eslint-plugin: plugin do ESLint com regras específicas para TypeScript, aprimorando a análise estática e identificação de erros.`
   - `eslint-import-resolver-typescript: plugin de resolução de importação para TypeScript no ESLint, permitindo que importações sejam resolvidas corretamente em projetos TypeScript.`
   - `eslint-plugin-import: plugin do ESLint para análise estática de importações, auxiliando na detecção de problemas e padronização.`
   - `eslint-plugin-import-helpers: plugin do ESLint para análise estática de importações, auxiliando na detecção de problemas e padronização.`

8. [Nodemon](https://nodemon.io/): É uma ferramenta de desenvolvimento para Node.js que monitora e reinicia automaticamente o servidor sempre que detecta alterações nos arquivos do projeto. Ele permite um fluxo de desenvolvimento contínuo, eliminando a necessidade de reiniciar manualmente o servidor a cada modificação no código. O Nodemon é amplamente utilizado para agilizar o desenvolvimento de aplicações Node.js, proporcionando uma experiência mais produtiva e eficiente.

9. [Jest](https://jestjs.io/docs/): É um framework de testes em JavaScript, altamente configurável, usado em aplicações Node.js e front-end. Ele oferece suporte para testes unitários, integração e snapshots, além de integração nativa com ES6 e TypeScript. Jest é amplamente adotado pela sua velocidade, simplicidade e recursos avançados, como mocks e spies, que permitem uma cobertura abrangente de testes em projetos JavaScript. Sua comunidade ativa e vasta documentação o tornam uma escolha popular para garantir a qualidade e a estabilidade do código em ambientes de desenvolvimento.

   - `@types/jest: pacote que fornece definições de tipos TypeScript para o Jest, permitindo o desenvolvimento com TypeScript e garantindo a verificação de tipos durante o desenvolvimento e testes.`
   - `vitest: ferramenta que oferece um ambiente de testes leve e rápido para aplicações Node.js, adequada para execução em ambientes de desenvolvimento e CI/CD.`
   - `vitest-mock-extended: plugin para o vitest que permite a criação de mocks estendidos, oferecendo recursos avançados para criar e manipular mocks durante os testes.`

10. [AWS SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/): O AWS SDK (Software Development Kit) é uma biblioteca e conjunto de APIs que permite interagir e gerenciar os serviços da Amazon Web Services (AWS). Suporta várias linguagens de programação e oferece recursos para criar, implantar e gerenciar recursos na nuvem AWS, como instâncias EC2, bancos de dados RDS e objetos S3. Além disso, fornece funcionalidades avançadas, como autenticação, integração com serviços específicos da AWS e acesso a métricas e logs para monitoramento e análise de desempenho. O AWS SDK é amplamente utilizado para desenvolver aplicações escaláveis, seguras e confiáveis na infraestrutura da AWS.

11. [Axios](https://axios-http.com/docs/): É uma biblioteca JavaScript baseada em promessas (Promise) que oferece uma API simplificada e assíncrona para fazer requisições HTTP em ambientes Node.js e no navegador. Ele suporta todos os métodos HTTP comuns, como GET, POST, PUT e DELETE, e possui recursos avançados, como interceptadores de requisição e resposta, permitindo a manipulação e o tratamento de erros de forma eficiente. O Axios é amplamente utilizado para realizar comunicação com APIs e serviços web de forma concisa e confiável.

12. [bcrypt](https://www.npmjs.com/package/bcrypt): É uma biblioteca de criptografia de senhas para JavaScript e outras linguagens de programação. Ele utiliza um algoritmo de hash lento e adaptativo para armazenar senhas de forma segura no banco de dados, protegendo-as contra ataques de força bruta. O Bcrypt também suporta o uso de "salts" (sais) para aumentar ainda mais a segurança das senhas armazenadas. Ele é amplamente utilizado em aplicações web para garantir que as senhas dos usuários sejam armazenadas de forma segura e não sejam facilmente decifradas em caso de vazamentos de dados.

    - `@types/bcrypt: é um pacote que fornece definições de tipos TypeScript para a biblioteca Bcrypt, permitindo a verificação de tipos durante o desenvolvimento com TypeScript.`

13. [helmet](https://helmetjs.github.io/): Helmet.js é uma biblioteca middleware para Node.js que ajuda a aumentar a segurança de aplicações web ao configurar automaticamente diversos cabeçalhos HTTP relacionados à segurança. Ele oferece proteção contra vulnerabilidades comuns, como ataques de injeção de scripts (XSS), ataques de redirecionamento aberto, entre outros. O Helmet.js é altamente configurável, permitindo que os desenvolvedores escolham quais cabeçalhos de segurança desejam habilitar. É amplamente utilizado para melhorar a segurança de aplicações web, reduzindo riscos de ataques e vulnerabilidades.

14. [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken): JsonWebToken (jsonwebtoken) é uma biblioteca JavaScript que permite a criação, assinatura e verificação de tokens de acesso baseados em JSON. Ele é amplamente utilizado para autenticação e autorização em aplicações web e APIs RESTful. O jsonwebtoken utiliza o algoritmo de assinatura HMAC (Hash-based Message Authentication Code) ou RSA (Rivest-Shamir-Adleman) para garantir a autenticidade e integridade dos tokens. Os tokens gerados pelo jsonwebtoken contêm informações codificadas em formato JSON e podem ser utilizados para validar a identidade do usuário e controlar o acesso a recursos protegidos.

    - `@types/jsonwebtoken: é um pacote que fornece definições de tipos TypeScript para a biblioteca jsonwebtoken, permitindo a verificação de tipos durante o desenvolvimento com TypeScript.`

15. [Multer](https://www.npmjs.com/package/multer): Multer é uma biblioteca middleware para Node.js que lida com o processamento de formulários multipartes, permitindo o upload de arquivos em requisições HTTP. Ele oferece suporte para envio de múltiplos arquivos simultaneamente e permite configurar o destino de armazenamento dos arquivos temporários e permanentes. Além disso, Multer permite definir limites de tamanho e tipos de arquivos aceitos, fornecendo mecanismos de validação e segurança contra ataques de DoS. Essa biblioteca é amplamente adotada em aplicações web para gerenciar de forma eficiente o envio e armazenamento de arquivos em servidores Node.js.

    - `multer-s3: é um pacote que estende o Multer para possibilitar o upload de arquivos diretamente para o serviço de armazenamento na nuvem da Amazon S3.`
    - `@types/multer: é um pacote que fornece definições de tipos TypeScript para o Multer, permitindo a verificação de tipos durante o desenvolvimento com TypeScript.`
    - `@types/multer-s3: é um pacote que fornece definições de tipos TypeScript para o multer-s3, permitindo a verificação de tipos quando se utiliza o multer-s3 com TypeScript.`

16. [Nodemailer](https://nodemailer.com/about/): É uma biblioteca de envio de emails para Node.js que oferece uma API assíncrona para configurar, compor e enviar mensagens de email através de diversos protocolos de transporte, como SMTP, Sendmail, entre outros. Ele suporta anexos de arquivos, conteúdo HTML e permite personalização de cabeçalhos para atender requisitos específicos de envio de emails. O Nodemailer é altamente configurável, permitindo o uso de autenticação, TLS e SSL para garantir a segurança durante o envio dos emails. Sua abordagem assíncrona e recursos avançados tornam-no uma escolha popular para automação de envio de emails em aplicações Node.js.

    - `@types/nodemailer: é um pacote que fornece definições de tipos TypeScript para a biblioteca Nodemailer, permitindo a verificação de tipos durante o desenvolvimento com TypeScript.`

17. [Handlebars](https://handlebarsjs.com/guide/): É um mecanismo de templates JavaScript que permite a geração dinâmica de conteúdo HTML. Ele utiliza uma sintaxe simples e expressiva, com chaves duplas `{{}}` para inserir valores e chaves triplas `{{{}}}` para inserir valores HTML escapados. Handlebars trabalha com objetos de contexto, permitindo a interpolação de dados em templates pré-definidos. Ele também suporta diretivas condicionais, como `if` e `else`, e iterações com `each`, possibilitando a criação de templates flexíveis e reutilizáveis. Ao renderizar um template, Handlebars substitui as expressões com os valores correspondentes do objeto de contexto, resultando em conteúdo HTML final dinamicamente gerado.

18. [Compression](https://www.npmjs.com/package/compression): É um middleware utilizado em aplicações Node.js para comprimir o conteúdo HTTP antes de ser enviado ao cliente, reduzindo o tamanho dos dados transferidos e melhorando o desempenho. Ele utiliza algoritmos de compressão, como gzip ou deflate, para compactar os dados antes do envio. Quando o cliente solicita um recurso, o servidor verifica se a solicitação suporta compressão e, se for o caso, comprime o conteúdo antes de enviá-lo. O cliente, por sua vez, descomprime o conteúdo automaticamente antes de processá-lo. Compression é uma técnica eficaz para economizar largura de banda e reduzir o tempo de carregamento de páginas web em aplicações Node.js.

    - `@types/compression: é um pacote que fornece definições de tipos TypeScript para a biblioteca compression, permitindo a verificação de tipos durante o desenvolvimento com TypeScript.`

19. [CORS](https://expressjs.com/en/resources/middleware/cors.html): CORS (Cross-Origin Resource Sharing) é um mecanismo de segurança do navegador que impõe políticas para permitir ou restringir o acesso a recursos entre origens diferentes em aplicações web. Ele é baseado em cabeçalhos HTTP, como "Access-Control-Allow-Origin", que determinam quais origens têm permissão para fazer solicitações a um servidor. O CORS é usado para evitar ataques de solicitação cruzada (CSRF) e proteger recursos sensíveis, garantindo que apenas origens autorizadas possam interagir com o servidor. É amplamente implementado para permitir a comunicação segura entre origens diferentes em aplicações web.

    - `@types/cors: é um pacote que fornece definições de tipos TypeScript para a biblioteca cors, permitindo a verificação de tipos durante o desenvolvimento com TypeScript.`

20. [dotenv](https://www.npmjs.com/package/dotenv): Dotenv é uma biblioteca JavaScript que carrega variáveis de ambiente a partir de um arquivo `.env`, permitindo que aplicativos Node.js acessem configurações sensíveis, como chaves de API e credenciais, de forma segura. As variáveis definidas no arquivo `.env` são carregadas no processo de ambiente do Node.js durante a inicialização da aplicação. Isso facilita a configuração de ambientes de desenvolvimento, teste e produção, mantendo informações sensíveis fora do código fonte e evitando que sejam expostas acidentalmente. Dotenv é amplamente utilizado para gerenciar configurações e informações sensíveis em aplicações Node.js de forma segura e eficiente.

21. [pdfmake](https://pdfmake.github.io/docs/): pdfmake é uma biblioteca para criação de documentos PDF no Node.js. Oferece uma abordagem programática para gerar documentos PDF, permitindo a criação de PDFs personalizados com textos, imagens, tabelas, listas e outros elementos gráficos. Ideal para gerar relatórios, faturas e outros documentos que requerem formatação específica.
    - `@types/pdfmake`: Pacote de definições de tipos para pdfmake, facilitando o desenvolvimento em TypeScript ao prover verificação de tipos e autocomplete para as funcionalidades da biblioteca.

22. [http-status-codes](https://www.npmjs.com/package/http-status-codes): Esta biblioteca fornece constantes de códigos de status HTTP, tornando o código mais legível e fácil de entender. Em vez de usar números mágicos, os desenvolvedores podem utilizar as constantes nomeadas para referenciar códigos de status HTTP, melhorando a clareza e a manutenção do código. Ideal para ser usada em conjunto com frameworks de servidor como Express.js, facilitando a definição de respostas HTTP com códigos de status claros e descritivos.

## Como Iniciar o Projeto

Para começar a trabalhar com o projeto Uirapuru API, siga estes passos:

1. Clone o repositório GitHub do projeto usando o link fornecido:

   ```
   git clone git@github.com:Techamazonof/uirapuru-api.git
   ```

2. Instale o Node.js: Verifique se você tem o Node.js instalado em seu sistema. Você pode baixá-lo no site oficial: https://nodejs.org/

3. Instale as dependências do projeto: Navegue até o diretório do projeto e instale as dependências necessárias usando o npm (Node Package Manager):

   ```
   cd uirapuru-api
   npm install
   ```

4. Execute o aplicativo em modo de desenvolvimento: Use o seguinte script npm para iniciar o servidor de desenvolvimento com o nodemon para reinicializações automáticas quando houver alterações no código:

   ```
   npm run dev
   ```

5. Testes da API: O projeto inclui uma estrutura de testes usando o vitest. Você pode executar o conjunto de testes usando o seguinte script npm:

   ```
   npm test
   ```

6. Implantação: Para implantar o aplicativo, use o seguinte script npm, que irá criar o projeto e implantá-lo usando o Serverless Framework:

   ```
   npm run deploy
   ```

7. Outros Scripts: Vários outros scripts npm estão disponíveis no arquivo `package.json` para lidar com várias tarefas, e estão descritos na sessão 'Scripts do Projeto'.

## Código

branch desenvolvimento: `main`

branch produção: `production`

- Clone o projeto em seu ambiente e instale as dependências com `npm install`.

- Deploy no desenvolvimento: Se desenvolveu uma função e precisa testar no ambiente de dev, você pode rodar o comando `npm run deploy -s dev` (Fique atento de ter configurado sua função no arquivo serverless.yml)

- Depois de desenvolvido a demanda e pretende enviar para a produção, suba seu código da branch, faça um `git cherry-pick <id do seu commit>` na branch de produção `production` e faça um push.

## Migrações no banco de dados

- Para fazer alguma alteração no banco de dados como inserir, editar, alterar e deletar. Você precisará usar o docker para o ambiente de testes.

- Para uma boa prática, faça uma migração por vez (O passo 2 geralmente ja tem no repositório então não será preciso criar )

1 - Rodar comando: npx prisma db pull

2 - Criar arquivo na raiz do diretório com a extensão .sh e com o script dentro do arquivo:

- echo '\nPreparando banco de dados de teste\n'<br>
- sudo docker pull postgres<br>
- sudo docker run --name=postgres -p **\*54\*\*\*\***:**\*** -e POSTGRES_PASSWORD='**\*\*\***' -e POSTGRES_USER='techamazon' -e POSTGRES_DB='uirapurudb' -d postgres:latest<br>
- sudo docker ps

3 - Rodar comando para permissão de execução do arquivo .sh:<br>

- 3.1 - chmod 777 db.sh<br>
- 3.2 - ./db.sh

4 - Mudar URL do banco para: DATABASE_URL=postgres://techamazon:21392996@localhost/uirapurudb

5 - Rodar comando para gerar migration inicial: npx prisma migrate dev 

6 - Modificar schema.prisma

7 - Rodar comando para gerar migration final: npx prisma migrate dev

8 - Excluir migration inicial

9 - Voltar URL do banco dev

10 - Rodar migration final no banco dev: npx prisma migrate deploy

1 - rodar npx prisma db pull<br>
2 - rodar banco de dados local<br>
3 - criar migration inicial no banco local<br>
4 - fazer as modificações no schema.prisma<br>
5 - criar migration final no banco local<br>
6 - excluir migration inicial<br>
7 - rodar migration final no banco desejado<br>

- `Para que uma migração seja enviada, não poderá ter uma antes, então se der erro, exclua a migration antiga e faça a migração atual.`

- `Caso dê algum erro, pode ser que já exista containers e imagens do docker, então pare e exclua os container e imagens existentes.`

- `Outro caso de erro seria que a rota  ja estaria sendo usada, então pare o que está nessa rota e continue o processo.`

<br>
<br>

## Produção

- Se depois de testado e aprovado, o seu código pode entrar em produção. Como dito acima, entre na branch production e faça o `git cherry-pick <id do seu commit>` e depois faça um push para a branch production

- Deploy na produção:depois de ter dado o push você pode fazer o deploy com o `npm run deploy -s prod`

## Migrações no banco de dados

- Para uma boa prática, faça uma migração por vez.

1 - Depois de todo o processo de atualizar a produção com o sua alteração, você pode usar o `npx prisma migrate deploy`

- `Para que uma migração seja enviada, não poderá ter uma antes, então se der erro, exclua a migration antiga e faça a migração atual.`

## Scripts do Projeto

O `package.json` do projeto inclui uma variedade de scripts para facilitar o desenvolvimento, teste, e implantação:

- **`npm run update`**: Atualiza as dependências do projeto e salva as novas versões no `package.json`.

- **`npm run dev`**: Inicia o servidor em modo de desenvolvimento usando Nodemon, que reinicia o servidor automaticamente a cada alteração no código.

- **`npm run lint`**: Executa o TypeScript Compiler (tsc) para compilação e verifica o código com ESLint, focando em arquivos dentro do diretório `src`.

- **`npm run v`**: Atualiza a versão do projeto sem criar uma tag git, útil para controle de versão interno.

- **`npm run build`**: Limpa o diretório `dist` e transpila o código TypeScript para JavaScript compatível com versões mais antigas de navegadores e ambientes Node.js usando Babel.

- **`npm run minify`**: Minifica os arquivos JavaScript no diretório especificado, ajudando a reduzir o tamanho do arquivo para produção.

- **`npm run deploy`**: Combina os processos de build e minificação, gera os clientes do Prisma e implanta o projeto em um ambiente serverless usando o Serverless Framework.

- **`npm run start`**: Prepara o ambiente para execução local em modo de produção, servindo o projeto via Serverless Offline.

- **`npm run invoke`**: Permite a invocação local de funções serverless após a construção do projeto, especificando a função a ser invocada como argumento.

- **`npm run debug`**: Constrói o projeto e inicia o Serverless Offline em modo de depuração, permitindo a inspeção e o debug do código.

- **`npm test`**: Executa os testes do projeto com Jest, garantindo que os testes sejam executados sequencialmente e tratando corretamente as conexões pendentes para uma finalização limpa.

Lembre-se de executar esses scripts a partir do diretório raiz do projeto e de instalar todas as dependências necessárias com `npm install` antes de proceder.

<br>
<br>

## Funções

- As funções do uirapuru são o que rodam a api e para isso usamos o AWS Lambda. <br>
  <br>

Estrutura para chegar nas funções

    -- src
      - functions

Depois de desenvolver sua função você precisa importa-la no arquivo `handler.ts` e tambem declarar sua função no arquivo `serverless.yml`, seguindo toda a estrutura já montada.

## Regressão Linear

O Algoritimo para regressão linear é feito em python e se encontra em um ambiente no caminho `src\shared\linearRegression`, nele há as seguintes libs instaladas:

1. [pandas](https://pandas.pydata.org/): pandas é uma biblioteca de manipulação e análise de dados de código aberto para Python, oferecendo estruturas de dados poderosas e flexíveis como DataFrame e Series. É ideal para limpeza de dados, transformações, e análises complexas. pandas simplifica tarefas como carregar, filtrar, agrupar e visualizar dados.

2. [scikit-learn](https://scikit-learn.org/stable/): Uma biblioteca de aprendizado de máquina para Python. Oferece ferramentas simples e eficientes para análise preditiva e mineração de dados. Inclui algoritmos de classificação, regressão, clustering e redução de dimensionalidade, além de funcionalidades para pré-processamento de dados e ajuste de modelos.

   - `train_test_split`: Função do scikit-learn para dividir arrays ou matrizes de dados em subconjuntos aleatórios de treino e teste.
   - `LinearRegression`: Implementação do scikit-learn de regressão linear simples e múltipla.
   - `metrics`: Módulo do scikit-learn que fornece funções de avaliação de modelo, como erro médio quadrático e acurácia.

3. [sys](https://docs.python.org/3/library/sys.html): sys é um módulo que faz parte da biblioteca padrão do Python. Fornece acesso a algumas variáveis e funções que têm forte interação com o interpretador Python. Utilizado para manipular a linha de comando e o ambiente em que o script Python está sendo executado.


## Overview

Esta API é parte do Projeto Uirapuru, uma plataforma desenvolvida para monitoramento de sistemas elétricos utilizando dispositivos IoT conectados através da internet. Ela funciona através do framework NodeJs, desenvolvida na linguagem Typescript utilizando como banco de dados PostgresSQL e estruturada como uma aplicação Serverless.

## Contact us

<p style="font-size: 18px;">
Copyright © Tech Amazon - Soluções em Energia Elétrica, 2021
</p>
<p style="font-size: 18px;">
| comercial@techamazon.tech | https://www.techamazon.tech
</p>
