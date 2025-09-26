Título do projeto: ConectaONG

Descrição do projeto: O ConectaONG é uma plataforma que tem o objetivo de conectar, de forma simples, usuários às ONGS de Fortaleza, apresentando suas necessidades de voluntários, itens e canais de contato. Com o ConectaONG, em poucos segundos qualquer pessoa poderá acessar informações da ONG escolhida, como endereço, voluntários necessários, itens em falta e formas de contato. Da mesma forma, as ONGS poderão se cadastrar e atualizar suas informações de maneira prática.

Problema abordado e justificativa: As informações a cerca das ONGS são extremamente escassas e o problema fica ainda maior quando queremos saber as necessidades delas. O problema que queremos solucionar é justamente essa dificuldade para encontramos informações sobre as ONGS.

Objetivo do sistema: Trazer mais visibilidade para as ONGS de Fortaleza, tanto no sentido de informações sobre elas quanto nas suas necessidades de materiais e voluntáriado.

Escopo do projeto:
-1.Objetivo do projeto: Desenvolvedor um site fácil de usar que conecta o público às ONGS da cidade e suas necessidades.

-2.Entregas do projeto:
--Pagina inicial (home)
--Página de Login / registro
--Página minha ONG (para criação, edição ou exclusão da ONG)
--Página com a lista de usuários, permitindo exclusão e edição (exclusivo para o admin)
--Página com a lista de ONGS criadas, permitindo exclusão (exclusivo para o admin)
--Página com as informações da ONG escolhida
--Layout responsivo
--Redirecionamento para as redes sociais das ONGS

-3.Fora do escopo:

- Doação de valores não serão feitas através do site

Tecnologias propostas:

- Frameworks: Next.js e tailwind
- Libs: react, shadcn, zod, next-auth, bcrypt, prisma, cloudinary, dayjs
- Linguagem: Typescript
- Banco de dados: MongoDB
- Banco de imagens: Cloudinary

Visão geral da arquitetura: Client-server

Diagrama da arquitetura: [ Cliente - Navegador ] --> [ Servidor Next.js ] --> (Entrega frontend (SSR/SSG), Server actions) --> [ Servidor de Banco de Dados (MongoDB) e banco de Imagens (Cloudinary)]

Cronograma para Etapa 2 (N708):

- Criação manual de dados ficticios de ONGS em um arquivo
- Criação do Header e Footer
- Criação da Home
- Utilização dos dados ficticios para verificar como ficou a Home
- Criação da página Sobre a ONG
- Utilização dos dados ficticios para verificar como ficou a página Sobre a ONG
- Criação no MongoDB da base de dados
- Conexão do Prisma com o MongoDB e configuração dos models de User e ONG
- Criação da página de registro de usuário
- Vericar se o usuário está sendo salvo no MongoDB
- Por padrão, todos os usuário criados terão a role de 'ONG'. Por só haver 1 'Admin' no sistema, altere manualmente no MongoDB a role do usuário que será o admin de 'ONG' para 'Admin'
- Configuração do Next-Auth para login
- Criação da página de Login
- Verificar se o Login está funcionando
- Conectar o projeto ao cloudinary para armazenas imagens
- Criar a página de criação / edição de ONG
- Criar uma ONG
- Verificar se as imagens da ONG estão sendo salvas no Cloudinary
- Verificar se a ONG está sendo salva / editada no MongoDB
- Editar ONG e verificar se as alterações foram salvas no MongoDB
- Substituir na Home os dados ficticios das ONGS pelos dados vindo do MongoDB
- Criar a página com a lista de usuários que só o Admin terá acesso
- Adicionar a funcionalidade de remover usuários que só o Admin terá acesso
- Verificar se os links de redirecionamento das ONGS para suas redes sociais estão funcionando
- Verificar como está o site em telas menores
- Verificar a velocidade do site com o Lighthouse

Integrantes da equipe e seus papéis:
Italo -> Responsável pela página principal (Home)
Daniel -> Responsável pelos formulários de login / registro
Neto -> Responsável por configurar o banco de dados com o prisma
Jocelito -> Responsável pelas requisições feitas pelo Server Actions
Kaio -> Responsável por criar a página que traz informações sobre a ONG e garantir a otimização do site
Juliana -> Responsável por verificar a responsividade e corrigir erros
