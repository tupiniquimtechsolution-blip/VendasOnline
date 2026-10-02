# Security Policy

## Segredos

Nunca faça commit de:

- API keys;
- access tokens;
- refresh tokens;
- senhas;
- cookies;
- private keys;
- service-account credentials;
- arquivos .env reais.

Use secret manager ou variáveis de ambiente protegidas.

## Se um segredo for exposto

1. Revogue imediatamente.
2. Gere um novo segredo.
3. Verifique logs/uso.
4. Atualize somente o secret manager.
5. Não registre o valor antigo ou novo neste repositório.

## Aplicação futura

O frontend nunca deverá receber segredos de providers.

Credenciais de marketplaces, ads e APIs deverão permanecer no backend/worker e com escopo mínimo necessário.

## Pesquisa e compliance

Antes de automatizar coleta:

- validar documentação oficial;
- termos de uso;
- limites de API;
- permissões de armazenamento;
- dados pessoais envolvidos.

## Vulnerabilidades

Até o início do desenvolvimento, este repositório contém principalmente documentação.

Quando código for introduzido, adicionar processo de:

- dependency audit;
- secret scanning;
- SAST;
- atualização de dependências;
- revisão de permissões;
- CI security gates.
