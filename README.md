# U05-RESTful-API

Projektbeskrivning:

Installation och körning
1. Klona repot:
   git clone https://github.com/ALex-Svensson1/U05-RESTful-API

2. Installera depenencies:
   npm install

3. Skapa en .env fil med:
   MONGO_URI=<din MongoDB Atlas URI>
   PORT=5000

4. Starta servern
    npm run dev


Endpoints

1. Skapa film (POST)
curl -X POST http://localhost:5000/api/movies \
-H "Content-Type: application/json" \
-d "{\"title\":\"Interstellar\",\"director\":\"Christopher Nolan\",\"year\":2014,\"genre\":\"Sci-Fi\"}"

2. Hämta alla filmer (GET)
curl http://localhost:5000/api/movies

3. Hämta en film med ID (GET)
curl http://localhost:5000/api/movies/<id>

4. Uppdatera film (PUT)
curl -X PUT http://localhost:5000/api/movies/<id> \
-H "Content-Type: application/json" \
-d "{\"title\":\"Interstellar 2\",\"year\":2025}"

5. Ta bort film (DELETE)
curl -X DELETE http://localhost:5000/api/movies/<id>
