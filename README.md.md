# 🚢 BRAM Offshore - Sistema de Controle de Pedidos

Sistema completo para controle e análise de pedidos da BRAM Offshore.

---

## 📊 COMPONENTES DO SISTEMA

### 🖥️ **Dashboard Desktop**
**Arquivo:** `index.html`
- Análise completa de pedidos
- KPIs e gráficos interativos
- Fornecedores críticos
- Multi-comprador (Lineker, Rafael, Thiago)
- Consolidado de backlog (Rafael)
- Filtro por semana e período

**Acesso:** https://seu-usuario.github.io/seu-repositorio/

### 📱 **App Mobile (PWA)**
**Arquivo:** `app.html`
- Versão otimizada para celular
- Instalável na tela inicial
- Funciona offline
- Mesmas funcionalidades do dashboard
- Interface touch-friendly

**Acesso:** https://seu-usuario.github.io/seu-repositorio/app.html

---

## 🔄 ATUALIZAÇÃO DE DADOS

Os dados são atualizados **automaticamente** via Google Sheets:

1. **Planilha** → Você atualiza os dados
2. **Apps Script** → Processa automaticamente
3. **API** → Disponibiliza via JSON
4. **Dashboard/App** → Atualiza ao recarregar (F5)

**Fonte de Dados:**
- Google Sheets (via Apps Script)
- API: `https://script.google.com/macros/s/AKfycbx.../exec`

---

## 📱 INSTALAÇÃO DO APP (PWA)

### **Android:**
1. Abra `app.html` no Chrome
2. Banner: "Adicionar à tela inicial"
3. Toque em "Adicionar"
4. ✅ Ícone aparece na tela inicial

### **iPhone:**
1. Abra `app.html` no Safari
2. Botão Compartilhar 📤
3. "Adicionar à Tela de Início"
4. ✅ Pronto!

### **Desktop (Windows/Mac):**
1. Abra `app.html` no Chrome
2. Barra de endereço → ➕ Instalar
3. ✅ App instalado!

---

## 📊 FUNCIONALIDADES

### **Dashboard Principal:**
- ✅ Seleção de comprador (Lineker, Rafael, Thiago)
- ✅ Filtro por área (Manutenção / Operações)
- ✅ Filtro por período (mês/ano)
- ✅ 6 KPIs principais
- ✅ Gráficos interativos
- ✅ Análise de valores
- ✅ Fornecedores críticos

### **Consolidado (Rafael):**
- ✅ Análise de backlog por comprador
- ✅ Filtro por semana (8, 7, 6, 5, 4...)
- ✅ Breakdown por categoria:
  - 🔍 Sob Análise
  - 🔧 Pend. Manutenção
  - ⏳ Aguard. Aprovação
  - 📦 Pend. Fornecedor
- ✅ Top 5 fornecedores por comprador
- ✅ Variação semanal com cores:
  - 🟢 Verde = Backlog diminuiu (bom!)
  - 🔴 Vermelho = Backlog aumentou (atenção!)

### **Interatividade:**
- ✅ Todos os cards são clicáveis
- ✅ Modais com informações detalhadas
- ✅ Drill-down por fornecedor
- ✅ Exportação de dados

---

## 🎨 TECNOLOGIAS

- **Frontend:** HTML5, CSS3, JavaScript (Vanilla)
- **Charts:** Chart.js + DataLabels
- **Backend:** Google Apps Script
- **Database:** Google Sheets
- **PWA:** Service Worker + Web Manifest
- **Hosting:** GitHub Pages

---

## 📁 ESTRUTURA DE ARQUIVOS

```
📁 Repositório
├── 📄 index.html          # Dashboard principal
├── 📄 app.html            # App mobile (PWA)
├── 📄 manifest.json       # Configuração PWA
├── 📄 sw.js               # Service Worker (offline)
├── 🖼️ icon-192.svg        # Ícone 192x192
├── 🖼️ icon-512.svg        # Ícone 512x512
└── 📄 README.md           # Este arquivo
```

---

## 🔧 CONFIGURAÇÃO

### **Google Apps Script:**

A API está configurada em:
```
https://script.google.com/macros/s/AKfycbxSVoT9gjBy0isz_fgJVIs7cYwQim0mn1is9O09ZHOPqqSD_bQ3f_1y79BE_nW-Ghz9/exec
```

### **Planilha:**
- Fonte de dados: Google Sheets
- Abas: Manutenção/Operações por comprador + Consolidado

---

## 📊 COMO USAR

### **1. Dashboard Desktop:**
```
https://seu-usuario.github.io/seu-repositorio/
```
- Selecione o comprador
- Escolha a área
- Filtre por período
- Clique nos cards para detalhes

### **2. App Mobile:**
```
https://seu-usuario.github.io/seu-repositorio/app.html
```
- Mesmas funcionalidades
- Interface mobile-friendly
- Instalável como app

### **3. Consolidado (Rafael):**
- Selecione "Rafael" no comprador
- Selecione "📊 CONSOLIDADO" na área
- Use o filtro de semana
- Clique nos cards para drill-down

---

## 🎯 CORES DO BACKLOG

**Importante:** No Consolidado, as cores indicam:

- 🟢 **VERDE** = Backlog **diminuiu** = ✅ BOM!
  - Menos pendências que na semana anterior
  - Equipe está resolvendo pedidos
  
- 🔴 **VERMELHO** = Backlog **aumentou** = ⚠️ ATENÇÃO!
  - Mais pendências que na semana anterior
  - Trabalho está acumulando

**Exemplo:**
- Lineker: +3 pedidos → 🔴 Vermelho (acumulou)
- Rafael: -71 pedidos → 🟢 Verde (resolveu!)

---

## 🔄 ATUALIZAR DADOS

1. Atualize a planilha Google Sheets
2. Aguarde processamento automático do Apps Script
3. Recarregue o dashboard (F5)
4. ✅ Dados atualizados!

**Não precisa fazer nada no GitHub!**

---

## 📱 SUPORTE

- Dashboard funciona em: Chrome, Edge, Firefox, Safari
- App PWA funciona em: Android, iOS, Windows, macOS
- Requer conexão com internet para dados atualizados
- Cache offline disponível via Service Worker

---

## 📄 LICENÇA

Uso interno - BRAM Offshore

---

**Desenvolvido para BRAM Offshore** 🚢
**Última atualização:** Fevereiro 2026
