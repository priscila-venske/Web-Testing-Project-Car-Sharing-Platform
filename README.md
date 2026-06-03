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
| L4 | Frase "Carshering~$ X Duração: X min" — erro ortográfico e de formatação | [❌ REPROVADO](https://drive.google.com/file/d/1t2M5meKtArEyQvGKbt0n5rCKsFSK0vo5/view?usp=drive_link) |
| L5 | Layout do botão "Reservar" divergente do especificado | [❌ REPROVADO](https://drive.google.com/file/d/1NtrpqTMUAGXKW-dq1t6-lx12_CR2UHXJ/view?usp=drive_link) |
| L6 | Exibe carro azul no modo Personal | ✅ APROVADO |
| L7 | Rota não exibida no mapa | [❌ REPROVADO](https://drive.google.com/file/d/1H_blCEOjqCVK37a5h__yB8i3LFBydOET/view?usp=drive_link) |
| L8 | Carros azuis não aparecem no mapa após reservar | [❌ REPROVADO](https://drive.google.com/file/d/1vr2hu1oB-3kW35hyKx-eLVQcOmUbRXT9/view?usp=drive_link) |
| L9 | Localização do BMW ausente no mapa (Casual) | [❌ REPROVADO](https://drive.google.com/file/d/1050flMFKjDrHHBYbWIlKrDyUOd9zB1xM/view?usp=drive_link) |
| L10 | Exibe modelo de veículo na tarifa Casual | ✅ APROVADO |
| L11 | Exibe frase "Apenas negócios, nada extra" | ✅ APROVADO |
| L12 | Inconsistência visual no texto de tempo/espera (Casual) | [❌ REPROVADO](https://drive.google.com/file/d/1RgZeYGK47qQw5-OvqGA171kYa4U2FSQ1/view?usp=drive_link) |
| L13 | Ilustração sem frisos na roda/porta dianteira (Casual) | [❌ REPROVADO](https://drive.google.com/file/d/1db51WjGnprbATGYnJe67lxmfPPkMDz_t/view?usp=drive_link) |
| L14 | Texto de acessórios em letras minúsculas indevidamente | [❌ REPROVADO](https://drive.google.com/file/d/1LjlXc_fvjjYilhNoqCSg7dmsK_eXW_FS/view?usp=drive_link) |
| L15 | Info de km/duração ausente próxima ao botão "RESERVAR" | [❌ REPROVADO](https://drive.google.com/file/d/1Z8LzMKZeDxfqF268Jhcb13d81zeFASMd/view?usp=drive_link) |
| L11-CDM | Botão "Adicionar Carteira" sem símbolo ">" | [❌ REPROVADO](https://drive.google.com/file/d/1v6hq-i0-4EoOX3hyOjTxlypAzsruiKLo/view?usp=drive_link) |
| L12-CDM | Campo sem destaque verde/ícone de verificação após carteira válida | [❌ REPROVADO](https://drive.google.com/file/d/1iH6RJHUzh4omiPOle642xts5GK68XIG1/view?usp=drive_link) |
| L13-POP | Pop-up exibe apenas "O carro foi reservado" sem dados completos | [❌ REPROVADO](https://drive.google.com/file/d/1KKtFbjLpBQAIsQn8A7hOHpC9ZA2TdTJs/view?usp=drive_link) |
| L14-POP | Nome do veículo ausente na confirmação | [❌ REPROVADO](https://drive.google.com/file/d/1nbOBK_bw3RWm3oh_0fdltduXzs8N9HzH/view?usp=drive_link) |
| L15-POP | Ilustração sem frisos no pop-up de confirmação | [❌ REPROVADO](https://drive.google.com/file/d/1WVnLCUSToB4_3gmAvCzg41lhEojcmNwL/view?usp=drive_link) |
| L16-POP | Botão "Cancelar" inativo na tela de confirmação | [❌ REPROVADO](https://drive.google.com/file/d/17uaJ0rGu_XBLxR35oPo8D1HtX0x4ZOeJ/view?usp=drive_link) |
| L17-POP | Custo não exibido no formato "Custo – $X" | [❌ REPROVADO](https://drive.google.com/file/d/196sJ-rD-D_fW5MtXBDKRhCr3w0fdkqpW/view?usp=drive_link) |
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
| P4 | Últimos 4 dígitos do cartão não exibidos após adição | [❌ REPROVADO](https://drive.google.com/file/d/1DjixQs-s0CcdQGE19o2wzCiFG3Ci2NPW/view?usp=drive_link) |
| P5 | Botão "Cancelar" fecha janela de cadastro | ✅ APROVADO |
| P6 | Botão "X" fecha janela de cadastro | ✅ APROVADO |
| P7 | Formato nnnn nnnn nnnn aceito | ✅ APROVADO |
| P8 | Campo aceita caracteres não numéricos | [❌ REPROVADO](https://drive.google.com/file/d/1-rnKBOl6AKc9rCh81nzUfHzVpWK_zNMS/view?usp=drive_link) |
| P9 | Validação de intervalo 0000–9999 por bloco não funciona | [❌ REPROVADO](https://drive.google.com/file/d/1CkPsu4YbmCAdzYEcKWZ3W75uaUf08S4B/view?usp=drive_link) |
| P10 | Espaços não inseridos automaticamente ao sair do campo | [❌ REPROVADO](https://drive.google.com/file/d/1xHJrMFzVzd_njlV1D9xW-0L-wt7Dj4ye/view?usp=drive_link) |
| P11 | Botão "Adicionar" inativo com menos de 12 símbolos | ✅ APROVADO |
| P12 | Campo permite inserir mais de 12 símbolos | [❌ REPROVADO](https://drive.google.com/file/d/1e4p-ET9CwXTHY4dc-0uu9P6VnlK9xkE5/view?usp=drive_link) |
| P13 | Formato do código: 2 símbolos | ✅ APROVADO |
| P14 | Código aceita somente números | ✅ APROVADO |
| P15 | Campo "Código" permite inserir "00" | [❌ REPROVADO](https://drive.google.com/file/d/1qXvaARv9fqO-blRuBTtZToeCiooTd9XG/view?usp=drive_link) |
| P16–P19 | Valores 01, 02, 98, 99 aceitos corretamente | ✅ APROVADO |
| P20 | Campo "Código" permite inserir "100" | [❌ REPROVADO](https://drive.google.com/file/d/1K-CTt2UD_O4a--4DGHXG3e9xqEbWRdJQ/view?usp=drive_link) |
| P21 | Botão "Adicionar" ativo com menos de 2 símbolos no código | [❌ REPROVADO](https://drive.google.com/file/d/1SMIR3AQrhYn4gU4-vXZbxNOjPh__dElq/view?usp=drive_link) |
| P22 | Campo aceita caracteres fora dos requisitos | [❌ REPROVADO](https://drive.google.com/file/d/1f4ZMgvmx6QXi5joyGAW_kkYCrtUO5Qi9/view?usp=drive_link) |
| P23 | Cartão e código válidos habilitam botão "Adicionar" | ✅ APROVADO |
| P24 | Botão "Adicionar" habilitado com cartão inválido + código válido | [❌ REPROVADO](https://drive.google.com/file/d/1UGq6BjBMh8Xf26JD-dKnxOSzRi4fs2hb/view?usp=drive_link) |
| P25 | Botão "Adicionar" habilitado com cartão válido + código inválido | [❌ REPROVADO](https://drive.google.com/file/d/1Gp3G61uu_ejVT5FN9j77tuh7oK9Q4lit/view?usp=drive_link) |
| P26 | Botão "Adicionar" habilitado com cartão e código inválidos | [❌ REPROVADO](https://drive.google.com/file/d/1icmYGOz4nk5zr5x5VKg3qc_lQWNHIwX5/view?usp=drive_link) |
| P27 | Sem preenchimento, botão permanece desabilitado | ✅ APROVADO |
 
---
 
### Aba 3 — Casos de Teste: Lógica do Botão "Reservar"
 
| ID | Descrição resumida | Resultado |
|----|--------------------|-----------|
| R1 | Reserva com todos os campos preenchidos corretamente | ✅ APROVADO |
| R2 | Janela "Carteira adicionada" ausente ao reservar sem carteira | [❌ REPROVADO](https://drive.google.com/file/d/1tHOhaYP_R17KOUnukZykuRjfdslRQGmE/view?usp=drive_link) |
| R3 | Janela "Cartão adicionado" ausente ao reservar sem pagamento | [❌ REPROVADO](https://drive.google.com/file/d/1wXvOsSVHzI92jTLKceWwL4UpwW4zp4iU/view?usp=drive_link) |
| R4 | Botão "Reservar" permanece ativo após excluir endereços | [❌ REPROVADO](https://drive.google.com/file/d/1rLwqLoA6upigAH4Q-ydLHIstVUz-ISzV/view?usp=drive_link) |
| R5 | Todos os campos vazios e endereços excluídos | 🔒 BLOQUEADO |
 
---
 
### Aba 4 — Casos de Teste: Lógica dos Recursos de Reserva (Locação)
 
| ID | Descrição resumida | Resultado |
|----|--------------------|-----------|
| T1 | Reserva com campos De/Para preenchidos funciona corretamente | ✅ APROVADO |
| T2 | Cancelamento da reserva não funciona corretamente | [❌ REPROVADO](https://drive.google.com/file/d/17xNHvyItt4BXYSmSseYaCxOO5eiO2dRn/view?usp=drive_link) |
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
 

