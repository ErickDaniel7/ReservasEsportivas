### Sistema de Aluguel de Quadras Esportivas

Este sistema visa modernizar e otimizar o processo de gerenciamento de reservas de campos esportivos. Desenvolvido com Flask para o backend e Angular para o frontend, o sistema permite que donos de campos e clientes gerenciem e agendem horários para esportes como futebol, tênis e vôlei, de maneira eficiente e prática.

<details><summary><h3>Instruções Front End</h3></summary>
  
Este projeto foi gerado com [Angular CLI](https://github.com/angular/angular-cli) versão 18.2.5.

## Servidor de desenvolvimento

Execute `ng serve` para iniciar um servidor de desenvolvimento. Acesse `http://localhost:4200/`. A aplicação será recarregada automaticamente se você alterar qualquer um dos arquivos de origem.

## Criação de código

Execute `ng generate component component-name` para gerar um novo componente. Você também pode usar `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build (Construção)

Execute `ng build` para construir o projeto. Os artefatos de construção serão armazenados no diretório `dist/` .

## Executando testes unitários

Execute `ng test` para executar os testes unitários via [Karma](https://karma-runner.github.io).

## Executando testes de ponta a ponta

Execute `ng e2e` para executar os testes de ponta a ponta usando uma plataforma de sua escolha. Para usar este comando, é necessário primeiro adicionar um pacote que implemente recursos de teste de ponta a ponta.

## Ajuda adicional

Para obter mais ajuda sobre o Angular CLI, use `ng help` ou consulte a página [Visão Geral e Referência de Comandos do Angular CLI.](https://angular.dev/tools/cli).

</details>
<details>
  <summary><h3>Instruções Back End</h3></summary>

  # **Sistema de Aluguel de Quadras**

Este é um sistema desenvolvido em Flask para gerenciar o aluguel de quadras esportivas.

## **Pré-requisitos**

* **Git:** Para clonar o repositório.
* **Python 3.8.10** ou superior.
* **Virtualenv:** Para criar um ambiente virtual isolado para o projeto.

## **Instalação**

### **1. Clonar o Repositório**

```bash
git clone https://github.com/vagnersantosdasilva/aluguel-quadras.git
cd aluguel-quadras  # Acesse o diretório do projeto
```

### **2. Criar e Ativar o Ambiente Virtual**

* No **Linux/macOS**:
  ```bash
  python3 -m venv venv  # Cria um ambiente virtual
  source venv/bin/activate  # Ativa o ambiente virtual
  ```

* No **Windows**:
  ```bash
  python -m venv venv
  venv\Scripts\activate  # Ativa o ambiente virtual
  ```

### **3. Instalar as Dependências**

```bash
pip install -r dependencias.txt  # Instala as dependências listadas
```

### **4. Configurar o Ambiente**

1. **Criar o arquivo `.env`**: Na raiz do projeto, crie um arquivo `.env` e adicione as variáveis de ambiente necessárias:

```bash
LOCACAO_MONITOR_INTERVAL=15  # Intervalo para verificar locações canceladas
PAGAMENTO_MONITOR_INTERVAL=10  # Intervalo para verificar pagamentos pendentes
SGBD=mysql+mysqlconnector
DB_USER=seu_usuario
DB_PASSWORD=sua_senha
DB_HOST=seu_host
DB_NAME=nome_do_banco

MAIL_SERVER=smtp-relay.sendinblue.com
MAIL_PORT=587
MAIL_USE_TLS=True
MAIL_USE_SSL=False
MAIL_USERNAME=seu_email
MAIL_PASSWORD=sua_senha
MAIL_DEFAULT_NAME="Sistema de Aluguel de Quadras"
MAIL_DEFAULT_EMAIL=seu_email_padrao
```

2. **Configurar o banco de dados**: Crie o banco de dados e certifique-se de que as credenciais estejam corretas no arquivo `config.py`.

### **5. Executar a Aplicação**

Com o ambiente virtual ativado e as configurações corretas, execute a aplicação com o seguinte comando:

```bash
flask run
```

A aplicação estará acessível em `http://127.0.0.1:5000/`.

## **Funcionalidades**

* **Gerenciamento de usuários:** Cadastro
* **Gerenciamento de quadras:** Criação, edição e exclusão de quadras.
* **Agendamento de locações:** Reservas de quadras em horários disponíveis.
* **Monitoramento de listas de espera**
* **Controle de reservas para horários concorridos**
* **Envio de notificações por email**
* **Monitoramento de pagamentos:** Controle de pagamentos pendentes e confirmados.

</details>
