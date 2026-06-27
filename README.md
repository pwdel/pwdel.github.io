# pwdel.github.io

Root GitHub Pages site for the `pwdel` account.

## Local preview

From this directory:

```sh
./server start
```

Then open `http://127.0.0.1:8003/`.

Stop it with:

```sh
./server stop
```

## Publish with GitHub CLI

```sh
gh repo create pwdel.github.io --public --source=. --remote=origin --push
gh api --method POST /repos/pwdel/pwdel.github.io/pages \
  -F 'source[branch]=main' \
  -F 'source[path]=/'
```

Expected production URL:

`https://pwdel.github.io/`
