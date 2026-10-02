# clamk-tools.github.io

The hub at <https://clamk-tools.github.io/>. It lists every repo in the
[clamk-tools](https://github.com/clamk-tools) org that has the topic `tool`.

## Add a tool to the hub

No change here is needed. On the tool's repo page, click the gear next to **About** and:

1. Add the topic `tool`.
2. Set **Website** to its Pages URL (`https://clamk-tools.github.io/<repo>/`).
3. Write a one-line description; it becomes the card text.

## Publishing safely

This repo is public. `.githooks/check-privacy.sh` blocks a commit or push that carries a non-noreply email,
a private local path or a secret, and CI runs the same check on every push and PR. Turn it on once per clone with
`git config core.hooksPath .githooks`, and commit with a GitHub noreply address. It reports `file:line` only,
never the offending text. A line holding an invented example can carry the marker `privacy-ok` in a comment.

## Hosting

Plain HTML, no build. Settings → Pages → Deploy from a branch → `main` / root.
The org name lives in the `ORG` constant in `index.html`.
