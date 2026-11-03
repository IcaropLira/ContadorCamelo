# Contador Camelo

Site que conta as faltas de Gabriel Camelo nas cadeiras da UFCG.

## Como atualizar

Edite o arquivo [`faltas.md`](faltas.md) no formato:

```
Cálculo 2 : 3
Linear : 1
```

- O número é de **dias** de falta.
- O site multiplica por 2 para mostrar o total de faltas.
- Para incluir uma cadeira nova, adicione uma linha nova.
- Linhas que começam com `#` e linhas em branco são ignoradas.

Ao salvar o commit na branch `main`, o GitHub Actions republica o site automaticamente.

## Publicação (GitHub Pages)

Em **Settings → Pages**, escolha **Source: GitHub Actions** (só na primeira vez).
O site fica em https://icaroplira.github.io/ContadorCamelo/

## Rodar localmente

```
python3 -m http.server
```

Abra http://localhost:8000 (abrir o `index.html` direto do disco não funciona, porque o navegador bloqueia a leitura do `faltas.md`).
