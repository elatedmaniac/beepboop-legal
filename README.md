# BeepBoop public policy site

Standalone Jekyll website for BeepBoop (formerly HomeBots), operated by
ElatedManiac in Washington, USA. This repository contains only the public
homepage, policy drafts and site assets. The agent harness is maintained
separately.

## Publication

GitHub repository: https://github.com/elatedmaniac/beepboop-legal

GitHub Pages uses `main` and `/ (root)` as its publishing source. Jekyll builds
Markdown and Liquid automatically; do not add `.nojekyll`.

- Homepage: https://elatedmaniac.github.io/beepboop-legal/
- Privacy: https://elatedmaniac.github.io/beepboop-legal/privacy/
- Terms: https://elatedmaniac.github.io/beepboop-legal/terms/

The pages remain **drafts**, with no effective date. Encryption at rest and
complete data-deletion validation remain unresolved. An owner-approved host
workflow handles primary stores; residual copies still require manual review.
Shared corpus contributions remain by default, while creator-owned session files
are deleted even in shared threads. Required shared-content removals remain
subject to owner review and applicable privacy/platform obligations.
Publishing this site does not establish compliance or verify the Discord app.
Keep `draft: true` until the stated commitments can be met and the policy review
is complete. The draft banner and `noindex` hint do not make the site private.

## Editing

Edit `index.md`, `privacy.md`, or `terms.md`, commit and push. Shared public
settings are in `_config.yml`: operator, location, contact, minimum age, effective
date and draft status. The public contact is `privacy@elatedmaniac.io`; forwarding
is configured separately from this repository and does not provide an outbound
mail identity. No tokens or credentials belong here.

There are no scripts, trackers or externally hosted fonts. Layout and appearance
live in `_layouts/default.html` and `assets/`.

## Build locally

From this directory on a rootless Docker host:

```sh
docker run --rm --user 0:0 -v "$PWD:/site" -w /site ruby:3.3 \
  bash -lc 'bundle install && bundle exec jekyll build --strict_front_matter'
```

The output is `_site/`, excluded from Git. GitHub's branch publisher provides its
own supported Jekyll environment; the Gemfile supports the independent local
build. Preview generated files through a local HTTP server so origin-relative
links and the Content Security Policy work as they do on Pages.

## Optional custom domain

Verify ownership and configure the domain in GitHub's Pages settings before
creating its DNS record. A subdomain CNAME targets `elatedmaniac.github.io`, with
no repository path. Set `url` to the custom HTTPS origin and `baseurl` to `""`,
then enable HTTPS once its certificate is ready. Keep the policy pages reachable
without authentication; review any Cloudflare Access default-deny setting for
that exact hostname. No custom domain is configured by the source files here.

After the policies are ready to take effect, set their effective date and update
the Discord Developer Portal and bot onboarding/help with the final public URLs.

References: [GitHub Pages publishing](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site),
[custom domains](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site).
