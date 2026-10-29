## Hi, I'm Brian

I'm studying Accounting and Finance at LSE, but most of my spare time goes into building things: apps, bots, AI agents, and lately a few hackathons. I started coding to test trading ideas properly and never really stopped. Building things turned out to be the part I enjoy most.

### Things I've built

**[NorthStar](https://github.com/TheIntrinsicInvestor/Nebius-x-Noetic-Hackathon)** ([live demo](https://northstar-lovat-eight.vercel.app))<br>
Covenant early warning for mid-sized companies, built in a day with a teammate at the Noetic x Nebius hackathon. Firms with $10m to $500m of revenue carry real bank debt but rarely have a treasury team, so they often find out about a covenant breach after the quarter has closed. You upload the loan agreement and management accounts, and it reads the covenants, maps the accounts, projects six quarters and shows how close each covenant gets to its limit, with sliders and plain-English what-if questions. The one rule: the language model never produces a number on screen. Open-weight models on Nebius do the reading and a deterministic Python engine does the maths. Replaying Nortech Systems from its SEC filings, it forecast a breach while leverage still showed 30% headroom, and the company breached at its next test.

**[Timbre Care](https://github.com/TheIntrinsicInvestor/timbre-care)** ([live demo](https://timbre-care.edgeone.dev))<br>
An AI care agent for older people who live alone, built with a teammate for Tencent Cloud's Age Well hackathon. It writes up doctor's appointments in plain language as they happen and makes a short check-in call each day. Under the hood it's an MCP server with 17 tools and two agent skills, and the guardrails are enforced in those tools rather than in the prompt. If the agent tries to downgrade something urgent, the tool refuses and tells it which rule it broke.

**[Condition Desk](https://github.com/TheIntrinsicInvestor/condition-desk)**<br>
My build for NEBULA X, a rail hackathon run by LTA with SMRT, SBS Transit and Google Cloud. Four ML models, one per train subsystem, work on raw sensor and vibration recordings and sit behind a FastAPI and Next.js app. The model report says where my own scores are probably too optimistic, and why.

**[Everesteer Hedge Fund Hackathon](https://github.com/TheIntrinsicInvestor/everesteer-hackathon)**<br>
A live prediction tournament at LSE: predict forward returns on futures baskets, then stake money on your own models over four 20-minute rounds. The write-up is a post-mortem. I'd picked my training window on a practice board that covers a single period, which overfits; a four-block forward test I built mid-event showed that every variant using more history or more regularisation beat it, and the live rounds ended up agreeing. It also covers the round where I ignored that evidence to chase a top-3 place, and what that cost.

**[Bank Well church switch](https://github.com/sspencespence/ftbuild-bank-well-church-switch/tree/sortcode-db)** (team project, FaithTech BUILD 2026)<br>
We wanted to find out where UK churches keep their money, for Bank Well's push to get them onto banks with higher ESG ratings. Lots of churches never name their bank in their filings, but many print a sort code on their giving page. I wrote the crawler that collects those codes and a lookup that maps each one to the bank behind it, including agency codes you'd get wrong from the first two digits. I also did the cleaning, used Claude subagents to review the borderline rows (then checked their labels with a script), and cross-checked everything against OpenStreetMap. Of the 2,185 churches we could confirm, half bank with the lowest ESG-rated banks.

**[AI Equity Research](https://github.com/TheIntrinsicInvestor/ai-equity-research)**<br>
An LLM pipeline that writes sell-side style research reports from institutional data. The first pass, Claude Sonnet with tool calling, builds a thesis without seeing the rules-based score. The second, Claude Opus, has to compare the two and explain where it disagrees. FinBERT scores the sentiment of each earnings release. I split it that way because when the model sees the score first, it tends to write a story around it.

**[RunLoop](https://github.com/TheIntrinsicInvestor/runloop-app)** (iOS app, personal project)<br>
Pick a distance and a start point and it plans a proper loop: you finish where you started without retracing the same streets. Routes come from a GraphHopper server I host myself, covering Singapore and the San Francisco Bay Area, and it can rank them by total climb if you'd rather avoid hills. During a run, a Live Activity keeps distance, time and pace on the lock screen. Built in React Native with Expo, with a FastAPI route service behind it.

**[Remix Web](https://github.com/TheIntrinsicInvestor/remix-web)** (web and iOS app, personal project)<br>
Turns a song into a backing track for covers. Give it a YouTube or Spotify link or upload a file, and it splits the song into stems with Demucs, then pitch-shifts, time-stretches and adds effects. Underneath is a Python toolkit I drive by describing the sound I want to Claude, which writes the recipe and runs it. FastAPI backend on my server, Next.js frontend.

**[Telegram Expense Tracker](https://github.com/TheIntrinsicInvestor/telegram-expense-tracker)**<br>
A budgeting bot I run for myself and a few friends. You text it something like `15 lunch` and it logs it, and if it guesses the category wrong it remembers your fix. Reports compare your spending with what you'd usually have spent by that day of the month, so paying rent on the 1st doesn't make every month look like a disaster.

I've also made a live F1 timing screen. If I keep wishing something existed, I usually end up building it, and most of these run on a small server I look after.

### Hackathons

So far: Tencent Cloud's Age Well challenge, NEBULA X, FaithTech BUILD, Noetic x Nebius and Everesteer's hedge fund hackathon at LSE. I like having a weekend and a real problem to work on, and I'm keen to do more in London, especially anything with AI agents or something people will use once the weekend's over.

### Finance

I still like finance and build in it too. I backtest options and volatility ideas on institutional data and post the results on [theintrinsicinvestor.com](https://theintrinsicinvestor.com), including the ones that didn't work. The code is in [Backtesting](https://github.com/TheIntrinsicInvestor/Backtesting).

### How I work

I build a lot with Claude Code, often with several subagents working in parallel on research, testing and review. I care more about whether the result is right than who typed each line, so I write the spec, read the code, run it and check the output. If a number looks too good, I assume I've made a mistake somewhere.

What I use most: Python, TypeScript, FastAPI, Flask, Next.js, React Native (Expo), the Claude API and MCP, pandas, and a Linux server I deploy to.
