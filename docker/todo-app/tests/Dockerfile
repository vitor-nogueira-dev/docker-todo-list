# criando a imagem com base na imagem node:14
FROM mjgargani/puppeteer:trybe1.0 AS todotests

# adicionando o arquivo node_modules (descompactado) a imagem (o ADD descompacta e adiciona ao mesmo tempo)
ADD node_modules.tar.gz .

# copiando tudo para a imagem
COPY . /app

# diretório de trabalho
WORKDIR /app

# aqui executa sempre que inicia, e não pode ser sobreescrito
ENTRYPOINT [ "npm" ]

# vai executar quando iniciar, mas pode ser sobreescrito
CMD [ "test" ]
