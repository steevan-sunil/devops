Use an official base image
FROM alpine:latest

For Node.js apps:
FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
CMD ["npm", "start"]

# For Python apps:
# FROM python:3.9-slim
# WORKDIR /app
# COPY requirements.txt ./
# RUN pip install -r requirements.txt
# COPY . .
# CMD ["python", "app.py"]

# Minimal working example:
RUN echo "Hello from Docker" > /message.txt
CMD ["cat", "/message.txt"]
