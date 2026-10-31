# Contributing to NetRadar

Thanks for helping improve NetRadar! Contributions are made through pull requests.

## How to contribute

1. **Fork** the repository and create a branch from `main`
   (e.g. `fix-dca-recovery`).
2. Make your change. Keep pull requests focused on one topic.
3. Run what you can locally (`bash -n` on shell scripts, `python -m compileall`
   on Python code; for the docs, `mkdocs build --strict`).
4. **Open a pull request** against `main` and fill in the template.

`main` is protected: nobody pushes to it directly. Every change needs a passing
check run (including a secret scan) and a maintainer's approval before it is
merged.

## Never commit secrets or private details

Do not include passwords, Tailscale auth keys, API tokens, `.env` files,
`nanomq/auth/` files, IP addresses or host names of your own deployment, or
personal data. The secret scan will block the pull request, and anything pushed
to a public repository should be considered leaked — rotate it immediately.

## Reporting bugs and asking questions

Open an issue in the relevant repository. Include what you ran, what you
expected, and the relevant log output (with passwords and addresses removed).

Security problems: please report them privately — see `SECURITY.md`.

## Licence

By contributing, you agree that your contributions are licensed under the
Apache License 2.0, the licence of the project.
