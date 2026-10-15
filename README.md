## Hi, I'm Brian

I build software that solves real problems, a lot of it with AI at the core. I study Accounting and Finance at LSE in London, and I write code because I'd rather build the thing than wait for someone else to.

### What I've built

**[Timbre Care](https://github.com/TheIntrinsicInvestor/timbre-care)** · AI care agent for elderly people living alone ([live](https://timbre-care.edgeone.dev))<br>
Built with a teammate for the Tencent Cloud Age Well hackathon. It's an MCP server with 17 tools that writes up doctor's visits in plain language and runs daily check-in calls. Its safety rules are enforced in code rather than in the prompt, so an agent that tries to lower an urgency gets refused, with the rule it broke.

**[Condition Desk](https://github.com/TheIntrinsicInvestor/condition-desk)** · ML condition monitoring for trains<br>
From the NEBULA X rail hackathon (LTA, SMRT, SBS Transit, Google Cloud). Four models for four train subsystems behind one FastAPI and Next.js app, plus a model report that spells out where its own scores are too optimistic.

**[Bank Well church switch](https://github.com/sspencespence/ftbuild-bank-well-church-switch/tree/sortcode-db)** · team project at FaithTech BUILD 2026<br>
Our team worked out where UK churches keep their money, for Bank Well's push to move it to ethical banks. Many churches never name their bank in their filings but print a sort code on their giving page. I built the crawler that finds those codes, a lookup that turns a code into the bank behind it (including agency codes that a first-two-digits lookup gets wrong), and the cleaning and cross-checks against OpenStreetMap. Result: of 2,185 confirmed churches, half bank with the lowest-rated high-street banks.

**[AI Equity Research](https://github.com/TheIntrinsicInvestor/ai-equity-research)** · LLM pipeline that writes research reports<br>
Two passes of Claude over institutional data. The first writes a thesis without seeing the rules-based score. The second has to reconcile the thesis with the score and say where it overrides it, so the model can't just build a story around a number it saw first.

**[Telegram Expense Tracker](https://github.com/TheIntrinsicInvestor/telegram-expense-tracker)** · a budgeting bot I run for myself and a few friends<br>
You text it `15 lunch` and it files the expense. It learns your category corrections and sends back report cards whose saving tips are based on what you normally spend, not on averages.

**Smaller tools for my own problems.** A mobile app that generates proper running loops. A live F1 timing screen. If I keep wishing something existed, I build it, and most of it runs on a server I maintain.

### Hackathons

I like a short deadline and a real problem. So far: the Tencent Cloud Age Well challenge, NEBULA X and FaithTech BUILD. I'm looking for more in London, especially ones about AI agents or products for real users.

### Finance, too

Finance is still a domain I enjoy building in. I backtest options and volatility ideas on institutional data and publish the results, including the ones that fail, at **[theintrinsicinvestor.com](https://theintrinsicinvestor.com)** ([source](https://github.com/TheIntrinsicInvestor/Backtesting)).

### How I work

I build fast with AI coding tools, mostly Claude Code, and I care more about whether the thing is correct than about who typed each line. I write the spec, read what gets written, run it, and check the output before I trust it. If a result looks too good, I assume I made a mistake first.
