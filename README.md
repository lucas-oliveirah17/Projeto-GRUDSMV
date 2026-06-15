# Projeto-GRUDSMV
## Projeto da disciplina "Desenvolvimento  para Dispositivos Móveis" (GRUDSMV) - IFSP Guarulhos

# Tema 10 — Aplicativo de Chamados Técnicos

## Enunciado do Projeto

Desenvolva um aplicativo mobile para gerenciamento de chamados técnicos em uma organização. O app deve permitir que usuários registrem chamados para suporte técnico informando o problema, o setor e a urgência. Técnicos visualizam os chamados atribuídos a eles e atualizam o status (aberto, em atendimento, resolvido). A aplicação deve registrar datas de abertura e resolução, manter um histórico de status e permitir que administradores visualizem todos os chamados com filtros por responsável ou urgência. O app também implementa regras básicas de SLA com indicadores visuais de prazo.

## 1. Histórias de Usuário

### 🔐 Autenticação e Autorização

- Como visitante, quero me cadastrar com nome, e-mail e senha para poder registrar chamados para suporte técnico
- Como usuário autenticado, quero fazer login e ter meu token JWT persistido para acessar os recursos da API de forma segura
- Como administrador, quero que o app exiba telas e ações diferenciadas conforme o papel (USER, TECHNICIAN, ADMIN) para organizar o fluxo e a triagem dos chamados

### 🆘 Abertura de Chamados

- Como usuário autenticado, quero registrar um chamado técnico com descrição, setor e nível de urgência (seletor) para solicitar suporte em problemas identificados
- Como sistema, quero registrar e exibir automaticamente a data e hora de abertura do chamado para controle do tempo de atendimento
- Como usuário autenticado, quero visualizar meus chamados com seus respectivos status em uma lista para acompanhar o andamento das minhas solicitações

### 🔧 Atendimento Técnico

- Como técnico, quero visualizar a lista de chamados disponíveis ou atribuídos a mim em uma tela dedicada para iniciar o atendimento
- Como técnico, quero atualizar o status do chamado para "em atendimento" ou "resolvido" com seletor visual para indicar o progresso
- Como técnico, quero registrar observações técnicas ou soluções aplicadas ao chamado em um campo de texto para documentar o histórico da intervenção
- Como sistema, quero registrar e exibir a data de resolução quando o chamado for finalizado para cálculo do tempo de atendimento

### 📊 Supervisão e Relatórios

- Como administrador, quero visualizar todos os chamados por status em uma tela de dashboard com contadores para supervisionar o desempenho da equipe técnica
- Como administrador, quero filtrar os chamados por técnico, urgência ou status para facilitar a priorização de atendimentos
- Como administrador, quero identificar visualmente (ex: badge vermelho) os chamados que ultrapassaram o tempo máximo de resposta (SLA) para agir em casos críticos de atraso

## 2. Requisitos de Testes
Testes unitários de regras de negócio para atualização de status, cálculo de SLA e verificação de permissões com Jest

## 3. Extras/Opcionais

- Notificações locais (expo-notifications) para técnicos ao receberem chamados atribuídos
- Tela de dashboard com tempo médio de resposta por técnico em gráfico de barras
- Priorização automática de chamados na listagem com base na urgência e tempo de espera


## 🎓 Autores
- **Daniel Navarro Porto**

  [![GitHub](https://img.shields.io/badge/GitHub-100000?style=plastic&logo=github&logoColor=white)](https://github.com/danielnporto)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=plastic&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/danielnporto/)

- **Lucas Silva de Oliveira**
   
  [![GitHub](https://img.shields.io/badge/GitHub-100000?style=plastic&logo=github&logoColor=white)](https://github.com/lucas-oliveirah17)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=plastic&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lucas-oliveirah17/)

- **Guilherme Dionizio Ludgero**

  [![GitHub](https://img.shields.io/badge/GitHub-100000?style=plastic&logo=github&logoColor=white)](https://github.com/Gludgero)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=plastic&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/guilhermeludgero/)

---
