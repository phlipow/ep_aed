# Use a imagem oficial do Debian como base
FROM debian:buster

# Define o ambiente de trabalho
WORKDIR /app

# Atualiza o sistema e instala as ferramentas necessárias
RUN apt-get update && apt-get install -y \
    build-essential \  # Ferramentas essenciais para compilação
    gdb \             # Depurador
    gcc \             # Compilador C
    valgrind \        # Ferramenta para detecção de vazamento de memória
    git \             # Sistema de controle de versão
    vim \             # Editor de texto
    curl \            # Ferramenta para transferência de dados
    wget              # Ferramenta para download de arquivos da web

# Copia o diretório atual para o contêiner
COPY . .

# Define o comando padrão para executar quando iniciar o contêiner
CMD ["bash"]
