# 🛠️ Projeto ETL com Python e Requests  

Este projeto implementa um pipeline ETL (Extração, Transformação e Carga) utilizando Python. O objetivo é extrair dados de uma API REST, transformá-los para atender às necessidades do negócio e armazená-los em um banco de dados relacional para futuras análises.  

---

## 📋 Funcionalidades  

- **Extração**: Realiza requisições HTTP para obter dados de uma API REST usando a biblioteca `requests`.  
- **Transformação**: Processa e estrutura os dados brutos, incluindo limpeza, filtragem e formatação.  
- **Carga**: Insere os dados transformados em um banco de dados relacional.  

---

## 🛠️ Tecnologias Utilizadas  

- **Python**: Linguagem de programação principal.  
- **Requests**: Para comunicação com a API REST.  
- **Pandas**: Manipulação e transformação dos dados.  
- **SQLAlchemy**: Interface para conexão com o banco de dados.  
- **SQLite**: Banco de dados relacional utilizado (pode ser substituído por outro).  

---

## 📂 Estrutura do Projeto  

```plaintext  
etl_project/  
│  
├── README.md            # Documentação do projeto  
├── requirements.txt     # Dependências do projeto  
├── config.py            # Configurações (URL da API, credenciais, etc.)  
├── extract.py           # Módulo de extração de dados  
├── transform.py         # Módulo de transformação de dados  
├── load.py              # Módulo de carga de dados  
├── database/            # Diretório para arquivos do banco de dados  
│   └── etl_data.db      # Banco de dados SQLite  
└── main.py              # Script principal para executar o pipeline  

⚙️ Configuração
1. Pré-requisitos

    Python 3.8 ou superior.
    Gerenciador de pacotes pip.

2. Instalação

    Clone o repositório:
    git clone https://github.com/seu-usuario/seu-repositorio.git 
    cd etl_project  

3. Configure o arquivo config.py com:

    A URL da API.
    Parâmetros de autenticação (se necessários).
    Detalhes do banco de dados.

🚀 Como Executar

    Execute o script principal:
    python main.py  

1. O pipeline será executado nas seguintes etapas:

    Extração: Os dados são coletados da API.
    Transformação: Os dados são limpos e ajustados.
    Carga: Os dados são inseridos no banco de dados. 

🛠️ Personalização

    Fonte de Dados: Atualize a URL da API no arquivo config.py.
    Transformações Específicas: Modifique as funções em transform.py.
    Banco de Dados: Substitua o SQLite por outro banco (ex.: MySQL, PostgreSQL) configurando config.py.

🤝 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

📝 Licença

Este projeto está licenciado sob a MIT License.

Essa versão possui uma melhor separação de tópicos, maior clareza e uma estrutura mais limpa para facilitar a navegação e o entendimento. Caso precise de mais ajustes, é só pedir! 😊
