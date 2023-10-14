## Git

- Initialise, with (initial) *branch name* being  **'main'**:

```sh
git init -b main
```

## Set repo  

- Add 'origin' *remote* - (re: `add` and `set-url`)

    - NOTE: `git@github.com` (for SSH authentication)

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

- Add files to 'staging area':

```sh
git add .
```

- Commit, with a message

    - NOTE: `-S` for (SSH) *signing* a commit

```sh
git commit -S -am "Message..."
```

- Push!

```sh
git push origin main
```


