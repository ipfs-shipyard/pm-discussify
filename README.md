# Discussify

Discuss the web.

*Note that all planning happens under [`project/design/planning`](project/design/planning).*

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

### POC - phase 1:

Key goals:
  - Develop a browser extension
  - Authentication using uPort until "POC - phase 2"
  - Ability to view a discussion happening on the current webpage
  - Create, remove, edit comments

Approximate end date: 21th September

### POC - phase 2:

Key goals:

- Ability for users to authenticate themselves using the strategy outlined in [this RFC](https://github.com/ipfs-shipyard/peer-star/pull/15)
- Verify ownership of the comments via signatures, also detailed in the RFC

Approximate end date: 19th October   
Desired end in time: 12th October because [MozFest](https://mozillafestival.org/) is happening 22nd-28th October

### MVP

Key goals:

- Capabilities, ensuring the changes performed by users are allowed
- Ability to view discussions I've participated
- Ability to know which discussions have new comments or replies

Approximate end date:

### v1

Key goals:

- Ability to discuss on specific parts of the page, using [Web Annotations](https://www.w3.org/annotation/)
- Ability to have private discussions
- Have a stable product with replication integrated

Approximate end date:
