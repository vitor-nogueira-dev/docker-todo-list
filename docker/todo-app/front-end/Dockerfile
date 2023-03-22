# criando a imagem com base na imagem node:14
FROM node:14-alpine AS todofrontend

# definindo a porta de exposição
EXPOSE 3000

# diretório de trabalho app
WORKDIR /app

# adicionando o arquivo node_modules (descompactado) a imagem (o ADD descompacta e adiciona ao mesmo tempo)
ADD node_modules.tar.gz .

# copiando todos os arquivos . para o diretório app
COPY . .

# executa sempre que inicia, e não pode ser sobreescrito
ENTRYPOINT [ "npm" ]

# executa quando inicia, e pode ser sobreescrito (no terminal)
CMD [ "start" ]
