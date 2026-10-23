<h1 align="center">Caique Andrade</h1>
<p align="center"><b>Desenvolvedor Python · Automação de Processos (RPA) · Backend</b></p>

<p align="center">
  <a href="mailto:kiqand21@gmail.com"><img src="https://img.shields.io/badge/Email-kiqand21@gmail.com-D14836?style=flat&logo=gmail&logoColor=white"></a>
  <a href="https://linkedin.com/in/caique-andrade-588971115"><img src="https://img.shields.io/badge/LinkedIn-Caique%20Andrade-0A66C2?style=flat&logo=linkedin&logoColor=white"></a>
</p>

Profissional de operações com 8+ anos em ambiente industrial/logístico que se tornou desenvolvedor criando, por conta própria, as automações que hoje rodam em produção num terminal de combustíveis de grande porte. Conecto **SAP, Excel, sistemas web, e-mail e hardware de portaria** para eliminar trabalho manual, reduzir erros e manter a operação rodando 24/7.

> 💡 *"Transformo processos manuais em sistemas autônomos."*

---

## 📊 Impacto em números

| Resultado | Projeto |
|---|---|
| 💰 **~R$ 20 mil/mês** de economia em laudos de laboratório | Robô Pedido de Laudo |
| ⏱️ **~6 h/dia** de trabalho administrativo eliminado | Automação de Temperatura |
| ⏱️ **~2 h/dia** de trabalho de supervisão eliminado | Impressão de Documentação de Trem |
| 🚧 **94,6%** das passagens pela cancela feitas sem intervenção humana · **~85%** menos tempo no gate | Autoatendimento de Portaria |
| 📄 **~180 notas fiscais/dia** lidas por OCR e lançadas no SAP | Escrituração RPA |
| 💰 **~R$ 550/mês** de economia | Agendamento de Checklist + Curso Operação Sem Derrame |
| 🔁 **+15 automações e sistemas** em uso diário na operação | — |

---

## 🛠️ Stack

**Linguagens & Backend:** Python · JavaScript · TypeScript · SQL / PostgreSQL · VBA
**Automação / RPA:** Selenium · SAP GUI Scripting · pywin32 / win32com · pywinauto · Tesseract OCR · pdfplumber · openpyxl · schedule
**Interfaces:** Tkinter · HTML/CSS · React + Vite · Next.js · Tailwind · Zustand
**Dados & Infra:** Supabase · SQLite · GitHub Pages · Vercel · pytest

---

## 🏭 Automações em produção (ambiente industrial)

### 💰 Robô de Pedido de Laudo — [`robo-pedido-laudo`](https://github.com/CAIQUE4NDRADE/robo-pedido-laudo)
Lê e-mails de "virada de tanque", identifica o tanque que virou e o tanque que está expedindo (via planilha de passagem de turno no SharePoint) e envia automaticamente ao laboratório o pedido de laudo **somente dos tanques necessários**, aplicando regras de composição de produto.
**Impacto:** antes o laboratório emitia laudo de todos os tanques sem solicitação → **economia de ~R$ 20 mil/mês**.
`Python` `Selenium` `E-mail` `SharePoint`

### 🌡️ Automação de Temperatura — [`automacao-temperatura-bpa`](https://github.com/CAIQUE4NDRADE/automacao-temperatura-bpa)
Ciclo a cada 30 min que coleta dados do sistema web, preenche planilha, executa macros e atualiza temperatura/densidade no SAP. Deploy multiusuário, keep-alive, prevenção de suspensão, reconexão automática, notificações escalonadas e log centralizado.
**Impacto:** **~6 h/dia** de trabalho manual eliminado em processo que afeta faturamento.
`Python` `Selenium` `win32com` `SAP GUI Scripting` `Excel COM`

### 🚂 Impressão de Documentação de Trem — [`Impressao-Trem`](https://github.com/CAIQUE4NDRADE/Impressao-Trem)
Monitora o Outlook Web, reconhece e-mails de documentação de trem por padrão de assunto, baixa o ZIP, lê o PDF "Resumo de Composição" e imprime as notas **na ordem dos vagões**, com regras por remetente. Antes de imprimir, confirma por voz ("posso imprimir?").
**Impacto:** **~2 h/dia** a menos de trabalho manual da supervisão.
`Python` `Tkinter` `Selenium` `PDF parsing` `TTS`

### 🚛 Monitor de Carregamento — [`Monitor-Descarga`](https://github.com/CAIQUE4NDRADE/Monitor-Descarga)
Varre o painel de carregamento e avisa por voz quando um caminhão atinge 75%, informando baia e produto para chamar o próximo — seguindo a fila de pedidos e pulando pendências que não podem ser chamadas.
`Python` `Selenium` `TTS`

### 🚧 Autoatendimento de Portaria (Cancela + Totem) — [`rais-automacao`](https://github.com/CAIQUE4NDRADE/rais-automacao)
Sistema multiárea de entrada/saída de caminhões: totem quiosque em Tkinter, sincronização de placas com o sistema de gestão, integração com reconhecimento facial (exportação via pywinauto → cache SQLite), controle anti-dupla abertura e cursor de eventos para impedir autorização com evento antigo. Watchdog de foco no SO para o quiosque nunca perder a tela.
**Em desenvolvimento:** leitura automática de placa por câmera (ALPR/OCR) no totem.
**Impacto:** **94,6%** das passagens automáticas (análise de 2.918 eventos) · **~85%** de redução no tempo de gate.
`Python` `Selenium` `Tkinter` `pywinauto` `SQLite` `OCR`

### 📄 Escrituração RPA (NF-e / Canhotos)
Pipeline de OCR que lê **~180 NF-e/dia** (pdfplumber + Tesseract), bloqueia placas no sistema de gestão e faz o lançamento no SAP; módulos de extração de canhotos CIF/FOB e download no Portal NF-e.
`Python` `Tesseract` `pdfplumber` `SAP GUI Scripting`

### 📊 Fechamento Diário + Conciliação
Orquestrador do fechamento do dia: dispara transações SAP, downloads em paralelo, cadeia de macros VBA, impressão de spool em PDF e captura de tela quando relatório vem vazio. Motor de conciliação viagem a viagem entre sistema de gestão e SAP, com janela de tempo por entrada do caminhão, mapeamento de produtos e Treeview colorido por divergência.
`Python` `Tkinter` `SAP GUI Scripting` `openpyxl` `VBA`

### 🧾 Robô de Lançamento Fiscal (SAP)
Substituiu macros VBA por um robô em 4 etapas: imputa dados do SAP, lança notas fiscais, vincula nota de remessa ao banco de dados (casamento por placa + volume, sem sobrescrever) e confere estoque.
`Python` `SAP GUI Scripting` `HTML parsing`

### 🛢️ Monitor de Nível de Tanques
Dashboard de 19 tanques com alarmes de volume, coluna de ETA para atingir limite, detecção de sensor congelado, margens por tanque e relatório mensal em XLSX. **32 testes automatizados** com pytest.
`Python` `Tkinter` `openpyxl` `pytest`

### ⚙️ Suite de Macros SAP (Excel + VBA)
Atualização em lote de transporte, checagem de cadastro de placas (até 2.000 linhas por execução), cadastro/consulta de motoristas e lançamento de canhotos — tudo direto do Excel.
`VBA` `Excel` `SAP GUI Scripting`

---

## 🌐 Sistemas web internos

### Gestão de Gate e Pátio — [`RAIZEN-AGENDAMENTO-DESCARGA`](https://github.com/CAIQUE4NDRADE/RAIZEN-AGENDAMENTO-DESCARGA)
Controle de descarga de caminhões: entrada/saída, agendamento, chamada do motorista por WhatsApp com a baia, histórico com reversão de ações e perfis Operador/Supervisor. Evoluído da **v1 à v29** em uso diário.
`JavaScript` `HTML/CSS` `Supabase`

### Agendamento de Checklist + Curso Operação Sem Derrame — [`checklist-e-opsemderrame`](https://github.com/CAIQUE4NDRADE/checklist-e-opsemderrame)
Motorista agenda pelo celular via **QR code** o checklist do caminhão e o curso semanal de segurança.
**Impacto:** **economia de ~R$ 550/mês**.
`JavaScript` `Supabase` `GitHub Pages`

### Lançamento de Horas Extras — [`horas-extras-bpa`](https://github.com/CAIQUE4NDRADE/horas-extras-bpa)
Substitui a folha de papel: cada colaborador lança sua HE (35% / 80% / noturna / 100%), o supervisor direto aprova e no fim do mês sai a folha pronta para impressão.
`JavaScript` `Supabase` `GitHub Pages`

---

## 🛍️ Projetos freelance (clientes reais)

| Projeto | O que é | Stack |
|---|---|---|
| [**Adega da Praça**](https://adega-da-praca.vercel.app) | Delivery completo com PWA, contas de cliente, painel admin e gestão de pedidos | Next.js 15 · TypeScript · Tailwind · Supabase |
| [**Milê Atelier**](https://mile-atelier.vercel.app) | Painel de aluguel de vestidos com calendário, detecção de conflito, geração de contrato e upload de fotos | React · Vite · Supabase |
| [**NVS Street**](https://nvs-street.vercel.app) · [`repo`](https://github.com/CAIQUE4NDRADE/nvs-street) | E-commerce streetwear com carrinho e checkout via WhatsApp | React · Zustand · Supabase Storage |
| [**Dyna Festas**](https://dyna-festas-rdzk.vercel.app) | Site/sistema para empresa de festas | React · Vite · Supabase |

---

## 🎯 Foco atual
- Backend, APIs e integrações entre sistemas
- Visão computacional aplicada (leitura de placas)
- Automação de processos para empresas (aberto a projetos)

## 👤 Sobre mim
🏢 Assistente de Operações — Raízen · 🎓 Cursando Análise e Desenvolvimento de Sistemas (ADS) · 🟡 Lean Six Sigma Yellow Belt · 📍 Sumaré — SP
