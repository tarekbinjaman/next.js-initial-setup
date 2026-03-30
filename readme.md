Go prisma > Docs > Quickstart > postgreSQL

### 1. Create a new project

~~~
mkdir hello-prisma
cd hello-prisma
~~~

Initialize a TypeScript project:

~~~
npm init -y
npm install typescript tsx @types/node --save-dev
npx tsc --init
~~~ 

### 2. Install required dependencies

~~~
npm install prisma @types/pg --save-dev
npm install @prisma/client @prisma/adapter-pg pg dotenv
~~~

Here's what each package does:

- prisma - The Prisma CLI for running commands like prisma init, prisma migrate, and prisma generate
- @prisma/client - The Prisma Client library for querying your database
- @prisma/adapter-pg - The node-postgres driver adapter that connects Prisma Client to your database
- pg - The node-postgres database driver
- @types/pg - TypeScript type definitions for node-postgres
- dotenv - Loads environment variables from your .env file


### 3. Configure ESM support
Update tsconfig.json for ESM compatibility:

~~~
{
  "compilerOptions": {
    "module": "ESNext",
    "moduleResolution": "bundler",
    "target": "ES2023",
    "strict": true,
    "esModuleInterop": true,
    "ignoreDeprecations": "6.0"
  }
}
~~~

Update package.json to enable ESM:

~~~
{
  "type": "module"
}
~~~