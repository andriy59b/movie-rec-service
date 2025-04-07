# Movie Recommendation Service  
API service for movie recommendations built with FastAPI and Python

## Installing using GitHub

Install PostgreSQL (if using a database) and create a database if needed.

```bash
git clone https://github.com/andriy59b/movie-rec-service.git
cd movie-rec-service
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
Configure Environment Variables
Create a .env file in the root directory.
Make sure it includes all the variables listed in the .env.example file.
Ensure that the variable names and values match those in the sample file.

bash
Copy
Edit
set SECRET_KEY=<your secret key>
set MODEL_PATH=./models/recommender.pkl
You can generate a secret key using Python:

python
Copy
Edit
import secrets; print(secrets.token_hex(32))
Run the Server
To start the development server, run:

bash
Copy
Edit
uvicorn app.main:app --reload
Then open in browser:

Swagger docs: http://127.0.0.1:8000/docs

ReDoc docs: http://127.0.0.1:8000/redoc

Run with Docker
Docker and Docker Compose must be installed

bash
Copy
Edit
docker-compose build
docker-compose up
The API will be available at http://localhost:8000

Features
🎬 Movie recommendations based on user preferences

🧠 Machine Learning model (collaborative or content-based filtering)

⚡ Built with FastAPI for high performance

🔐 Optional JWT authentication support

📊 Auto-generated API documentation via Swagger and ReDoc

🧪 Ready for testing and integration

