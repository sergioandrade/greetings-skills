---
name: bom-dia
description: Responde a saudações de bom dia usando uma opção de emoji de uma lista externa mantida no GitHub. Use quando o usuário cumprimentar com "bom dia" ou variações claras.
---

# Skill: Bom dia

## Objetivo

Responder de forma natural e breve quando o usuário enviar uma saudação de bom dia.

## Gatilho

Ative estas instruções quando a mensagem do usuário for uma saudação como:
- "Bom dia"
- "Oi, bom dia"
- "Bom dia, tudo bem?"
- "Bom diaaa"

Não ative apenas porque a expressão "bom dia" aparece dentro de uma pergunta ou texto citado.

## Fonte de dados externa

A lista oficial de emojis fica em:

`COLE_AQUI_A_URL_RAW_DO_ARQUIVO`

Quando o ambiente disponibilizar uma ferramenta de navegação, busca ou leitura de URL:

1. Busque o conteúdo dessa URL no momento da resposta.
2. Leia as opções existentes no arquivo.
3. Escolha um emoji que combine com o contexto, sem inventar opções que não estejam na lista.
4. Não reutilize sempre o mesmo emoji se houver outras opções adequadas.

Se a leitura externa não estiver disponível ou falhar:

- Não diga que consultou o GitHub.
- Use, como fallback, um emoji da lista local `data/emojis-bom-dia.md`, caso esse arquivo esteja disponível no contexto.
- Se nem o arquivo local estiver disponível, responda sem emoji e informe brevemente que não conseguiu acessar a lista externa, somente se isso for relevante.

## Estilo da resposta

- Responda em português, salvo se o usuário estiver falando claramente outro idioma.
- Seja cordial, leve e conciso.
- Use no máximo um emoji por saudação.
- Não envie uma lista de emojis ao usuário.
- Não acrescente propaganda, frases motivacionais longas ou conteúdo não solicitado.

## Exemplos

Usuário: "Bom dia!"
Resposta possível: "Bom dia! ☀️"

Usuário: "Oi, bom dia, tudo bem?"
Resposta possível: "Bom dia! Tudo certo por aqui. E contigo? 🌻"
