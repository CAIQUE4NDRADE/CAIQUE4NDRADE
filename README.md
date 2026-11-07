<h1 align="center">Caique Andrade</h1>
<h3 align="center">Desenvolvedor Python · Automação de Processos (RPA) · Backend</h3>
<p align="center"><i>"Transformo processos manuais em sistemas autônomos."</i></p>

<p align="center">
  <a href="https://linkedin.com/in/caique-andrade-588971115"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:kiqand21@gmail.com"><img src="https://img.shields.io/badge/E--mail-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <img src="https://img.shields.io/badge/Aberto%20a%20oportunidades-2ea44f?style=for-the-badge" />
</p>

---

Profissional de operações com **8+ anos em ambiente industrial e logístico** que se tornou desenvolvedor criando, por conta própria, as automações que hoje rodam **em produção 24/7** num terminal de combustíveis de grande porte.

Conecto **SAP, Excel, sistemas web, e-mail e hardware de portaria** para eliminar trabalho manual e reduzir erros.

## 📊 Impacto em números

| Resultado | Projeto |
|---|---|
| 🚧 **94,6%** das passagens pela cancela sem intervenção humana · **~85%** menos tempo no gate | Autoatendimento de Portaria |
| ⏱️ **~6 h/dia** de trabalho manual eliminado | Automação de Temperatura |
| 📄 **~180 NF-e/dia** lidas por OCR e lançadas no SAP | Escrituração RPA |
| ⏱️ **~2 h/dia** de trabalho da supervisão eliminado | Impressão de Documentação de Trem |
| 💰 Fim dos laudos de laboratório desnecessários | Robô de Pedido de Laudo |
| 🔁 **+15** automações e sistemas em uso diário | — |

## 🛠️ Stack

**Backend e linguagens**
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![VBA](https://img.shields.io/badge/VBA-217346?style=flat-square&logo=microsoftexcel&logoColor=white)

**Automação e RPA**
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)
![SAP GUI Scripting](https://img.shields.io/badge/SAP%20GUI%20Scripting-0FAAFF?style=flat-square&logo=sap&logoColor=white)
![Tesseract OCR](https://img.shields.io/badge/Tesseract%20OCR-5A5A5A?style=flat-square)
![pywinauto](https://img.shields.io/badge/pywinauto-5A5A5A?style=flat-square)
![win32com](https://img.shields.io/badge/win32com-5A5A5A?style=flat-square)
![pdfplumber](https://img.shields.io/badge/pdfplumber-5A5A5A?style=flat-square)
![openpyxl](https://img.shields.io/badge/openpyxl-5A5A5A?style=flat-square)

**Front-end**
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-5A5A5A?style=flat-square)
![Tkinter](https://img.shields.io/badge/Tkinter-5A5A5A?style=flat-square)

**Dados e infra**
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-222222?style=flat-square&logo=githubpages&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

## ⭐ Destaques

### 🚧 Autoatendimento de Portaria (Cancela + Totem) · [`rais-automacao`](https://github.com/CAIQUE4NDRADE/rais-automacao)
Sistema multiárea de entrada e saída de caminhões: totem quiosque, sincronização de placas com o sistema de gestão, integração com reconhecimento facial (pywinauto → cache SQLite), controle anti-dupla abertura, cursor de eventos para impedir autorização com evento antigo e watchdog para o quiosque nunca perder a tela.
**Em desenvolvimento:** leitura automática de placa por câmera (ALPR/OCR).
> **94,6%** das passagens automáticas (análise de 2.918 eventos) · **~85%** menos tempo de gate

`Python` `Selenium` `Tkinter` `pywinauto` `SQLite` `OCR`

### 🌡️ Automação de Temperatura · [`automacao-temperatura-bpa`](https://github.com/CAIQUE4NDRADE/automacao-temperatura-bpa)
Ciclo a cada 30 min que coleta dados do sistema web, preenche planilha, roda macros e atualiza temperatura e densidade no SAP. Deploy multiusuário, keep-alive, reconexão automática, notificações escalonadas e log centralizado.
> **~6 h/dia** de trabalho manual eliminado num processo que afeta o faturamento

`Python` `Selenium` `win32com` `SAP GUI Scripting` `Excel COM`

### 📄 Escrituração RPA (NF-e / Canhotos)
Pipeline de OCR que lê **~180 NF-e por dia** (pdfplumber + Tesseract), bloqueia placas no sistema de gestão e faz o lançamento no SAP. Inclui extração de canhotos CIF/FOB e download no Portal NF-e.

`Python` `Tesseract` `pdfplumber` `SAP GUI Scripting`

### 💰 Robô de Pedido de Laudo · [`robo-pedido-laudo`](https://github.com/CAIQUE4NDRADE/robo-pedido-laudo)
Lê e-mails de virada de tanque, cruza com a planilha de passagem de turno no SharePoint e pede ao laboratório o laudo **somente dos tanques necessários**, aplicando regras de composição de produto. Antes, o laboratório emitia laudo de todos os tanques.

`Python` `Selenium` `E-mail` `SharePoint`

<details>
<summary><b>🏭 Ver todas as automações em produção</b></summary>
<br>

**🚂 Impressão de Documentação de Trem** · [`Impressao-Trem`](https://github.com/CAIQUE4NDRADE/Impressao-Trem)
Monitora o Outlook Web, baixa o ZIP, lê o PDF "Resumo de Composição" e imprime as notas **na ordem dos vagões**, com regras por remetente e confirmação por voz antes de imprimir. **~2 h/dia** a menos para a supervisão.
`Python` `Tkinter` `Selenium` `PDF parsing` `TTS`

**🚛 Monitor de Carregamento** · [`Monitor-Descarga`](https://github.com/CAIQUE4NDRADE/Monitor-Descarga)
Avisa por voz quando um caminhão atinge 75%, informando baia e produto para chamar o próximo, seguindo a fila de pedidos e pulando pendências que não podem ser chamadas.
`Python` `Selenium` `TTS`

**📊 Fechamento Diário + Conciliação**
Orquestra transações SAP, downloads em paralelo, macros VBA, impressão de spool em PDF e captura de tela quando o relatório vem vazio. Motor de conciliação viagem a viagem entre sistema de gestão e SAP, com mapeamento de produtos e destaque de divergências.
`Python` `Tkinter` `SAP GUI Scripting` `openpyxl` `VBA`

**🧾 Robô de Lançamento Fiscal (SAP)**
Substituiu macros VBA por um robô em 4 etapas: imputa dados do SAP, lança notas fiscais, vincula a nota de remessa (casamento por placa + volume) e confere estoque.
`Python` `SAP GUI Scripting` `HTML parsing`

**🛢️ Monitor de Nível de Tanques**
Dashboard de 19 tanques com alarmes, ETA para atingir limite, detecção de sensor congelado e relatório mensal em XLSX. **32 testes automatizados.**
`Python` `Tkinter` `openpyxl` `pytest`

**⚙️ Suíte de Macros SAP (Excel + VBA)**
Atualização em lote de transporte, checagem de até 2.000 placas por execução, cadastro de motoristas e lançamento de canhotos, direto do Excel.
`VBA` `Excel` `SAP GUI Scripting`

</details>

<details>
<summary><b>🌐 Ver sistemas web internos</b></summary>
<br>

**Gestão de Gate e Pátio** · [`RAIZEN-AGENDAMENTO-DESCARGA`](https://github.com/CAIQUE4NDRADE/RAIZEN-AGENDAMENTO-DESCARGA)
Controle de descarga com agendamento, chamada do motorista por WhatsApp com a baia, histórico com reversão de ações e perfis Operador/Supervisor. Evoluído da **v1 à v29** em uso diário.
`JavaScript` `HTML/CSS` `Supabase`

**Agendamento de Checklist + Curso Operação Sem Derrame** · [`checklist-e-opsemderrame`](https://github.com/CAIQUE4NDRADE/checklist-e-opsemderrame)
O motorista agenda pelo celular, via **QR code**, o checklist do caminhão e o curso semanal de segurança.
`JavaScript` `Supabase` `GitHub Pages`

**Lançamento de Horas Extras** · [`horas-extras-bpa`](https://github.com/CAIQUE4NDRADE/horas-extras-bpa)
Substitui a folha de papel: o colaborador lança a HE (35% / 80% / noturna / 100%), o supervisor aprova e no fim do mês sai a folha pronta para impressão.
`JavaScript` `Supabase` `GitHub Pages`

</details>

## 🛍️ Projetos freelance (clientes reais)

| Projeto | O que é | Stack |
|---|---|---|
| [**Adega da Praça**](https://adega-da-praca.vercel.app) | Delivery completo com PWA, contas de cliente, painel admin e gestão de pedidos | Next.js 15 · TypeScript · Tailwind · Supabase |
| [**Milê Atelier**](https://mile-atelier.vercel.app) | Aluguel de vestidos com calendário, detecção de conflito, geração de contrato e upload de fotos | React · Vite · Supabase |
| [**NVS Street**](https://nvs-street.vercel.app) · [`repo`](https://github.com/CAIQUE4NDRADE/nvs-street) | E-commerce streetwear com carrinho e checkout via WhatsApp | React · Zustand · Supabase Storage |
| [**Dyna Festas**](https://dyna-festas-rdzk.vercel.app) | Site e sistema para empresa de festas | React · Vite · Supabase |

## 🧪 Projetos pessoais

**🔒 [FilhaBlock](https://github.com/CAIQUE4NDRADE/filhablock)**: trava teclado e mouse no Windows enquanto o vídeo continua rodando, para minha filha assistir desenho sem bagunçar o PC. Usa hooks de baixo nível do Windows, só com a biblioteca padrão do Python.
`Python` `ctypes` `WinAPI`

## 🎯 Foco atual

- 🚘 **Leitura automática de placas (ALPR)**: integrando câmera + OCR ao totem de portaria para eliminar a digitação da placa pelo motorista
- 🔗 **Integração SAP ↔ sistemas web**: levando dados de processos que hoje dependem de planilha e macro para bancos PostgreSQL/Supabase
- 🌐 **Sistemas web com Supabase**: apps internos e para clientes (agendamento, gestão de pátio, delivery) com autenticação, perfis e banco em tempo real
- 🎓 **Cursando ADS**: aprofundando em arquitetura de software, banco de dados e boas práticas de backend
- 💼 **Aberto a oportunidades** como Desenvolvedor Python / RPA e a projetos de automação para empresas

## 👤 Sobre mim

🏢 Assistente de Operações na Raízen · 🎓 Cursando Análise e Desenvolvimento de Sistemas (ADS) · 🟡 Lean Six Sigma Yellow Belt · 📍 Sumaré, SP
