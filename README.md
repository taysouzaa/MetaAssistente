# MetaAssistente

> Assistente web interativo para orientação estratégica de partidas, com duas interfaces especializadas.

![Status](https://img.shields.io/badge/status-concluído-22c55e)
![Frontend](https://img.shields.io/badge/frontend-HTML%2FCSS%2FJS-1f6feb)
![Tipo](https://img.shields.io/badge/tipo-ferramenta%20web-f59e0b)
![Licença](https://img.shields.io/badge/licença-proprietária-red)

> **Estado:** ativo · **Última revisão:** 2026-08-10

## Visão geral

O **MetaAssistente** é uma aplicação web que responde dúvidas de estratégia de partidas consultando a **API do Google Gemini** (`generativelanguage/v1beta`). São duas interfaces distintas sobre a mesma ideia, cada uma com sua própria lógica e identidade visual. Projeto construído durante o **NLW Agents** da Rocketseat.

### O que o sistema resolve

- Fornece orientações estratégicas de forma rápida e acessível.
- Oferece duas experiências visuais distintas para diferentes preferências.
- Interface leve: roda direto no navegador, sem backend próprio nem instalação.

## O que foi desenvolvido

### 1. Interface 1 — Assistente Principal (`index1.html`)
- Consulta de estratégias e orientações em tempo real.
- Layout limpo focado na usabilidade.
- Lógica de interação em `script1.js`.

### 2. Interface 2 — Visão Alternativa (`index2.html`)
- Experiência visual alternativa com background imersivo (`bg.jpg`).
- Fluxo de navegação diferenciado.
- Lógica independente em `script2.js`.

## Stack

- **Frontend:** HTML5, CSS3, JavaScript (vanilla)
- **IA:** API do Google Gemini, chamada direto do navegador via `fetch`
- **Deploy:** Hospedagem estática — sem build

> ⚠️ A chave da API do Gemini é digitada pelo usuário no próprio formulário e fica só na memória da página — não é versionada nem enviada a lugar nenhum além do endpoint do Google. É uma escolha adequada a uma demo pessoal; num produto real a chamada iria para um proxy no servidor, como faço nos outros projetos.

## Estrutura do projeto

```text
.
├─ index1.html    ← interface principal
├─ index2.html    ← interface alternativa
├─ script1.js     ← lógica da interface 1
├─ script2.js     ← lógica da interface 2
├─ style1.css     ← estilos da interface 1
├─ style2.css     ← estilos da interface 2
├─ bg.jpg         ← imagem de fundo
└─ logo.png       ← logotipo
```

## Rodar local

Abra `index1.html` ou `index2.html` diretamente no navegador.

## Licença

Licença proprietária — todos os direitos reservados. O código pode ser lido para avaliação profissional ou estudo; qualquer reuso, cópia, modificação ou uso comercial exige autorização prévia e por escrito da autora. Ver [LICENSE](./LICENSE).