# Convenções

## Git — títulos de commit/push/PR

Padrão Conventional Commits: `<tipo>(<escopo>): <descrição no imperativo, minúscula, sem ponto final>`

Tipos: `feat`, `fix`, `refactor`, `perf`, `style`, `test`, `docs`, `build`, `ci`, `chore`, `db`, `revert`.

- Escopo obrigatório quando dá para identificar a área.
- Título com no máximo 72 caracteres.
- Breaking change: `!` antes dos dois pontos e rodapé `BREAKING CHANGE: <explicação>`.
- Corpo explica o quê e por quê, não o como.
- Título de PR segue o mesmo padrão.

## Supabase — migrations

Não se aplica a este projeto (site estático), mas, se surgir banco: arquivo `supabase/migrations/<timestamp>_<nome_snake_case>.sql`, cabeçalho comentado (MIGRATION, TÍTULO, DESCRIÇÃO, AUTOR, DATA, IMPACTO, REVERSÍVEL), rollback comentado ao final, commit com tipo `db`.
