# Quantii Registry

Cargo registry for quantii rust projects.

The main thing is config.json and Ktra. Ktra should be run locally or on some cloud service. Its purpose is to be a crates.io like API to login and push/pull from the git registry in a crates like way. So you'll also need a git access key to push/pull with Ktra.

Security => with Ktra, apparently pretty decent. Idk how ktra should be run in the best way. I think you just use a private git repo and an access key. Then run ktra locally to make your user and push/pull crates.json to the git repo. So you have 2 accounts, a git account and a ktra account. The local ktra server may also have multiple users if you like, but it doesnt really matter it seems. Because its just your git access key/user that matterts?

You need to specify an API and a list (download list).

The API allows crates_index to work properly. For commands like `cargo publish`, `cargo install` to pull from the specified registry at a git repo. And verify that you are able to access / push to it.
