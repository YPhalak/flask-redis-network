.
├── app.py
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
└── README.md

Flask App increments and shows a page visit counter.

Redis stores the count.

Docker Compose spins up both containers in a custom user-defined bridge network, so they can talk to each other using service names.

🔧 Setup Instructions
1. Clone the Repo

git clone https://github.com/your-username/flask-redis-docker.git
cd flask-redis-docker

2. Build and Start the Containers

docker-compose up --build

This will:

Build the Flask image from the Dockerfile

Pull the official Redis image

Start both containers on a shared Docker network

3. Open Your Browser

Visit:

http://localhost:5000

You should see something like:

Hello! This page has been visited 1 times.

🛑 Stopping the Containers
To stop and clean up:

docker-compose down

📚 Learning Points
Docker networking with docker-compose

Communication between containers using service names

Minimal Python + Redis integration using Flask
