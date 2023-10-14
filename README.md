## Git

- Initialise, with (initial) *branch name* being  **'main'**:

```sh
git init -b main
```

## Set repo

Set up 'origin' *remote* - (re: `add` and `set-url`)

```sh
git remote add origin https://github.com/$NAME_USER/$NAME_REPO.git

git remote set-url origin git@github.com:$NAME_USER/$NAME_REPO.git

# git remote -v |less  # // Can check
```

## Set name & email

```sh
git config user.email "$USER_EMAIL"
git config user.name "$USER_NAME"
```

## Set SSH key

```sh
git config gpg.format ssh
git config user.signingkey ~/.ssh/id_ed25519.pub
```

## WORKFLOW

```sh
git add .

# // NOTE: `-S` for *signing* a commit
git commit -S -am "Message..."