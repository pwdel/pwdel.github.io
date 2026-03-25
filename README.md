# pwdel.github.io

Root GitHub Pages site for the `pwdel` account.

## Local preview

From this directory:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000/`.

## Publish with GitHub CLI

```sh
gh repo create pwdel.github.io --public --source=. --remote=origin --push
gh api --method POST /repos/pwdel/pwdel.github.io/pages \
  -F 'source[branch]=main' \
  -F 'source[path]=/'
```

Expected production URL:

`https://pwdel.github.io/`
