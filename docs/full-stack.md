**Running in dev mode**

Note for OS X users: if `pocketbase` does not run, it's probably your [security settings](https://support.apple.com/guide/mac-help/open-a-mac-app-from-an-unidentified-developer-mh40616/mac).

**Prerequisites**

```bash
brew install caddy
```

Then:

```bash
git clone git@github.com:benallfree/pockethost.git
cd pockethost
yarn
cp .env-template .env # modify as needed, if you used `pockethost.test` for your local domain, everything should work

yarn dev
open https://pockethost.test
open https://pockethost-central.pockethost.test
  # login: admin@pockethost.test (change in .env)
  # password: admin@pockethost.test (change in .env)
```