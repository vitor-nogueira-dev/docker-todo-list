# criando a imagem com base na imagem node:14
FROM node:14-alpine AS todobackend

# definindo a porta de exposição
EXPOSE 3001

# diretório de trabalho
WORKDIR /app

# adicionando o arquivo node_modules (descompactado) a imagem (o ADD descompacta e adiciona ao mesmo tempo)
ADD node_modules.tar.gz .

# copiando tudo para a imagem
COPY . .

# aqui executa sempre que inicia, e não pode ser sobreescrito
ENTRYPOINT [ "npm" ]

# vai executar quando iniciar, mas pode ser sobreescrito
CMD [ "start" ]
