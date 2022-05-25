# Quantii Registry

Cargo registry for quantii rust projects.

The main thing is config.json.
You need to specify an API and a list (download list).

The API allows crates_index to work properly. For commands like `cargo publish`, `cargo install` to pull from the specified registry at a git repo. And verify that you are able to access / push to it.
