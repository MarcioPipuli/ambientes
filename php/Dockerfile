FROM ubuntu:latest

#atualiza os repositórios
RUN apt update && apt upgrade -y

#instala o PHP 7.4 no container (php 8.0 não está no repositório padrão do UBUNTU)
RUN apt install php7.4-cli php7.4-mysql pdo-mysql -y

#instala o editor no container
RUN apt install vim -y

#abre o bash no diretório /tmp
WORKDIR "/php"

VOLUME [ "/php" ]

ENTRYPOINT ["bash"]
