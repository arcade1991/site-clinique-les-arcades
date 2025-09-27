git clone https://github.com/TON_COMPTE/site-clinique-les-arcades.git
cd site-clinique-les-arcades
# site-clinique-les-arcades
docker-compose up --build -d
docker-compose logs -f
cd backend
npx prisma migrate dev --name init
npx ts-node prisma/seed.ts
npx ts-node prisma/seed.ts
docker exec -it site-clinique-les-arcades_db_1 psql -U clinic -d clinicdb -c "SELECT * FROM \"Medecin\";"
docker exec -it site-clinique-les-arcades_db_1 psql -U clinic -d clinicdb -c "SELECT * FROM \"Medecin\";"
http://localhost:4000/api/medecins
http://localhost:4000/api/appointments
http://localhost:4000/api/health
