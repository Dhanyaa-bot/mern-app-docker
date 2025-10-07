Basic structure of a mern file<br>
mern-app/<br>
│<br>
├── backend/<br>
│   ├── package.json<br>
│   ├── server.js<br>
│   └── Dockerfile<br>
│<br>
├── frontend/<br>
│   ├── package.json<br>
│   ├── src/<br>
│   └── Dockerfile<br>
│<br>
└── docker-compose.yml<br>
<br>
To run everything together<br>
<br>docker-compose up --build
<br>Then open:

<br>🌐 http://localhost:3000 → React Frontend

<br>🌐 http://localhost:5000 → Node Backend
