FROM nginx:latest

# Diretório de trabalho
# Cria o diretório e posiciona nele
WORKDIR /app

RUN apt-get update && \
    apt-get install vim -y

# copia o diretório local html para o diretório do container /usr/share/nginx
COPY html /usr/share/nginx/html

ENTRYPOINT ["/docker-entrypoint.sh"]

CMD ["nginx", "-g", "daemon off;"]