---
created: 2025-01-02T16:29
updated: 2025-01-18T13:04
---
# **Repositório de conteúdos para as redes sociais**

Este repositório funciona como um **backup centralizado e organizado** de todo o conteúdo que produzo para redes sociais. Aqui você encontrará:
- ✍️ **Textos e slides** para posts
- 🔗 **Links úteis** e referências
- 📅 **Histórico de publicações**
- 💡 **Ideias e rascunhos** para conteúdo futuro

## 📂 **Estrutura**

O conteúdo está organizado nas seguintes categorias:
- /archives     → Conteúdo finalizado e publicado
- /drafts         → Rascunhos e ideias em desenvolvimento
- /scheduled  → Conteúdo finalizado e agendado para publicação
- /template    → Templates para as notas
- /theme        → CSS que customizam as notas

## 🗒 **Desenvolvimento**

Uso o Obsidian para criar e organizar postagens, com os plugins listados em [plugins-obsidian](plugins-obsidian.md). O fluxo de desenvolvimento está representado a seguir:

```mermaid
flowchart TD

    A["➕ Criar diretório em 'drafts' <br><small>(✏️ yyyyMMDD-tema-da-postagem)</small>"] --> B["➕ Adicionar uma nova nota"]

    B --> C["📥 Adicionar o template<br><small>(🔌Templater ➡️ 🗒<i>nota</i>)</small>"]

    C --> D["✏️ Preencher metadados<br><small>(YALM)</small>"]

    D --> E["👩‍💻 Desenvolver o conteúdo"]


    n4["📅 Agendar postagem"] --> n5("Mover para 'scheduled'<br><small>(📂drafts ➡️ 📂scheduled)</small>")

    n3{"Postado?"} -- sim --> n6("Mover para 'archives'<br><small>(📂scheduled ➡️ 📂archives)</small>")

    n5 --> n3

    E --> n4


    %% Estilos para os nós
    style A fill:#E3F2FD,stroke:#1E88E5
    style B fill:#E3F2FD,stroke:#1E88E5
    style C fill:#BBDEFB,stroke:#1E88E5
    style D fill:#BBDEFB,stroke:#1E88E5
    style E fill:#C8E6C9,stroke:#2E7D32
    style n4 fill:#FFF9C4,stroke:#F9A825
    style n5 fill:#FFF9C4,stroke:#F9A825
    style n3 fill:#FFD54F,stroke:#FF6F00,stroke-width:2px,shape:decision
    style n6 fill:#B2DFDB,stroke:#00796B

```

 
## 🤝 **Contribuições**

Sugestões e feedback são bem-vindos através das *issues*!

## 📝 **Licença**

Este conteúdo está sob licença MIT. 
Consulte o arquivo [[LICENSE]] para mais detalhes.
