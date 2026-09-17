# Filtro de Notas Fiscais 📑

Aplicação web para filtrar e organizar arquivos de notas fiscais por identificadores únicos (RLOC, número de NF, etc).

## 🎯 O que faz

Permite que você:
1. **Envie uma pasta inteira** com notas fiscais (PDFs)
2. **Cole os códigos** que deseja buscar (RLOC, número de NF, etc) — um por linha
3. **Filtre automaticamente** — busca no nome do arquivo E dentro do conteúdo do PDF
4. **Baixe um .zip** com apenas os arquivos encontrados, mantendo a estrutura original

## ✨ Características

- ✅ **100% client-side** — nenhum arquivo é enviado a servidor
- ✅ **Busca dupla** — nome do arquivo + conteúdo do PDF
- ✅ **PDFs escaneados** — ignorados automaticamente (sem erros)
- ✅ **Preserva estrutura** — mantém pastas e nomes originais no .zip
- ✅ **Relatório detalhado** — mostra quais códigos foram encontrados, onde, e qual não foi
- ✅ **Suporta multiplos uploads** — selecione uma pasta inteira de uma vez

## 🚀 Como usar

1. Abra o app no navegador
2. Clique em "Selecionar arquivos/pasta" e escolha a pasta com as notas fiscais
3. Cole seus códigos de busca (um por linha)  
   Exemplo: RPS_001234
            RPS_005678
            RPS_009101
4. (Opcional) Marque "Buscar também dentro dos PDFs" para fazer busca de texto
5. Clique em **Filtrar arquivos**
6. Baixe o `.zip` com os resultados

## 📊 Resultados

O app mostra:
- Quais arquivos foram encontrados
- Para cada código: se foi encontrado (por nome ou conteúdo) ou não
- Lista de códigos não encontrados
- Opção de download do .zip com os arquivos filtrados

## 🛠️ Stack

- **HTML5** — markup e layout
- **Vanilla JS** — lógica de filtro
- **pdf.js** — extração de texto de PDFs
- **JSZip** — criação de arquivo .zip

## 📝 Notas

- PDFs com texto selecionável são totalmente suportados
- PDFs escaneados/imagem: buscam apenas no nome do arquivo
- Todos os arquivos mantêm seus nomes e pastas originais no resultado
- Sem limite de tamanho (processamento local)
- Funciona offline (depois de carregada a página)

## 📦 Deployment

1. Clone o repositório
2. Abra `index.html` no navegador (ou publique em um servidor estático)
3. Pronto para usar

---

**Desenvolvido para organizar o workflow de escrituração fiscal da Flytour.**
