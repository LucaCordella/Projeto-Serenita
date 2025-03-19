# **Serenità**

> **Aplicativo/Site para gerenciamento, monitoramento e mapeamento da saúde mental.**

![Black and Beige Minimalist Aesthetic Modern Simple Typography Agency Logo (1)](https://github.com/user-attachments/assets/fcd8ab24-fd52-44f4-b022-003463fe21a3)

---

## **Índice**

1. [Visão Geral do Projeto](#visão-geral-do-projeto)  
2. [Objetivos e Público-Alvo](#objetivos-e-público-alvo)  
3. [Funcionalidades Principais](#funcionalidades-principais)  
4. [Arquitetura e Tecnologias](#arquitetura-e-tecnologias)  
5. [Instalação e Configuração](#instalação-e-configuração)  
6. [Como Usar](#como-usar)  
7. [Protótipo e UX/UI](#protótipo-e-uxui)  
8. [Diagramas](#diagramas)  
9. [Roadmap e Tarefas Futuras](#roadmap-e-tarefas-futuras)  
10. [Contribuição](#contribuição)  
11. [Licença](#licença)  
12. [Contato](#contato)

---

## **Visão Geral do Projeto**

O **Serenità** é um aplicativo/site focado em **gerenciar e monitorar a saúde mental** dos usuários. Ele oferece recursos para registro de humor, sintomas, testes psicológicos simples e visualização de relatórios e tendências emocionais. Com isso, o projeto busca **auxiliar no autoconhecimento**, oferecer **apoio psicológico** e promover o **bem-estar** de seus usuários.

> **Por que “Serenità”?**  
> O nome vem do italiano e significa “serenidade”, transmitindo uma sensação de calma, equilíbrio e bem-estar mental.

---

## **Objetivos e Público-Alvo**

- **Objetivo Principal:**  
  Ajudar usuários a **monitorar** seu bem-estar emocional, **identificar padrões** e **adotar hábitos saudáveis**.

- **Público-Alvo:**  
  - Pessoas interessadas em melhorar sua saúde mental.  
  - Principalmente universitários e pessoas jovens que buscam equilíbrio emocional.

- **Problema Resolvido:**  
  Falta de ferramentas **acessíveis** e **intuitivas** para acompanhamento da saúde mental.

---

## **Funcionalidades Principais**

1. **Diário de Humor:**  
   - Registro diário do estado emocional com emojis ou escalas de humor.  
2. **Registro de Sintomas:**  
   - Espaço para anotar sentimentos, pensamentos ou eventos impactantes.  
3. **Tendências e Relatórios:**  
   - Gráficos que mostram a evolução emocional ao longo do tempo.  
4. **Testes Psicológicos Simples:**  
   - Questionários baseados em escalas de ansiedade, estresse e depressão.  
5. **Gerenciamento e Autocuidado:**  
   - Tarefas diárias, hábitos saudáveis, meditações guiadas, exercícios de respiração.  
6. **Rede de Apoio e Comunidade:**  
   - Lista de contatos de confiança, números de emergência e fórum anônimo para trocas.  
7. **Segurança e Privacidade:**  
   - Bloqueio com senha/biometria, modo emergência, exportação de dados.  
8. **Sistema de Recompensas (Gamificação):**  
   - Incentivos para manter o acompanhamento regular.  

---

## **Arquitetura e Tecnologias**

O projeto segue uma arquitetura **Client-Server** com separação entre **Front-end** e **Back-end**:

- **Front-end**  
  - **HTML5**, **CSS3**, **JavaScript**  
  - **ReactJS** (ou outra biblioteca como Vue.js/Angular)  
  - **Bootstrap** ou **Tailwind CSS** para estilização responsiva

- **Back-end**  
  - **Python com Django** + **Django REST Framework**  
  - **Banco de Dados**: PostgreSQL (produção) / SQLite (desenvolvimento inicial)

- **Infraestrutura e DevOps**  
  - **Docker** para containerização  
  - **Git** para versionamento  
  - **GitHub Actions** / GitLab CI para integração contínua

### **Requisitos Não Funcionais Importantes**  
- **Responsividade:** Compatível com desktop, tablet e smartphone  
- **Segurança:** Proteção de dados, conformidade com LGPD/GDPR  
- **Acessibilidade:** Segue as diretrizes WCAG 2.1  
- **Escalabilidade:** Suporta um grande número de usuários  
- **Testabilidade:** Testes unitários e de integração

---

## **Instalação e Configuração**

### **1. Pré-Requisitos**

- **Python 3.8+**  
- **Node.js 14+** (se for usar React ou outra biblioteca JS)  
- **Git** instalado  
- **Docker** (opcional, caso queira usar container)

### **2. Clonando o Repositório**

```bash
git clone https://github.com/seu-usuario/serenita.git
cd serenita
```

### **3. Configurando o Back-end (Django)**

1. Crie e ative um **ambiente virtual** (recomendado):
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
3. Configure o **banco de dados** no `settings.py` (ex.: PostgreSQL ou SQLite).  
4. Rode as migrações:
   ```bash
   python manage.py migrate
   ```
5. Inicie o servidor local:
   ```bash
   python manage.py runserver
   ```

### **4. Configurando o Front-end (React, Exemplo)**

1. Entre na pasta do front-end:
   ```bash
   cd frontend
   ```
2. Instale as dependências:
   ```bash
   npm install
   ```
3. Inicie a aplicação:
   ```bash
   npm start
   ```
4. Acesse em `http://localhost:3000` (ou porta configurada).

---

## **Como Usar**

1. **Cadastro/Login:** Acesse a página principal para criar uma conta ou fazer login.  
2. **Painel de Monitoramento:**  
   - Registre seu humor no Diário de Humor.  
   - Adicione sintomas ou eventos importantes.  
3. **Tendências e Relatórios:**  
   - Acompanhe gráficos de evolução emocional.  
4. **Testes Psicológicos:**  
   - Responda questionários para avaliar ansiedade, estresse e depressão.  
5. **Rede de Apoio e Comunidade:**  
   - Liste contatos de emergência e compartilhe experiências anonimamente.  
6. **Segurança e Exportação de Dados:**  
   - Habilite bloqueio com senha/biometria e exporte seus registros em PDF ou CSV.

---

## **Protótipo e UX/UI**

- **Figma:**  
  - Protótipo principal: [Link para o Figma](https://www.figma.com/board/LDCBPR0Jz721etm4GXQ4bf/Prot%C3%B3tipo-do-Projeto?node-id=0-1&t=t3953wPMupVoPPak-1)

**Imagem de Exemplo:**  
> ![image](https://github.com/user-attachments/assets/f19fa834-3c88-459f-9c9a-27faed646707)

---

## **Diagramas**

Para uma melhor compreensão do projeto, acesse os diagramas na pasta [`/docs`](./docs/) do repositório:

1. **Diagrama de Ishikawa (Espinha de Peixe):**  
   ![Diagrama Espinha de Peixe - PS](https://github.com/user-attachments/assets/0aa41bd5-65af-47f7-8649-d7e8dbb17826)

2. **Diagrama de Caso de Uso:**  
   - [Link do Diagrama](#)

3. **Diagrama de Classes:**  
   - [Link do Diagrama](#)

4. **Diagrama de Atividades:**  
   - [Link do Diagrama](#)

---

## **Roadmap e Tarefas Futuras**

- **v1.0 (MVP)**  
  - [x] Cadastro e Login de Usuários  
  - [x] Registro de Humor e Sintomas  
  - [x] Visualização de Tendências e Relatórios  
  - [ ] Testes Psicológicos Simples  
  - [ ] Rede de Apoio Básica  
  - [ ] Exportação de Dados

- **v2.0**  
  - [ ] Gamificação e Sistema de Recompensas  
  - [ ] Comunidade Anônima Integrada  
  - [ ] IA para Análise de Sentimentos (em estudo)  
  - [ ] Integração com Dispositivos (Wearables)

---

## **Contribuição**

1. **Fork** o repositório  
2. Crie uma **branch** com a feature ou correção: `git checkout -b feature/sua-feature`  
3. Faça **commit** das alterações: `git commit -m 'Adiciona nova feature'`  
4. Faça **push** para a branch: `git push origin feature/sua-feature`  
5. Abra um **Pull Request** no GitHub

---

## **Licença**

Este projeto está sob a licença [MIT](LICENSE.md) - sinta-se à vontade para usar e modificar como desejar. Leia o arquivo `LICENSE.md` para mais detalhes.

---

## **Contato**

- **Autor:** Luca Cordella (https://github.com/LucaCordella)  
- **E-mail:** lucacordella12@gmail.com  
- **LinkedIn:** [linkedin.com/in/lucacordella](https://linkedin.com/in/lucacordella)

> *Se tiver dúvidas ou sugestões, fique à vontade para abrir uma [issue](./issues) ou entrar em contato!*

---

### **Referências**

- [Documento do Projeto Serenità (PDF)](#)  
- [Repositório de Documentação](#)  
- [Site Oficial da Organização Mundial da Saúde (OMS)](https://www.who.int/)  
- [Ministério da Saúde (gov.br)](https://www.gov.br/saude/pt-br)

