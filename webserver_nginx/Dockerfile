# Use uma imagem base
FROM nginx:alpine

# Autor
LABEL author="Seu Nome <seu@email.com>"

# Copie os arquivos do servidor web para dentro do contêiner
COPY ./meu_site /usr/share/nginx/html

# Exponha a porta 80 para tráfego web
EXPOSE 80

# Defina o comando padrão a ser executado quando o contêiner for iniciado
CMD ["nginx", "-g", "daemon off;"]