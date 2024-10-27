Para instalar a versão mais recente do Go no Ubuntu, você pode seguir os passos abaixo:
1. Remover Versões Anteriores do Go

Se você já tiver uma versão anterior do Go instalada, é uma boa prática removê-la antes de instalar a nova versão. Execute:

bash

sudo apt remove golang-go

2. Baixar a Versão Mais Recente do Go

Visite a página de lançamentos do Go no GitHub para obter o link da versão mais recente: Go Releases. Você pode usar o wget para baixar o arquivo tar.gz da versão mais recente. Por exemplo:

bash

wget https://golang.org/dl/go1.21.5.linux-amd64.tar.gz

(Substitua 1.21.5 pela versão mais recente disponível.)
3. Extrair o Arquivo Baixado

Extraia o arquivo baixado para o diretório /usr/local:

bash

sudo tar -C /usr/local -xzf go1.21.5.linux-amd64.tar.gz

4. Configurar o PATH

Adicione o diretório do Go ao seu PATH. Abra o arquivo ~/.bashrc ou ~/.profile no seu editor de texto favorito:

bash

nano ~/.bashrc

Adicione a seguinte linha ao final do arquivo:

bash

export PATH=$PATH:/usr/local/go/bin

Salve e feche o arquivo. Para aplicar as mudanças, execute:

bash

source ~/.bashrc

5. Verificar a Instalação do Go

Para confirmar que o Go foi instalado corretamente, verifique a versão com o seguinte comando:

bash

go version
