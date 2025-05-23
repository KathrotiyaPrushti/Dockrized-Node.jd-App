# 🐳 Dockerized Node.js App with MongoDB & Mongo Express

A beginner-friendly Node.js application that showcases the power of Docker through **containerization** 🧩, **networking** 🌐, **volumes** 💾, and **Docker Hub image publishing** ☁️. This project is a great starting point to learn how to run multi-container apps using Docker.

---

## ✨ Features

- 🚀 Node.js backend with Express
- 🛢️ MongoDB containerized database
- 🖥️ Mongo Express for viewing MongoDB data
- 🌐 Docker networking to connect containers
- 💾 Docker volumes to persist MongoDB data
- ☁️ Docker Hub deployment for image sharing

---

## 🧰 Tech Stack

| Layer         | Technology           |
|---------------|----------------------|
| Backend       | Node.js + Express    |
| Database      | MongoDB (Docker image) |
| DB Viewer     | Mongo Express        |
| Containerization | Docker, Docker Compose |
| Deployment    | Docker Hub           |

---

## 📸 Screenshots

### 1. App Running in Browser 🌟
![image](https://github.com/user-attachments/assets/4eb8ef65-9362-428a-a8a3-78b3507acdec)


### 2. Mongo Express Dashboard 🗄️
![image](https://github.com/user-attachments/assets/83b32ffa-9a7d-4857-b977-d1c61348e048)

---

## 🛠️ Development Steps
1. **Set up MongoDB container:**  
Pull the official MongoDB Docker image 🐳 and run it in detached mode. Map the default MongoDB port (27017) to the host machine. Configure the container with a root username and password (admin). Connect the container to a Docker network named `mongo-network` 🌐. After running, the MongoDB container will run in the background 💤.


2. **Set up Mongo Express container:**  
Pull the official Mongo Express Docker image 🐳 and run it in detached mode. Map the default Mongo Express port (8081) to the host. Configure it with the same MongoDB admin credentials and connection URL to link it with the MongoDB container. Connect it to the same Docker network (`mongo-network`) 🌐. This container will also run in the background 💤.


3. **Create a Dockerfile for the Node.js app:**  
Write a Dockerfile 📄 that defines the environment to run the Node.js application. This includes setting the base image, copying application files, installing dependencies, and exposing the app port 🚪.


4. **Build the Node.js app Docker image:**  
Build a Docker image 🖼️ from the Dockerfile and tag it appropriately for your Docker Hub repository 🏷️.


5. **Push the image to Docker Hub:**  
Log in to your Docker Hub account 🔐, tag your local image with your Docker Hub repository name 🏷️, and push the image to the remote repository 📤.


6. **Run the Node.js app container:**  
Run the built image in detached mode 💤, mapping the app port (default 3000) to the host. Attach this container to the existing Docker network `mongo-network` 🌐 so it can communicate with MongoDB 🛢️.

---

## Author

**Prushti Kathrotiya** ✨
