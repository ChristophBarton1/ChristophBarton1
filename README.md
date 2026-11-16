<a href="https://christophbarton.com"><img src="assets/head.jpg?v=2" width="100%" alt="Christoph Barton, full-stack developer in Vienna. I build web products end to end and keep them running. Six years in web teams. Four of my own products, built next to a full-time job: CookFuse (a grocery receipt becomes a pantry and recipes), ggez.gg (20 million matches a month), Earth Mood News (215 countries, every hour) and PromptShelf (reusable prompts, in development)." /></a>

I'm a full-stack developer in Vienna. For six years I have built websites and web applications in small teams. Next to my job I build my own products and keep them running. Most of my code is in private repositories, so this page describes the work instead of linking to it.

<br/>

### My own products

**[ggez.gg](https://ggez.gg)** is a statistics site for League of Legends and Teamfight Tactics with an AI coach. A collector takes in about 20 million matches a month from the Riot Games API into a self-hosted ClickHouse, and the site is rendered in 9 languages on Cloudflare. Live since December 2025. The current figures are public at [ggez.gg/data](https://ggez.gg/data).

**[CookFuse](https://cookfuse.app)** turns a photo of a grocery receipt into a pantry. Groceries are recognised on the device, tracked by shelf life and turned into recipes before they spoil. React Native, Expo, Cloudflare Workers and D1.

**[Earth Mood News](https://earth-mood-news.vercel.app)** is a globe coloured by the tone of each country's headlines. A scheduled job collects and scores the news of about 215 countries every hour. React, D3 and GitHub Actions.

**PromptShelf** saves prompts and turns them into reusable mini-tools with variables. SvelteKit, Cloudflare D1 and Drizzle. Private and still in development.

**[STS2 Hub](https://sts2-hub.pages.dev)** is a fan-made companion for Slay the Spire 2 with a deck builder, a card database, a tier list and guides in nine languages. SvelteKit and Tailwind on Cloudflare. The [code is public](https://github.com/ChristophBarton1/Slay-the-Spire-2-Plattform-Free).

Two smaller tools are public: **[Context Grabber](https://github.com/ChristophBarton1/Context-Finder)**, a browser extension for one-click bug reports with console errors, failed requests and the selected element, and **[Multi-Agent Terminal](https://github.com/ChristophBarton1/Multi-Agent-for-Terminal-Claude-Open-Ai-Grok)**, a Claude Code hook that asks ChatGPT and Grok the same question in parallel and hands Claude their answers.

<a href="https://ggez.gg"><img src="assets/card-ggez-top.svg" width="100%" alt="ggez.gg: League of Legends stats, builds, tier lists and an AI coach" /></a>
<a href="https://cookfuse.app"><img src="assets/card-cookfuse-shot.svg" width="100%" alt="CookFuse: receipt to pantry to recipes" /></a>
<a href="https://earth-mood-news.vercel.app"><img src="assets/card-earthmood-turn.svg" width="100%" alt="Earth Mood News: a rotating globe coloured by the tone of each country's news" /></a>
<img src="assets/card-promptshelf-shot.svg?v=2" width="100%" alt="PromptShelf: reusable prompts and mini-tools (private repository)" />
<a href="https://sts2-hub.pages.dev"><img src="assets/card-sts2-shot.svg" width="100%" alt="STS2 Hub: fan-made Slay the Spire 2 hub with deck builder, card database and guides" /></a>
<a href="https://github.com/ChristophBarton1/Context-Finder"><img src="assets/card-context-grabber.svg?v=3" width="100%" alt="Context Grabber: one-click bug reports for AI-built apps" /></a>
<a href="https://github.com/ChristophBarton1/Multi-Agent-for-Terminal-Claude-Open-Ai-Grok"><img src="assets/card-multi-agent.svg?v=3" width="100%" alt="Multi-Agent Terminal: Claude, GPT and Grok in parallel" /></a>

<sub>Private code can be walked through on request. Case studies for client work are on <a href="https://christophbarton.com">christophbarton.com</a>.</sub>

<br/><br/>

### How I work

- **Tests on every push.** ggez.gg runs more than 1,200 tests, a type-error budget that only goes down and Playwright layout checks. The chatbot plugin I built at work is tested with PHPUnit across PHP 7.4 to 8.3.
- **Releases that can be undone.** A build goes live only when CI is green, and server deploys roll back with one command.
- **Systems that run without me.** Collectors and scheduled jobs work around the clock. On ggez.gg a monitor checks the collector every fifteen minutes and mails me when a region falls behind. The database is backed up every night, and the restore is scripted and tested.
- **Careful with other people's limits.** The match collector reads its rate limits from the API's response headers, claims each match once and retries failures from a queue.
- **Decisions with a reason.** When ggez.gg's match data outgrew the 10 GB limit of its first database, I moved the analytics to a self-hosted ClickHouse. Statistics pages read aggregate tables built from it.
- **AI as a tool and as a feature.** I work with Claude Code every day. I have built an AI coach that answers from a player's own match data through tool calls, a chatbot for company websites and an MCP server for Moodle.

<br/>

### At work

**Full-stack developer at die Berater, Vienna, since 2023.** A team of three that chooses most of its own stack.

- An AI chatbot for the company's websites: a Next.js application with an admin back end, and a WordPress plugin in PHP.
- Moodle platforms, the largest with about 50,000 users: plugins, interfaces and an MCP server, plus work on data pipelines and server capacity.
- About 80 websites: custom PHP plugins, performance, SEO and server administration.

Before that I built client websites at Ghost Company (2021 to 2023) and front ends for web and hybrid mobile apps at Ameisenhaufen (2020 to 2021).

<br/>

### What I work with

**Every day:** TypeScript, SvelteKit, Next.js, Node.js, Cloudflare Workers, ClickHouse, SQL, PHP.

**In projects:** Vue and Nuxt, React Native and Expo, Hono, Drizzle, Turso, PostgreSQL, Docker.

<br/>

### Activity

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ChristophBarton1/ChristophBarton1/output/snake-dark.svg" />
  <img src="https://raw.githubusercontent.com/ChristophBarton1/ChristophBarton1/output/snake-light.svg" width="100%" alt="Contribution calendar" />
</picture>

<p>
  <a href="https://christophbarton1.github.io/ChristophBarton1/"><b>Play snake on my contribution graph &#8599;</b></a><br/>
  <sub>Most of my work happens in private client and product repositories. The calendar includes those contributions.</sub>
</p>

<br/>

### Contact

Open to full-time roles and freelance work in full-stack development. The best way to reach me is through [christophbarton.com](https://christophbarton.com).
