# CROMAI teste para Desenvolvedor 
📜 Este projeto tem como objetivo a realização do teste para Pessoa Desenvolvedora de Software Jr.
Neste repositório estão localizadas 3 arquivos:
1. ```app.py``` :aplicação de desenvolvimento para cálculo da relação de triângulos retângulo, o Teorema de Pitágoras.
    
2. ```Procfile``` :responsável por parâmetros de inialização do heroku ao realizar deploy. 
    
3. ```requirements.txt``` :responsável pelas bibliotecas necessária para rodar a aplicação.

#### Ferramentas utilizadas:
- Flask: para a construção da API;
- Heroku: para deplou da API;
- Gunicorn: para realização da interface Gateway http via Python;



## Utilizando a API
1. Acesse o local o ambiente de alocação da API:
    ```
    link = 'https://api-pitagoras-ederreis.herokuapp.com/'
    ```
2. Defina o método a calcular sabendo dois dos lados de triângulo retângulo:
 - ```calcular_hipotenusa``` : resultará no valor da hipotenusa dados os dois catetos.
 - ```calcular_cateto``` : resultará no valor de um dos catetos dados um cateto e a hipotenysa.
 
3. Cálculo para valor da hipotenusa:
 - ```link = 'https://api-pitagoras-ederreis.herokuapp.com/calcular_hipotenusa/valor1/valor2'```
 - Onde ```valor1``` e ```valor2``` são valores númericos dos catetos aplicados na método, que retornará a relação dos lados do triângulo retângulo em ```json```.

4. Cálculo para valor de um dos catetos:
- ```link = 'https://api-pitagoras-ederreis.herokuapp.com/calcular_cateto/valor1/valor2'```
-  Onde ```valor1``` e ```valor2``` são valores númericos de um dos catetos e a hipotenusa - dependendo do relação de valor (hipotenusa > cateto) aplicados no método, que retornará a relação dos lados do triângulo retângulo em ```json```.

## Aplicação front-end:
Também como parte desse projeto, foi criado uma aplicação utilizando **React.js**, cujo dados consumidos requisitam esta Api.Também, aqui o deploy foi realizado através do Heroku.
 - link da aplicação: <https://calculadora-react-ederreis.herokuapp.com/>
 - link repositório da aplicação: <https://github.com/EderReisS/calculadora-react>


💻 Configuração para Desenvolvimento

### Programas necessários
Segue a lista de coisas que você precisa configurar em sua máquina para utilizar este repositório:

1. Python 3  (se você estiver usando Linux, é provável que já esteja instalado. Execute o comando python3 -V para verificar)
2. Pip  (o instalador de pacote Python padrão)
3. Editor de código (exemplo vscode, PyCharm, Jupyter,etc.)

### Para utilizar este repositório
1. Fazer um clone da aplicação:
    ```shell
    git clone https://github.com/EderReisS/API_CALCULAR_HIPOTENUSA.git
    ```
2. Instale as bibliotecas necessárias:
    ```shell
    pip3 install requirements.txt
    ```
3. Inicializar api no ambiente local de desenvolvimento:
    ```shell
    python3 app.py
    ```

## 🗃 Histórico de lançamentos

* 02/12/2021 Criação do Projeto


## 🚀 Contribuições

1. Faça o _fork_ do projeto (<https://github.com/EderReisS/API_CALCULAR_HIPOTENUSA/fork>)
2. Crie uma _branch_ para sua modificação (`git checkout -b feature/fooBar`)
3. Faça o _commit_ (`git commit -am 'Add some fooBar'`)
4. _Push_ (`git push origin feature/fooBar`)
5. Crie um novo _Pull Request_
