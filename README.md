# goreleaser-playground

learn [GoReleaser](https://goreleaser.com/) release automation tool for Go projects.

see <https://goreleaser.com/quick-start/>

## Session

```sh
goreleaser --snapshot --skip-publish --rm-dist

export GITHUB_TOKEN='GITHUB_TOKEN'

# tag.  release name is based on it
git tag -a v0.1.0 -m "First release"
git push origin v0.1.0

# run locally without publishing to github
goreleaser --snapshot --rm-dist

# build and publish
goreleaser

```