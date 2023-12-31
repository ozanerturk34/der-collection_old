READ ME!

# generate intial package

# turn into turbo repo
delete submodules

# Database on local
DATABASE_URL=postgres://{user}:{password}@{hostname}:{port}/{database-name}

DATABASE_URL=postgres://postgres:1234@localhost:5432
	
# How to docker
docker dashboard and install docker package
pull prostgres for docker
docker pull postgres:alpine3.19
docker run --name vercel-commerce-postgres -e POSTGRES_PASSWORD=1234 -d -p 5432:5432 postgres:alpine3.19

# How to seed
cd apps/medusa
yarn seed

# Add admin to medusa
add links
medusa-config.js uncomment
yarn add @medusajs/admin
yarn build:admin
npx medusa user -e some@email.com -p some-password

# Add redis
medusa-config.js uncomment
docker pull redis:alpine3.16
docker run --name vercel-commerce-redis -d -p 6379:6379 redis:alpine3.16
