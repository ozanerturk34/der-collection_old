READ ME!

DATABASE_URL=postgres://{user}:{password}@{hostname}:{port}/{database-name}

DATABASE_URL=postgres://postgres:1234@localhost:5432
	
docker run --name vercel-commerce -e POSTGRES_PASSWORD=1234 -d -p 5432:5432 postgres

cd apps/medusa
yarn seed