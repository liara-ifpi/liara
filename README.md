# LIARA (Laboratório de Inteligência Artificial, Robótica e Automações) - IFPI Campus Picos Website

## 1. Introdução

Este repositório contém o código-fonte do site oficial do Laboratório de Inteligência Artificial, Robótica e Automações (LIARA) do Instituto Federal do Piauí (IFPI), Campus Picos. O site tem como objetivo principal servir como uma plataforma para divulgar os trabalhos de pesquisa, projetos desenvolvidos e apresentar os membros da equipe do laboratório. Atualmente, o site encontra-se em fase de desenvolvimento.

## 2. Estrutura do Projeto e Gerenciamento de Conteúdo

O site utiliza uma abordagem "headless" para o gerenciamento de conteúdo, onde os dados dos posts são armazenados em arquivos JSON estáticos. A configuração do conteúdo é definida em `keystatic.config.ts`, que especifica a estrutura esperada para cada post. Os arquivos de conteúdo estão localizados no diretório `src/content/posts/`.

## 3. Publicação de Novos Artigos/Posts

Para publicar um novo artigo ou post no site, siga os passos abaixo:

1.  **Crie um novo arquivo JSON** no diretório `/src/content/posts/`. O nome do arquivo deve ser descritivo e seguir um padrão consistente (ex: `Nome-do-Artigo.json`).

2.  **Preencha o arquivo JSON** com as informações do artigo, seguindo a estrutura abaixo:

    ```json
    {
      "title": "Título do Artigo", // Título completo do artigo.
      "description": "Uma breve descrição do conteúdo do artigo.", // Descrição concisa do artigo.
      "link": "https://example.com/link-para-o-artigo", // URL para o artigo completo (Lattes, SOL SBC, etc.).
      "date": "YYYY-MM-DD" // Data de publicação do artigo no formato AAAA-MM-DD.
    }
    ```

    **Exemplo:**

    ```json
    {
      "title": "Argumentation Schemes for Stress Inference",
      "description": "This study reviews stress assessment models and proposes argumentation schemes for stress inference. Leveraging enthymematic reasoning, these schemes formalize patterns linking contextual, physiological, and psychological factors to stress attributions.",
      "link": "https://sol.sbc.org.br/index.php/bracis/article/view/40775",
      "date": "2025-09-29"
    }
    ```

3.  **Salve o arquivo.** O sistema de gerenciamento de conteúdo (Keystatic) irá automaticamente reconhecer o novo post.

## 4. Configuração e Desenvolvimento Local

Para configurar e executar o projeto localmente, utilize os seguintes comandos:

```bash
npm install
```

To run:

```
npm run dev
```

Homepage: [http://localhost:4321](http://localhost:4321)
