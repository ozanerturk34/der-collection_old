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
docker run --name vercel-commerce -e POSTGRES_PASSWORD=1234 -d -p 5432:5432 postgres

# How to seed
cd apps/medusa
yarn seed

# Add admin to medusa
add links
medusa-config.js uncomment
yarn add @medusajs/admin
yarn build:admin
npx medusa user -e some@email.com -p some-password
