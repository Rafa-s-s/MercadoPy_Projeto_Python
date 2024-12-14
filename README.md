# MercadoPy - Sistema de Gerenciamento de Produtos

O **MercadoPy** é um projeto desenvolvido em Python que simula um sistema de gerenciamento de produtos. Com ele, é possível criar, listar e gerenciar um estoque virtual de forma simples e eficiente. Este projeto é ideal para iniciantes em Python ou para quem deseja aprender mais sobre organização de código em módulos, classes e boas práticas de programação.

---

## Funcionalidades Principais

- **Cadastro de Produtos**: Adicione produtos ao estoque com código, nome e preço.
- **Listagem de Produtos**: Exiba todos os produtos cadastrados de forma organizada e formatada.
- **Busca por Código**: Encontre um produto específico no estoque utilizando seu código único.
- **Formatação de Preços**: Exibição de preços no formato de moeda brasileira (ex.: R$ 1.234,56).

---

## Organização do Projeto

O projeto está estruturado da seguinte forma:

```
MercadoPy/
├── Armazem/                 # Diretório principal para armazenar dados
│   ├── models/              # Modelos principais do projeto
│   │   ├── __init__.py      # Inicialização do módulo
│   │   ├── produto.py       # Classe Produto
│   └── utils/               # Funções utilitárias
│       ├── __init__.py      # Inicialização do módulo
│       ├── helper.py        # Função de formatação de preços
│       ├── mercado.py       # Lógica principal do mercado
│       ├── teste.py         # Arquivo de testes
└── .venv/                   # Ambiente virtual (não incluído no repositório)
```

### **Descrição de Arquivos**

- **`produto.py`**: Define a classe `Produto`, que representa os produtos com atributos como código, nome e preço. Inclui métodos para formatação e exibição de informações.
- **`helper.py`**: Contém funções auxiliares, como a formatação de valores monetários para o padrão brasileiro.
- **`mercado.py`**: Implementa a lógica do sistema, como o cadastro e listagem de produtos.
- **`teste.py`**: Arquivo para testar as funcionalidades do sistema de forma isolada.

---

## Como Executar o Projeto

1. **Clonar o Repositório**:
   ```bash
   git clone https://github.com/seu-usuario/MercadoPy.git
   cd MercadoPy
   ```

2. **Instalar o Ambiente Virtual (Opcional)**:
   ```bash
   python -m venv .venv
   source .venv/bin/activate    # Para Linux/Mac
   .venv\Scripts\activate       # Para Windows
   ```

3. **Executar o Arquivo Principal**:
   ```bash
   python utils/mercado.py
   ```

4. **Rodar os Testes**:
   ```bash
   python utils/teste.py
   ```

---

## Exemplos de Uso

### Cadastro de Produtos
```python
from models.produto import Produto

produto1 = Produto(nome="Arroz", preco=19.99)
print(produto1)
```

### Listagem de Produtos
```python
from utils.mercado import listar_produtos

listar_produtos()
```

---

## Tecnologias Utilizadas

- **Python**: Linguagem de programação principal do projeto.
- **Ambiente Virtual**: `.venv` para isolar as dependências (opcional).

---

## Objetivo do Projeto

O **MercadoPy** foi desenvolvido com o objetivo de praticar conceitos de programação orientada a objetos, modularização e formatação de dados. Além disso, o projeto serve como base para estudos mais avançados, como a integração com bancos de dados e interfaces gráficas.

---

## Próximos Passos

- **Adicionar Integração com Banco de Dados**: Para armazenar produtos de forma persistente.
- **Criar Interface Gráfica**: Para facilitar o uso do sistema.
- **Adicionar Funções de Relatórios**: Como vendas e inventário.

---
## Explicação Interativa do Projeto
Para uma explicação detalhada e interativa do código, incluindo exemplos e a lógica por trás de cada parte, confira o seguinte arquivo:
[Acesse o notebook explicativo do projeto MercadoPy](https://github.com/Rafa-s-s/MercadoPy_Projeto_Python/blob/main/MercadoPy_Explica%C3%A7%C3%A3o.ipynb)

## Download
Baixe a versão mais recente do MercadoPy na seção de [Releases](https://github.com/Rafa-s-s/MercadoPy_Projeto_Python/releases/tag/v1.0.0).

## Licença

Este projeto está licenciado sob a **MIT License**.

---
![MercadoPy _img](https://github.com/user-attachments/assets/3463f750-2ad3-40b1-898d-97bf79bd6a99)
