---
name: dayzy
description: Work with the configured Dayzy account to list or manage boards and cards. Use for any Dayzy question or action.
---

# Dayzy

Use the Dayzy API at `https://fizzy.estoreautomate.com` for account `1`.

- Require `DAYZY_TOKEN` in the environment. Never ask for it in chat or store it in a repository.
- Send `Authorization: Bearer $DAYZY_TOKEN` and `Accept: application/json` with every request.
- Use account-prefixed API paths, including `/1/boards`, `/1/cards`, and `/1/boards/:board_id/cards`.
- Read requests are allowed when requested. Before creating, changing, or deleting anything, state the exact action and get confirmation unless the user explicitly requested it.
- Prefer `curl -sS` for a single request and return relevant fields rather than raw payloads.

The Channel Bay board ID is `03gks684fzfmk2e2t5j1kgsn5`.
