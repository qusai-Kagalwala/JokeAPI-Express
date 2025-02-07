# JokeAPI-Express
A simple Express.js API for fetching, adding, updating, and deleting jokes. Supports filtering jokes by type and retrieving jokes by ID.

🚀 Features

✅ Fetch a random joke

🔍 Retrieve jokes by ID or type

➕ Add new jokes

✏️ Update existing jokes (PUT & PATCH)

❌ Delete specific or all jokes (with master key protection)

📦 Installation

Make sure you have Node.js installed. Then, clone the repository and install dependencies:
git clone https://github.com/YOUR_USERNAME/JokeAPI-Express.git
cd JokeAPI-Express
npm install

▶️ Usage

Run the server using:
node index.js
By default, the server starts on http://localhost:3000.

📡 API Endpoints

🔹 Fetch Jokes

GET /random - Fetch a random joke

GET /jokes/:id - Get a joke by ID

GET /filter?type=<jokeType> - Get jokes filtered by type

🔹 Modify Jokes

POST /jokes - Add a new joke

PUT /jokes/:id - Replace an existing joke

PATCH /jokes/:id - Update specific joke fields

DELETE /jokes/:id - Remove a joke by ID

DELETE /all?key=<masterKey> - Delete all jokes (requires master key)

🛠 Example Request & Response

Fetch a Random Joke
curl http://localhost:3000/random
Response:
{
  "id": 1,
  "jokeText": "Why don't scientists trust atoms? Because they make up everything.",
  "jokeType": "Science"
}

🔑 Security

The /all DELETE endpoint requires a master key for security. Make sure to keep it safe.

👨‍💻 Contributing

Feel free to fork this repository, make changes, and submit a pull request. Contributions are welcome!

📜 License

This project is licensed under the MIT License.
