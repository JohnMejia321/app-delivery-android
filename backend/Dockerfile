# Selecciona la imagen base
FROM node:14

# Crea el directorio de la aplicación en el contenedor
WORKDIR /usr/src/app

# Copia los archivos del paquete.json y el paquete-lock.json
COPY package*.json ./

# Instala las dependencias del proyecto
RUN npm install

# Copia el resto de los archivos de la aplicación al contenedor
COPY . .

# Expone el puerto que tu aplicación utilizará
EXPOSE 3000

# Comando para iniciar la aplicación
CMD [ "node", "server.js" ]
