## keepassweb

This organization is not the KeePass Web application. The application is
[KeePass Web](https://keepass-web.app/), built and maintained by the
[keepass-web](https://github.com/keepass-web) organization — note the
hyphen, which is the whole reason this organization exists.

### Why this organization exists

Password managers are a common target for lookalike domains: a name a
letter or a hyphen off from the real one, hosting a copy of the login
page to collect credentials. `keepassweb` and `keepass-web` differ by
exactly one character. Rather than leave that name, and others like it,
available for someone else to register, this organization holds them and
watches for further lookalikes appearing elsewhere.

### What it does

- Holds domains and GitHub Pages sites that could otherwise be used to
  impersonate KeePass Web, and serves an identical parked page from each
  one, stating that the domain is parked and linking to
  [keepass-web.app](https://keepass-web.app/).
- Scans periodically for newly registered domains similar to
  `keepass-web.app`, and opens an issue with evidence when one is found
  serving content that resembles the KeePass Web brand.

### How it does it

- [`parked-domain-tools`](https://github.com/keepassweb/parked-domain-tools) —
  syncs the parked-page template from
  [`keepass-web/keepass-web.github.io`](https://github.com/keepass-web/keepass-web.github.io)
  across every domain listed in its manifest, and keeps each repo's
  GitHub Pages configuration correct.
- [`lookalike-monitoring-tools`](https://github.com/keepassweb/lookalike-monitoring-tools) —
  runs the scheduled scan for lookalike domains and opens an issue when
  one needs a closer look.

Questions about a specific repo belong on that repo's issue tracker.
