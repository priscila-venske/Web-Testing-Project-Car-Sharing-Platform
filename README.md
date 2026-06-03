# 🚗 Urban Routes — Web Testing Project · Car Sharing Platform
 
> Projeto de testes de software aplicado à plataforma **Urban Routes**, cobrindo testes de layout, validação de formulários, lógica do botão de reserva e fluxos de locação.
 
---
 
## 📋 Visão Geral
 
Este repositório documenta a execução completa de um ciclo de testes manuais na plataforma web **Urban Routes** (Car Sharing), incluindo checklists de layout, casos de teste funcionais e relatórios de bugs no formato Jira.
 
| Item                    | Detalhe                          |
|-------------------------|----------------------------------|
| **Plataforma**          | Urban Routes – Car Sharing Web   |
| **Navegador**           | Google Chrome                    |
| **Resolução**           | 800 × 600 px                     |
| **Total de itens testados** | 60+                          |
| **Bugs encontrados (REPROVADO)** | 33                    |
| **Itens aprovados**     | 20+                              |
| **Itens bloqueados**    | 5                                |
 
---
 
## 🧪 Escopo dos Testes
 
### Aba 1 — Checklist de Layout
 
Verificação visual da interface em estado inicial, modo Personal, mapa, tarifa Casual, carteira de motorista e pop-up de confirmação.
 
| ID | Descrição resumida | Resultado |
|----|--------------------|-----------|
| L1 | Exibe logotipo Urban.Routes | ✅ APROVADO |
| L2 | Exibe texto "PLATAFORMA" | [❌ REPROVADO](https://drive.google.com/file/d/1a7ka2W9It39bT_AbbbmWpKLf49n0Oysn/view?usp=drive_link) |
| L3 | Botão vermelho (De) e azul (Para) | ✅ APROVADO |
| L4 | Frase "Carshering~$ X Duração: X min" — erro ortográfico e de formatação | ❌ REPROVADO |
| L5 | Layout do botão "Reservar" divergente do especificado | ❌ REPROVADO |
| L6 | Exibe carro azul no modo Personal | ✅ APROVADO |
| L7 | Rota não exibida no mapa | ❌ REPROVADO |
| L8 | Carros azuis não aparecem no mapa após reservar | ❌ REPROVADO |
| L9 | Localização do BMW ausente no mapa (Casual) | ❌ REPROVADO |
| L10 | Exibe modelo de veículo na tarifa Casual | ✅ APROVADO |
| L11 | Exibe frase "Apenas negócios, nada extra" | ✅ APROVADO |
| L12 | Inconsistência visual no texto de tempo/espera (Casual) | ❌ REPROVADO |
| L13 | Ilustração sem frisos na roda/porta dianteira (Casual) | ❌ REPROVADO |
| L14 | Texto de acessórios em letras minúsculas indevidamente | ❌ REPROVADO |
| L15 | Info de km/duração ausente próxima ao botão "RESERVAR" | ❌ REPROVADO |
| L11-CDM | Botão "Adicionar Carteira" sem símbolo ">" | ❌ REPROVADO |
| L12-CDM | Campo sem destaque verde/ícone de verificação após carteira válida | ❌ REPROVADO |
| L13-POP | Pop-up exibe apenas "O carro foi reservado" sem dados completos | ❌ REPROVADO |
| L14-POP | Nome do veículo ausente na confirmação | ❌ REPROVADO |
| L15-POP | Ilustração sem frisos no pop-up de confirmação | ❌ REPROVADO |
| L16-POP | Botão "Cancelar" inativo na tela de confirmação | ❌ REPROVADO |
| L17-POP | Custo não exibido no formato "Custo – $X" | ❌ REPROVADO |
| L18 | Pop-up de cancelamento exibe mensagem correta | 🔒 BLOQUEADO |
| L19 | Mensagem de corrida cancelada exibida corretamente | 🔒 BLOQUEADO |
 
---
 
### Aba 2 — Checklist: Método de Pagamento e Adicionar Cartão
 
Validação dos campos e comportamentos da janela de pagamento.
 
| ID | Descrição resumida | Resultado |
|----|--------------------|-----------|
| P1 | Campo exibido vazio no estado inicial | ✅ APROVADO |
| P2 | Exige ao menos 1 cartão para concluir reserva | ✅ APROVADO |
| P3 | Sem restrição de quantidade de cartões | ✅ APROVADO |
| P4 | Últimos 4 dígitos do cartão não exibidos após adição | ❌ REPROVADO |
| P5 | Botão "Cancelar" fecha janela de cadastro | ✅ APROVADO |
| P6 | Botão "X" fecha janela de cadastro | ✅ APROVADO |
| P7 | Formato nnnn nnnn nnnn aceito | ✅ APROVADO |
| P8 | Campo aceita caracteres não numéricos | ❌ REPROVADO |
| P9 | Validação de intervalo 0000–9999 por bloco não funciona | ❌ REPROVADO |
| P10 | Espaços não inseridos automaticamente ao sair do campo | ❌ REPROVADO |
| P11 | Botão "Adicionar" inativo com menos de 12 símbolos | ✅ APROVADO |
| P12 | Campo permite inserir mais de 12 símbolos | ❌ REPROVADO |
| P13 | Formato do código: 2 símbolos | ✅ APROVADO |
| P14 | Código aceita somente números | ✅ APROVADO |
| P15 | Campo "Código" permite inserir "00" | ❌ REPROVADO |
| P16–P19 | Valores 01, 02, 98, 99 aceitos corretamente | ✅ APROVADO |
| P20 | Campo "Código" permite inserir "100" | ❌ REPROVADO |
| P21 | Botão "Adicionar" ativo com menos de 2 símbolos no código | ❌ REPROVADO |
| P22 | Campo aceita caracteres fora dos requisitos | ❌ REPROVADO |
| P23 | Cartão e código válidos habilitam botão "Adicionar" | ✅ APROVADO |
| P24 | Botão "Adicionar" habilitado com cartão inválido + código válido | ❌ REPROVADO |
| P25 | Botão "Adicionar" habilitado com cartão válido + código inválido | ❌ REPROVADO |
| P26 | Botão "Adicionar" habilitado com cartão e código inválidos | ❌ REPROVADO |
| P27 | Sem preenchimento, botão permanece desabilitado | ✅ APROVADO |
 
---
 
### Aba 3 — Casos de Teste: Lógica do Botão "Reservar"
 
| ID | Descrição resumida | Resultado |
|----|--------------------|-----------|
| R1 | Reserva com todos os campos preenchidos corretamente | ✅ APROVADO |
| R2 | Janela "Carteira adicionada" ausente ao reservar sem carteira | ❌ REPROVADO |
| R3 | Janela "Cartão adicionado" ausente ao reservar sem pagamento | ❌ REPROVADO |
| R4 | Botão "Reservar" permanece ativo após excluir endereços | ❌ REPROVADO |
| R5 | Todos os campos vazios e endereços excluídos | 🔒 BLOQUEADO |
 
---
 
### Aba 4 — Casos de Teste: Lógica dos Recursos de Reserva (Locação)
 
| ID | Descrição resumida | Resultado |
|----|--------------------|-----------|
| T1 | Reserva com campos De/Para preenchidos funciona corretamente | ✅ APROVADO |
| T2 | Cancelamento da reserva não funciona corretamente | ❌ REPROVADO |
| T3 | Não cancelamento retorna à tela "Carro reservado" | 🔒 BLOQUEADO |
 
---
 
## 🐛 Resumo dos Bugs por Severidade
 
| Severidade | Qtd | IDs |
|------------|-----|-----|
| 🔴 Blocker  | 7  | L7, P24, P25, P26, R2, R3, R4, T2 |
| 🟠 Major    | 18 | L4, L5, L8, L9, L10, L13-POP, L14-POP, L16-POP, P4, P8, P9, P12, P15, P20, P21, P22, R3, L15 |
| 🟡 Minor    | 8  | L2, L12, L13, L14, L11-CDM, L12-CDM, L15-POP, L17-POP, P10 |
 
---
 
## 📊 Distribuição dos Resultados
 
```
✅ APROVADO    ░░░░░░░░░░░░░░░░░░░░░  ~35%
❌ REPROVADO   ████████████████████   ~54%
🔒 BLOQUEADO   ░░░░░░                  ~8%
⚠️ N/A         ░░                      ~3%
```
 
---
 
## 📁 Bug Reports
 
Cada bug reprovado possui um relatório individual em formato PNG com os campos:
 
- **ID** — identificador da coluna A da planilha
- **Summary** — descrição objetiva do problema
- **Environment** — navegador, resolução e componente
- **Steps to Reproduce** — passo a passo para reprodução
- **Expected Result** — comportamento esperado
- **Actual Result** — comportamento observado
- **Priority** — Alta / Média / Baixa / Crítica
- **Severity** — Blocker / Major / Minor
> 📦 Todos os relatórios estão disponíveis no arquivo `bug_reports_urban_routes.zip` ou na pasta `/bug_reports`.
 
---
 
## 🛠️ Tecnologias e Ferramentas
 
| Ferramenta | Uso |
|------------|-----|
| **Google Chrome** | Execução dos testes |
| **Microsoft Excel / Google Sheets** | Registro dos casos e resultados |
| **Jira** (formato) | Estrutura dos relatórios de bug |
| **Python + Pillow** | Geração automatizada dos PNGs |
 
---
 
## 👤 Autora
 
Projeto desenvolvido como parte do programa de formação em **QA (Quality Assurance)** — TripleTen.
 
---
 
## 📄 Licença
 
Este repositório é de uso educacional. Os dados e capturas de tela pertencem ao ambiente de testes do curso.
 

