#imagem base do Gentoo Linux
FROM gentoo/stage3
# Atualize os repositórios e instale as atualizações
RUN emerge --sync && emerge --update --deep --with-bdeps=y --newuse @world

#variáveis de ambiente
ENV LANG pt_BR.UTF-8
ENV LC_ALL pt_BR.UTF-8

# Configurações adicionais, se necessário

# Limpeza para reduzir o tamanho final da imagem
RUN emerge --depclean && eclean-dist -d && rm -rf /var/cache/distfiles/*

# Execute o comando padrão ao iniciar o contêiner (se necessário)
CMD ["bash"]
