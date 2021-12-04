# CROMAI teste para Desenvolvedor 
📜 Este projeto tem como objetivo a realização do teste para Pessoa Desenvolvedora de Software Jr.
Neste repositório estão localizadas 3 arquivos:  
    1. ```app.py``` aplicação de desenvolvimento para cálculo da relação de triângulos retângulo, o Teorema de Pitágoras.
    
    2. ```Procfile``` responsável por parâmetros de inialização do heroku ao realizar deploy. 
    
    3. ```requirements.txt``` responsável pelas bibliotecas necessária para rodar a aplicação

#### Ferramentas utilizadas:
- Flask: para a construção da API;
- Heroku: para deplou da API;
- Gunicorn: para realização da interface Gateway http via Python;

<!--

## Utilizando a API
1. Autentique o usuário:
    ```python
    import requests
         
    login = {"username": "admin", "password": "admin"}
    url_auth = 'http://localhost:8000/api/token/'
           
    response = requests.post(url_auth, json=login)
    autorize = f'Bearer {response.json()["access"]}'
    ```
2. Envie os dados pelo método POST:
    ```python
   
   # converte moeda
    data = {
        "precosBRL": [
            "R$ 25,88",
            "R$ 29,88",
        ],
        "moedas": [
            "EUR",
        ]
    }
    url = 'http://127.0.0.1:8000/v1/convertemoeda'
    result = requests.post(url=url, headers={"Authorization": autorize}, json=data)
   
   # ordenação geográfica
   data = {
    "plano": [100, 100],
    "posicaoCliente": [50, 50],
    "lojas": [
        [40,88],
        [18, 56],
        [99, 2]
    ]
    }
    url = 'http://127.0.0.1:8000/v1/ordenacaogeografica'
    result = requests.post(url=url, json=data)
    ```

## 💻 Configuração para Desenvolvimento

### Programas necessários
Segue a lista de coisas que você precisa configurar em sua máquina para utilizar este repositório:

1. Python 3  (se você estiver usando Linux, é provável que já esteja instalado. Execute o comando python3 -V para verificar)
2. Pip  (o instalador de pacote Python padrão)
3. Docker e Docker Compose.


### Para utilizar este repositório
1. Fazer um clone da aplicação:
    ```shell
    git clone git@github.com:ravellys/SBF_teste.git
    ```
2. Instale as bibliotecas necessárias:
    ```shell
    pip install requirements.txt
    ```
3. Inicializar Docker
    ```shell
    docker-compose up -d
    ```
4. Realizar migrações
    ```shell
    docker-compose exec web python manage.py migrate
   ```
6. Criar superusuário que será utilizado nos testes:
    ```shell
    docker-compose exec web python manage.py createsuperuser 
   ursername=admin 
   email=admin@admin.com 
   password=admin 
   password=admin 
   Y   
    ```    
7. Realizar testes:
    ```shell
    docker-compose exec web pytest project/tests_auth_jwt.py
    docker-compose exec web pytest apps/convertemoeda/tests.py
    docker-compose exec web pytest apps/ordenacaogeografica/tests.py
    ```   

## 🗃 Histórico de lançamentos

* 30/05/2021 Criação do Projeto


## 📋 Meta

Lucas Ravelllys – [Portifólio](https://ravellys.github.io)
Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.


## 🚀 Contribuições

1. Faça o _fork_ do projeto (<https://github.com/ravellys/crud-cliente/fork>)
2. Crie uma _branch_ para sua modificação (`git checkout -b feature/fooBar`)
3. Faça o _commit_ (`git commit -am 'Add some fooBar'`)
4. _Push_ (`git push origin feature/fooBar`)
5. Crie um novo _Pull Request_
