# 📱 GUIA DE INSTALAÇÃO - BRAM OFFSHORE PWA

## ✅ ARQUIVOS DO PWA

Você recebeu 5 arquivos:

1. ✅ **App_Mobile_COMPLETO_Final.html** → Renomeie para `app.html`
2. ✅ **manifest.json** → Manifesto do PWA
3. ✅ **sw.js** → Service Worker (cache e offline)
4. ✅ **icon-192.svg** → Ícone 192x192 (renomeie para `icon-192.png` OU converta para PNG*)
5. ✅ **icon-512.svg** → Ícone 512x512 (renomeie para `icon-512.png` OU converta para PNG*)

*Nota: SVGs funcionam em muitos navegadores, mas PNG é mais compatível.

---

## 🚀 PASSO 1: FAZER UPLOAD NO GITHUB

### **1.1 — Estrutura de Arquivos:**

```
seu-repositorio/
├── app.html                    ← App principal
├── index.html                  ← Dashboard (já existe)
├── manifest.json               ← Novo
├── sw.js                       ← Novo
├── icon-192.png (ou .svg)      ← Novo
└── icon-512.png (ou .svg)      ← Novo
```

### **1.2 — Upload:**

1. Renomeie `App_Mobile_COMPLETO_Final.html` para `app.html`
2. Faça upload de **TODOS os 5 arquivos** no GitHub
3. Commit e push

---

## 📱 PASSO 2: CONVERTER SVG PARA PNG (OPCIONAL)

Se quiser melhor compatibilidade, converta os SVGs para PNG:

### **Opção A: Online (Rápido)**
1. Acesse: https://svgtopng.com
2. Faça upload de `icon-192.svg`
3. Defina tamanho: **192x192**
4. Download como `icon-192.png`
5. Repita para `icon-512.svg` → **512x512** → `icon-512.png`

### **Opção B: Usar como SVG (Funciona na maioria)**
1. Renomeie `icon-192.svg` para `icon-192.png`
2. Renomeie `icon-512.svg` para `icon-512.png`
3. (Muitos navegadores aceitam SVG mesmo com extensão .png)

---

## 📲 PASSO 3: INSTALAR NO CELULAR

### **ANDROID (Chrome/Edge):**

1. Abra o app: `https://seu-site.com/app.html`
2. Aguarde 1-2 segundos
3. Banner aparece: **"Adicionar BRAM Pedidos à tela inicial"**
4. Toque em **"Adicionar"** ou **"Instalar"**
5. ✅ Ícone aparece na tela inicial!

**OU:**
1. Menu (⋮) → **"Adicionar à tela inicial"**
2. Confirme
3. ✅ Pronto!

### **iPhone/iPad (Safari):**

1. Abra: `https://seu-site.com/app.html`
2. Toque no botão **Compartilhar** 📤 (na barra inferior)
3. Role para baixo
4. Toque em **"Adicionar à Tela de Início"**
5. Confirme
6. ✅ Ícone aparece na tela inicial!

### **WINDOWS (Chrome/Edge):**

1. Abra: `https://seu-site.com/app.html`
2. Barra de endereço → ícone **➕ Instalar**
3. Clique em **"Instalar"**
4. ✅ App aparece como atalho no desktop!

### **macOS (Chrome/Safari):**

1. Abra no Chrome: `https://seu-site.com/app.html`
2. Menu → **"Instalar BRAM Pedidos..."**
3. Confirme
4. ✅ App na barra de aplicativos!

---

## 🎯 COMO FUNCIONA

### **Service Worker:**
- ✅ Cacheia o app para funcionar offline
- ✅ Sempre busca dados novos da API quando online
- ✅ Se sem internet, mostra erro amigável

### **Manifest:**
- ✅ Define nome do app: "BRAM Pedidos"
- ✅ Define ícone e cores
- ✅ Configura modo standalone (sem barra do navegador)
- ✅ Permite instalação

### **Atualização Automática:**
- ✅ Sempre que abre o app → busca dados novos
- ✅ Sempre que troca comprador → busca novos dados
- ✅ Pull to refresh → atualiza dados

---

## ✅ VALIDAÇÃO

### **App instalado corretamente se:**
- ✅ Ícone com navio aparece na tela inicial
- ✅ Nome "BRAM Pedidos" aparece embaixo do ícone
- ✅ Ao abrir, não mostra barra de endereço
- ✅ Tela toda é do app (modo standalone)
- ✅ Dados carregam normalmente

### **Testar offline:**
1. Abra o app
2. Aguarde carregar
3. Ative modo avião ✈️
4. App continua funcionando (com dados em cache)
5. Tente atualizar → Mostra "Sem conexão"
6. Desative modo avião
7. Recarregue → Dados atualizados!

---

## 🔧 TROUBLESHOOTING

### **❌ Banner de instalação não aparece:**
- Verifique se **TODOS** os arquivos foram enviados
- Verifique se `manifest.json` está na raiz
- Verifique se `sw.js` está na raiz
- Limpe cache: F12 → Application → Clear storage
- Recarregue a página

### **❌ Ícone não aparece:**
- Verifique se os arquivos `icon-192.png` e `icon-512.png` existem
- Se usando SVG, converta para PNG
- Verifique o caminho no `manifest.json`

### **❌ Dados não atualizam:**
- Verifique se Apps Script foi atualizado
- Verifique se API foi reimplantada
- Teste a URL da API diretamente no navegador
- Limpe cache do app

### **❌ "Erro ao carregar":**
- Verifique conexão com internet
- Verifique se a URL da API está correta
- Teste no dashboard desktop primeiro

---

## 🎨 PERSONALIZAÇÕES

### **Mudar cores do app:**
Edite `manifest.json`:
```json
"background_color": "#001529",  ← Cor de fundo ao abrir
"theme_color": "#001529"        ← Cor da barra superior
```

### **Mudar nome do app:**
Edite `manifest.json`:
```json
"short_name": "BRAM Pedidos",   ← Nome na tela inicial
"name": "BRAM Offshore - ..."   ← Nome completo
```

### **Mudar ícone:**
Substitua os arquivos `icon-192.png` e `icon-512.png` por seus próprios ícones.

---

## 📊 CHECKLIST DE INSTALAÇÃO

- [ ] Renomear `App_Mobile_COMPLETO_Final.html` → `app.html`
- [ ] Upload de `app.html` no GitHub
- [ ] Upload de `manifest.json` no GitHub
- [ ] Upload de `sw.js` no GitHub
- [ ] Upload de `icon-192.png` (ou .svg) no GitHub
- [ ] Upload de `icon-512.png` (ou .svg) no GitHub
- [ ] Testar no navegador: `https://seu-site.com/app.html`
- [ ] Ver banner de instalação (ou menu "Adicionar à tela inicial")
- [ ] Instalar o app
- [ ] Verificar ícone na tela inicial
- [ ] Abrir app instalado
- [ ] Verificar modo standalone (sem barra do navegador)
- [ ] Testar carregamento de dados
- [ ] Testar seleção de comprador
- [ ] Testar consolidado Rafael
- [ ] Testar offline (modo avião)
- [ ] ✅ PWA funcionando 100%!

---

## 🚀 RESULTADO FINAL

Depois de instalado:
- ✅ Ícone bonito com navio na tela inicial
- ✅ Abre como app nativo (sem navegador)
- ✅ Funciona offline (dados em cache)
- ✅ Sempre busca dados atualizados quando online
- ✅ Mesmo comportamento do dashboard
- ✅ Pode desinstalar como qualquer app

---

**Faça upload e instale! Agora é um PWA DE VERDADE!** 📱✅
