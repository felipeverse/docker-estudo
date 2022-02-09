# Definição para usar a imagem golang versão 1.14 como base
FROM golang:1.14

# Copia todos os arquivos do diretório do Dockerfile e irá colar dentro da imagem gerada
COPY . .

# Gera o executável do arquivo go
RUN go build main.go

# Expoe a porta 8080 para comunicação com outros containers
EXPOSE 8080

# Define que ao iniciar container será executado o arquivo main.go gerado pelo comando RUM
ENTRYPOINT ["./main"]