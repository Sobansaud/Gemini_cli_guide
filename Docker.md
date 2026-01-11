
### CODEVERSE SOBAN 
# 🚀 Next.js Application → Docker Image → Docker Hub (Step by Step)


In this Video :-
1. Create a Next.js application  
2. Build a Docker image  
3. Push the image to Docker Hub  
4. Run the application using Docker  

---

## ✅ Prerequisites
- Node.js installed
- Docker Desktop installed and running
- Docker Hub account

---

## 📁 Step 1: Create a Next.js Application

```bash
npx create-next-app@latest nextjs-app
cd nextjs-app
```

Run the project locally to verify:

```bash
npm run dev
```

Open in browser:
```
http://localhost:3000
```

---

## 🐳 Step 2: Create a Dockerfile

Create a file named `Dockerfile` in the project root:

```dockerfile
FROM node:18-alpine

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]
```

---

## 🔐 Step 3: Login to Docker Hub

```bash
docker login
```

Enter your Docker Hub username and password.

---

## 🏗️ Step 4: Build the Docker Image

```bash
docker build -t sobansaud121/nextjs_website .
```

---

## ▶️ Step 5: Run the Docker Container

```bash
docker run -p 3000:3000 sobansaud121/nextjs_website
```

Open in browser:
```
http://localhost:3000
```

---

## ☁️ Step 6: Create Repository on Docker Hub

On Docker Hub:
- Repository Name: `nextjs_website`
- Owner: `sobansaud121`
- Visibility: Public

---

## ⬆️ Step 7: Push Image to Docker Hub

```bash
docker push sobansaud121/nextjs_website
```

---

## ⬇️ Step 8: Pull and Run Image from Docker Hub

```bash
docker pull sobansaud121/nextjs_website
docker run -p 3000:3000 sobansaud121/nextjs_website
```

---

## 🎉 Done!
Your **Next.js application is now running using Docker** 🚀

---

## ❤️ Support the Channel

**CodeVerse Soban**  
👍 Like the video  
🔁 Share with others  
🔔 Subscribe for more content  
