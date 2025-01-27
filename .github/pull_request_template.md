# Harmony Swap Token List

Token name: <!-- name of the token -->

## Requirements

- [ ] Is `.json` well formated?
- [ ] Does branch open well in [https://tokenlists.org/](https://tokenlists.org/)? example: `https://tokenlists.org/token-list?url=raw-tokenlist.json-url`
  - Grab the raw `tokenlist.json` file URL from the pull request and replace it in the `?url=` parameter above
- [ ] Is the contract verified?
- [ ] Does `name`, `decimal` and `symbol` data match contract data?
- [ ] Is version incremented?
  - Check the version field of the proposed `tokenlist.json` file. If token is being added then bump in minor, if token is being edited then bump in patch
- [ ] Is icon file present?
  - It's ok if the logo doesn't render in the proposed URL, but it has to be present in the PR
