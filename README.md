# Discussify

Discuss the web.

## Installing

Currently Discussify is available as a browser extension. Check its [repository](https://github.com/ipfs-shipyard/discussify-browser-extension) for installation instructions.

## Planning

*Note that all planning happens under [`project/design/planning`](project/design/planning).* Check [Contributing](#contributing) if you're interested in collaborating.

[💡 Concept](project/design/planning/concept.md)  
[🌈 Features](project/design/planning/features.md)  
[📈 SWOT Analysis](project/design/planning/swot.md)  
[👨‍👩‍👧‍👦 Audience](project/design/planning/audience.md)  
[📇 Business Model Canvas](project/design/planning/business-model-canvas.md)  
[💎 Brand Identity](project/design/planning/brand-identity.md)  
[📱 Prototype](project/design/planning/prototype.md)  

## Team

- [André Cruz](https://github.com/satazor) - Software engineer
- [André Sousa](https://github.com/andreforsousa) - Designer
- [Marco Oliveira](https://github.com/marcooliveira) - Product engineer
- [Pedro Santos](https://github.com/PedroMiguelSS) - Software engineer
- [Pedro Teixeira](https://github.com/pgte) - Project manager / [`peer-star-app`](https://github.com/ipfs-shipyard/peer-star-app) support


## Contributing

All work is organised on GitHub, through issues and this repository. We use [Waffle](https://waffle.io/ipfs-shipyard/pm-discussify) to organize ourselves and to plan sprints.

Every commit should be following [Conventional Commits](https://conventionalcommits.org/) guidelines. To avoid mistakes, there's a precommit hook that will validate all commits made to this repository. Please run `$ npm install` in your terminal before committing.

### Design

If you'd like an overview of the project folder structure, have a look at the [Design Workflow](design-workflow.md).

Note that all planning happens under [`project/design/planning`](project/design/planning).

### Codebase

The codebase lives in separate GitHub repositories:

- [`discussify-styleguide`](https://github.com/ipfs-shipyard/discussify-styleguide) - React components shared by the browser-extension, the web app and the iframe/embed.
- [`discussify-browser-extension`](https://github.com/ipfs-shipyard/discussify-browser-extension) - Discussify's browser extension app

## Roadmap

### POC phase 1:

Key goals:
  - [x] Develop a browser extension.
  - [x] Authentication using uPort until "POC phase 2".
  - [x] Ability to view a discussion happening on the current webpage.
  - [x] Create, remove, edit comments.
  - [x] Reply comments.
  - [x] Release for BETA testing.

### POC phase 2:

Key goals:

- [ ] Ability for users to authenticate themselves using the strategy outlined in [this RFC](https://github.com/ipfs-shipyard/peer-star/pull/15).
    - Effort is underway to develop this, under [IDM](https://github.com/ipfs-shipyard/pm-idm).
- [ ] Verify ownership of the comments via signatures, also detailed in the RFC.
    - Discussions [here](https://github.com/ipfs-shipyard/peer-star-app/issues/4#issuecomment-411109427).
- [ ] Ability to verify user's identities, including their claims & proofs.
- [ ] Ability to view comment history such as edits and removals.

### MVP

Key goals:

- [ ] Ability to view discussions I have participated in the past, including receiving notifications about new activity on any of them.
- [ ] Guarantee the persistency of the data by integrating the pinner.

### v1.0.0

Key goals:

- [ ] Ability to discuss on specific parts of the page, using [Web Annotations](https://www.w3.org/annotation/).
- [ ] Ability to have private discussions, with support for inviting and kicking users.
    - [Several discussions around ACL and capabilities](https://github.com/ipfs/dynamic-data-and-capabilities/issues?utf8=%E2%9C%93&q=is%3Aissue+is%3Aopen+acl).
- [ ] Ability to subscribe/mute discussions.
- [ ] Ability to invite other people to a public discussion, even if the invitee does not have Discussify installed. This would potentially mean creating a protocol for inviting for a generic collaboration, through IDM, which would require installing an additional app.
- [ ] Ensure that it's performant, stable and not resource hungry.
- [ ] Define (and execute) a plan for the launch of Discussify as a decentralized product.

## Privacy Policy

You can find and read our privacy policy [here](/PRIVACY_POLICY.md).
