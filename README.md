# 🔍 Consultor de CEP

Sistema moderno e responsivo para consulta de endereços brasileiros por CEP, utilizando múltiplas APIs confiáveis com fallback automático.

## ✨ Funcionalidades

- ✅ **Busca de CEP** - Integrada com 3 APIs brasileiras confiáveis
- ✅ **Fallback Automático** - Se uma API falhar, tenta a próxima automaticamente
- ✅ **Máscara de Entrada** - Formata automaticamente (XXXXX-XXX)
- ✅ **Validação em Tempo Real** - Verifica se o CEP tem 8 dígitos
- ✅ **Copiar para Clipboard** - Com feedback visual de sucesso
- ✅ **Interface Responsiva** - 100% responsivo (Desktop, Tablet, Mobile)
- ✅ **Loading Animado** - Spinner elegante durante busca
- ✅ **Tratamento de Erros** - Mensagens claras e úteis
- ✅ **Sem Dependências Externas** - HTML, CSS e JavaScript puro

## 🚀 Como Usar

### Online (GitHub Pages)

Acesse diretamente: **https://neiiiii.github.io/consultor-cep**

### Localmente

1. Clone o repositório:
```bash
git clone https://github.com/neiiiii/consultor-cep.git
cd consultor-cep
```

2. Abra o arquivo `index.html` no navegador

## 🔌 APIs Integradas

O sistema tenta as seguintes APIs em ordem:

1. **ViaCEP** - `https://viacep.com.br/`
   - Rápida e confiável
   - Sem autenticação necessária

2. **BrasilAPI v2** - `https://brasilapi.com.br/api/cep/v2/`
   - Alternativa confiável
   - Sem limite de requisições

3. **AwesomeAPI** - `https://cep.awesomeapi.com.br/`
   - Terceira opção como fallback
   - Resposta rápida

## 📱 Interface

### Estados do Sistema

**1. Estado Inicial**
- Campo de entrada vazio
- Mensagem de orientação

**2. Durante Busca**
- Spinner animado
- Botão desabilitado

**3. Resultado Encontrado**
- CEP formatado
- Logradouro/Rua
- Número/Complemento
- Bairro
- Cidade
- Estado (UF)
- Botões: Copiar Endereço e Nova Busca

**4. Erro**
- Mensagem clara explicando o problema
- Possibilidade de nova tentativa

## 🎨 Design

- **Gradiente**: Roxo ao violeta (#4f46e5 → #7c3aed)
- **Cores**:
  - Primária: #4f46e5
  - Sucesso: #10b981
  - Erro: #ef4444
- **Tipografia**: Sistema de fonts nativa do sistema operacional
- **Transições**: Suaves (0.3s)
- **Sombras**: Modernas e elegantes

## 🛠️ Tecnologias

- **HTML5** - Estrutura semântica
- **CSS3** - Grid, Flexbox, Gradientes, Animações
- **JavaScript (ES6+)** - Assíncrono, Fetch API

## 📊 Exemplo de Uso

```javascript
// Digite: 01001000
// Resultado:
// CEP: 01001-000
// Logradouro: Praça da Sé
// Bairro: Centro
// Cidade: São Paulo
// Estado: SP
```

## 🎯 Validações

- ✅ CEP deve ter exatamente 8 dígitos
- ✅ Aceita entrada com ou sem hífen
- ✅ Remove caracteres especiais automaticamente
- ✅ Mostra mensagem se CEP não for encontrado

## 📦 Estrutura de Arquivos

```
consultor-cep/
├── index.html    # Arquivo principal (HTML + CSS + JS)
├── README.md     # Este arquivo
└── .gitignore    # Arquivo de configuração git
```

## 🔄 Fluxo de Funcionamento

```
Usuário digita CEP
     ↓
Validação (8 dígitos)
     ↓
Tenta API 1 (ViaCEP)
     ↓
Se falhar → Tenta API 2 (BrasilAPI)
     ↓
Se falhar → Tenta API 3 (AwesomeAPI)
     ↓
Se falhar → Exibe erro
     ↓
Se sucesso → Exibe endereço
```

## 🌐 Compatibilidade

- ✅ Chrome/Chromium
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Opera
- ✅ Mobile browsers

## 📝 Licença

MIT License - Sinta-se livre para usar em seus projetos!

## 👨‍💻 Autor

Desenvolvido por **neiiiii**

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se livre para abrir issues ou enviar pull requests.

## 📧 Contato

Tem dúvidas ou sugestões? Abra uma issue no repositório!

---

**Desenvolvido com ❤️ usando HTML, CSS e JavaScript puro**