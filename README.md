# compile

The build pipeline for Crafted Resistance. **There is no game code in this repository.**

GitHub Actions are billed on a private repository and free on a public one, so the
build runs here while the code stays private: `.github/workflows/build.yml` checks the
code out at run time with a token, builds the launchers and installers, and publishes
them to a release. Nothing is ever written back to this repository.

- The game code lives in a private repository.
- The downloads live on the website's release.
- A build is staged privately unless the `PUBLISH` variable says otherwise.

Run it from the **Actions** tab.
