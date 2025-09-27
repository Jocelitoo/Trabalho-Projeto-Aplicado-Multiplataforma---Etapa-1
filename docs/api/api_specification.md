Endpoints previstos:

- /exemplo.com/api/sign-cloudinary-params

Parâmetros de requisição:

- DELETE

Formatos de resposta:

- "Sucesso"

Autenticação e autorização:

- NextAuth será usado para gerenciar o sistema de login
- Somente usuários logados conseguirão usar funções relacionadas ao banco de dados / cloudinary

OBS: Optamos por não usar API request em diversas partes do projeto porque o sistema se tornará mais otimizado se fizermos as requisições ao banco de dados através do Server Actions e não por API
