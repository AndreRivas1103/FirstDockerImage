# Usar una imagen base Alpine de Node
FROM node:18-alpine

# Establecer el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copiar los archivos package e instalar dependencias
COPY package*.json ./
RUN npm install

# Copiar el resto del código de la aplicación
COPY . .

# Exponer el puerto de la aplicación
EXPOSE 3000

# Comando para ejecutar Node.js dentro del contenedor
CMD ["node", "app.js"]
