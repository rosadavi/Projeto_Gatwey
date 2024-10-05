# Gateway de pagamento via PIX
# Gateway-Front

# Gateway-Back
Back-End do Gatway de Pagamento do BR Fideliza

## Pre-requisitos
1. Nodejs
2. Npm
3. Mysql

## Instalação e Uso
1. Clone o repositório
2. Instale as dependências utilizando o comando `npm ci`
3. Crie um banco Mysql com a query 
```
CREATE DATABASE Gateway 
```
4. Criar o arquivo .env na raiz do projeto seguindo o modelo:
```
DATABASE_URL="mysql://user:password@address:port/Gateway"
```
5. Execute o comando `npx prisma db push` para aplicar a modelagem salva no prisma ao banco configurado
6. Execute o comando `npx run dev` para iniciar o servidor
7. Acesse o prisma studio com o comando `npx prisma studio` para visualizar o banco

## Lista de Comandos

```bash
npm ci // Instala as dependências
npm run dev // Inicia o servidor
npx prisma db pull // Importa a modelagem do banco para a conexao do prisma
npx prisma db push // Exporta a modelagem do prisma para o banco
npx prisma generate // Atualiza a modelagem interna do prisma com a externa
npx prisma studio // Abre o prisma studio para visualizar o banco
```
