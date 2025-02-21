# ETL com a API do GitHub

Este repositório contém um projeto de ETL (Extract, Transform, Load) utilizando a API do GitHub. O objetivo do projeto é coletar dados sobre os repositórios de algumas empresas, transformá-los e armazená-los de forma estruturada.

Este trabalho faz parte da **formação de Engenharia de Dados da Alura**.

## 📌 Funcionalidades

- Extração de informações sobre repositórios públicos utilizando a API do GitHub.
- Transformação dos dados em um formato estruturado (DataFrame pandas).
- Armazenamento dos dados em arquivos CSV.
- Automação da criação de repositórios no GitHub e upload de arquivos.

## 🛠️ Tecnologias Utilizadas

- **Python**
- **Bibliotecas:** `requests`, `pandas`, `dotenv`, `base64`
- **API do GitHub**

## 📂 Estrutura do Projeto

```
📦 ETL_GitHub
├── 📄 ETL.py              # Script para extração e transformação dos dados
├── 📄 Salvando.py         # Script para criação de repositório e upload dos dados
├── 📄 .env.example       # Exemplo de configuração do arquivo .env
├── 📂 dados              # Pasta onde os arquivos CSV serão armazenados
└── 📄 README.md          # Documentação do projeto
```

## ⚠️ Configuração e Segurança

Para evitar a exposição de credenciais, o projeto utiliza variáveis de ambiente para armazenar o **token de acesso do GitHub**. Antes de executar o código, crie um arquivo `.env` na raiz do projeto e adicione:

```
GITHUB_TOKEN=seu_token_aqui
```

🚨 **Importante:** Nunca exponha seu token no código-fonte público! O arquivo `.env` deve estar no `.gitignore` para não ser versionado.

## 🚀 Como Executar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu_usuario/ETL_GitHub.git
   cd ETL_GitHub
   ```
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
3. Configure o arquivo `.env` conforme descrito acima.
4. Execute o script de ETL:
   ```bash
   python ETL.py
   ```
5. Execute o script de upload para criar o repositório e enviar os dados:
   ```bash
   python Salvando.py
   ```

## 📌 Melhorias Futuras

- Adicionar um banco de dados para armazenamento dos dados coletados.
- Implementar logging para melhor monitoramento da execução.
- Criar um dashboard para visualização dos dados coletados.

## 📄 Licença

Este projeto está licenciado sob a **MIT License** - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---
📌 **Autor:** Leonardo Koide  
📌 **Formação:** Engenharia de Dados - Alura

