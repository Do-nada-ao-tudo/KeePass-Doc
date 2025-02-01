# 📚 Documentação DNAT - Do Nada ao Tudo

[![en](https://img.shields.io/badge/lang-en-red.svg)](./README.md)
[![br](https://img.shields.io/badge/lang-br-green.svg)](./README-br.md)

## 🌟 Visão Geral

A **DNAT (Do Nada ao Tudo)** é um projeto com documentação organizada e
acessível, construída utilizando [VitePress](https://vitepress.vuejs.org/), um
gerador de sites estáticos moderno e eficiente. O objetivo principal deste
projeto é fornecer uma plataforma de documentação abrangente e fácil de usar,
permitindo que os usuários acessem informações detalhadas acerca de crypto,
blockchain, segurança e muito mais.

<br>

## 🏗️ Estrutura do Projeto

Abaixo está a estrutura organizada do projeto:

```
.
├── .vitepress/
│   ├── config.ts          # Configuração principal do VitePress
│   └── locales/           # Configurações específicas para cada idioma
├── assets/                # Arquivos estáticos (imagens, ícones, etc.)
├── src/
│   ├── index.md           # Página inicial do projeto(Padrão PT-BR)
│   └── locale/            # Pastas para cada idioma suportado
│       ├── docs/          # É aqui onde você deve adicionar suas páginas
│       └── index.md       # Página inicial para o idioma
└── README.md              # Resumo geral do projeto
```

> 💡 **Dica:** Use esta estrutura como referência ao adicionar novas páginas ou
> modificar o projeto, sempre visando manter um padrão consistente.

<br>

## 🤝 Como Contribuir

### 1. Adicionando Páginas

Para adicionar novas páginas à documentação, siga os passos abaixo:

1. Navegue até a pasta `src/`, onde há uma pasta para cada idioma suportado.
2. Escolha o idioma desejado e entre em `docs`, que é a pasta onde deve ser
   adicionado o conteúdo:
   - Crie uma nova pasta com o nome da página desejada.
   - Ou crie um arquivo `.md` dentro de uma pasta já existente, sempre
     respeitando a hierarquia das pastas.
3. Adicione conteúdo no formato **Markdown**.
4. Atualize o arquivo `.vitepress/locales/<locale>.ts` para incluir o caminho da
   nova página na barra lateral (`sidebar`).

### 2. Traduções

Para traduzir o conteúdo para novos idiomas:

1. Edite os arquivos em `.vitepress/locales/`.
2. Mantenha as chaves sincronizadas entre os idiomas para garantir consistência.
3. Atualize o arquivo `config.ts` para incluir o novo idioma, se necessário.

<br>

## 🛠️ Desenvolvimento Local

### Instalação

```bash
npm install
```

### Execução Local

Inicie o servidor de desenvolvimento:

```bash
npm run dev
```

Acesse o site localmente em:  
[http://localhost:5173](http://localhost:5173)

### Compilação

Para compilar o projeto para produção:

```bash
npm run build
```

### Executar o Build do Projeto

```bash
npm run preview
```

<br>

## 📋 Boas Práticas

Siga estas diretrizes para manter a documentação organizada e consistente:

- **Organização por temas:** Crie pastas temáticas dentro de `src/locale/docs/`
  para agrupar páginas relacionadas.
- **Traduções atualizadas:** Sempre que adicionar ou modificar conteúdo,
  certifique-se de que todas as traduções estejam sincronizadas.
- **Padrões estabelecidos:** Siga o estilo e as convenções já definidas no
  projeto para garantir uniformidade.

<br>

### 🔍 Exemplo de Uso de Markdown

#### Listas Aninhadas

Use listas aninhadas para organizar informações hierárquicas:

```markdown
- Categoria Principal
  - Subcategoria 1
    - Item 1
    - Item 2
  - Subcategoria 2
```

#### Tabelas

Tabelas são úteis para organizar informações tabulares:

| Comando         | Descrição                            |
| --------------- | ------------------------------------ |
| `npm install`   | Instala dependências                 |
| `npm run dev`   | Inicia o servidor de desenvolvimento |
| `npm run build` | Compila o projeto para produção      |

#### Blocos de Código

Use blocos de código para destacar comandos ou exemplos:

```javascript
const message = 'Olá, mundo!';
console.log(message);
```

<br>

## 📜 Licença

Este projeto está licenciado sob a **MIT License**. Consulte o arquivo
[LICENSE](./LICENCE.txt) para mais detalhes.

<br>

## 📞 Contato

Se precisar de ajuda ou quiser contribuir:

- Abra uma **issue** no repositório oficial.
- Entre em contato com a equipe responsável pelo projeto.
