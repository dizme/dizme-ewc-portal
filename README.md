<div align="center">
 <h1>Credential Issuance & Verification Portal</h1>
 <span>by </span><a href="https://dizme.io">Dizme</a>
 <span>Forked from </span><a href="https://walt.id">walt.id</a>
 <p>Sample application that showcases the issuance and verification of W3C Verifiable Credentials<p>
</div>

## Getting Started

First, run the development server:

```bash
pnpm dev
```

Build for production

```bash
pnpm build
```

Using Docker:

```bash
docker build -t dizme/portal -f Dockerfile .
docker run -p 7102:7102 -i -t dizme/portal
```
or, with environment variables:
```bash
docker run  --name dizme-portal -p 3001:3000 \
    -e NEXT_PUBLIC_VC_REPO="http://localhost:3000" \
    -e NEXT_PUBLIC_ISSUER="https://issuer.portal.walt-test.cloud" \
    -e NEXT_PUBLIC_VERIFIER="https://verifier.portal.walt-test.cloud" \
    -e NEXT_PUBLIC_WALLET="https://wallet.walt-test.cloud" \
    -i -t dizme/portal
```

## Join the community

* Connect and get the latest updates: <a href="https://discord.gg/AW8AgqJthZ">Discord</a> | <a href="https://walt.id/newsletter">Newsletter</a> | <a href="https://www.youtube.com/channel/UCXfOzrv3PIvmur_CmwwmdLA">YouTube</a> | <a href="https://mobile.twitter.com/walt_id" target="_blank">Twitter</a>
* Get help, request features and report bugs: <a href="https://github.com/walt-id/.github/discussions" target="_blank">GitHub Discussions</a>

## License

**Licensed under the [Apache License, Version 2.0](https://github.com/walt-id/waltid-ssikit/blob/master/LICENSE).**
