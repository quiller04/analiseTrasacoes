# 🚀 Analisador de Transações com OpenAI GPT  

Este projeto implementa uma integração da API do GPT da OpenAI com Python para analisar transações financeiras, identificar possíveis fraudes e fornecer recomendações sobre ações a serem tomadas.  

## ✨ Funcionalidades  

### ✅ Análise de Transações  
- Processa um conjunto de transações a partir de um arquivo CSV.  
- Identifica transações suspeitas com base em critérios de fraude, como valores discrepantes e locais distantes.  
- Adiciona um atributo `"status"` à transação, indicando se deve ser **"Aprovada"** ou marcada como **"Possível Fraude"**.  

### ✅ Geração de Parecer  
- Para transações sinalizadas como **"Possível Fraude"**, gera um parecer explicando os motivos da suspeita.  
- Se a transação for **"Aprovada"**, o parecer retorna **"Não Aplicável"**.  

### ✅ Recomendações de Ação  
- Com base no parecer gerado, o sistema sugere as seguintes ações:  
  - **Notificar Cliente** 📢  
  - **Acionar setor Anti-Fraude** 🔍  
  - **Realizar Verificação Manual** 📝  
- Classifica o tipo de fraude, se aplicável.  

## 🔧 Tecnologias Utilizadas  

- **Python** 🐍  
- **OpenAI API (GPT-4)** 🤖  
- **dotenv** (para gerenciamento seguro de credenciais)  
- **Manipulação de arquivos JSON e CSV** 📂  

## ⚙️ Como Usar  

### 1️⃣ Clone o repositório:  
```bash
git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/quiller04/analiseTrasacoes.git)
cd seu-repositorio
2️⃣ Instale as dependências:
bash
Copiar
Editar
pip install -r requirements.txt
3️⃣ Configure sua chave da OpenAI criando um arquivo .env:
ini
Copiar
Editar
OPENAI_API_KEY=sua-chave-aqui
4️⃣ Execute o analisador de transações:
bash
Copiar
Editar
python analisador_transacoes.py
