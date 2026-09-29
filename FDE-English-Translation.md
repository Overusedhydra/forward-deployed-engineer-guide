# The Forward Deployed Engineer: The Secret to Delivering Customer Value in the AI Era

**By Fan Bing (XDash)**

---

## Preface

Last summer, my social media feed was flooded with the same number: 95%.

MIT NANDA Lab's 2025 report *The GenAI Divide* revealed that over the past three years, enterprises worldwide spent $30-40 billion on generative AI, yet 95% of projects failed to produce any value that could appear on a financial statement. Around the same time, another story was racing in the opposite direction: on Silicon Valley job boards, a position called "Forward Deployed Engineer" (FDE) saw postings increase more than sevenfold in a single year. OpenAI was hiring, Anthropic was hiring, and over a hundred startups in Y Combinator were hiring.

On one side, a 95% failure rate for enterprise AI projects; on the other, a position with 700%+ annual growth in demand. Put these two facts together and the answer is clear: **models are no longer scarce — the people who can embed models into real customer businesses are.**

I first seriously considered this role while reading Palantir's origin story. Founded in 2003, the company spent twenty years doing something the software industry considers stubborn: sending their best engineers to customer sites — intelligence agencies, battlefields, oil fields, factories — to write code knee-deep in customer data.

Wall Street didn't understand Palantir for years, dismissing it as "more like a consulting company." Then what happened? In 2025, its market cap surpassed $400 billion, and its Rule of 40 metric was so healthy that analysts were rewriting their research reports overnight.

Digging deeper, more clues emerged: OpenAI quietly built an FDE team in 2024; in May 2026, it partnered with 19 top-tier capital firms to launch a "deployment company" valued at $10 billion; Anthropic was reportedly forming a comparable joint venture with Blackstone on nearly the same day. The conclusion is hard to avoid: FDE is not a hiring fad — it is a regime change in how software is delivered.

### Why I Wrote This Book

For the past decade, I've been doing one thing: systematically explaining what's happening in Silicon Valley that doesn't yet have a name in China. FDE sits at a familiar inflection point — Silicon Valley has already written it into org charts, while most Chinese-language discussion still stops at "isn't this just pre-sales with a new name?"

I can say responsibly upfront: it's not. But what it actually is can't be explained in one sentence — you have to go back to where it was born. How Palantir was forced into this approach by intelligence agencies' security walls, how OpenAI engineers delivered AI in Iowa farm fields, how a startup called Harvey broke into elite law firms where even ordinary software couldn't enter, and the subtle relationship between China's enterprise software industry's chronic "project-based" curse and FDE.

To explain all this, I combed through every primary source I could find: 51-minute podcast retrospectives by early Palantir executives, memoirs by former employees, venture capital industry analyses, the original MIT report, dozens of job postings from various companies, salary reports, forum posts by practitioners, and interviews with China's first-wave practitioners. This book is the distillation of that research — and my judgment.

### How to Read This Book

Chapter 1 traces the full arc of this role: where it came from, what it is, and why now. Chapters 2-7 follow the complete journey of a real delivery — finding the right problem, winning the customer, activating deployment, retaining renewals, expanding revenue, and scaling replication.

Chapter 8 returns to the source, reconstructing several of the most fascinating field stories in full. The epilogue discusses the boundaries of this profession, and the appendices contain ready-to-use metrics, a directory of key people, and sources for all data and cases.

You are probably one of three types of readers: 1) an entrepreneur looking to enter enterprise AI — you'll see a playbook better suited to this era; 2) an engineer considering or currently doing FDE — you'll see the full picture and ceiling of this role; or 3) someone who simply wants to understand how AI can actually land in enterprises — this is the trillion-dollar question of our time, and this book aims squarely at it.

One final thought. Throughout writing this book, I kept returning to a simple truth: complex problems cannot be solved through a screen — someone has to show up. FDE simply turns this truism into a profession.

May this book help you move AI from the demo room into the real world.

Fan Bing
July 2026

---

## Chapter 1: The Rise of FDE

> "One challenge of building software for spies is: I don't know any spies."
> — Bob McGrew, early Palantir executive, former Chief Research Officer at OpenAI

### 1.1 First, a Story About a Million Dollars That Died

The beginning of the story is always the same. In a large enterprise's conference room, the vendor's demo has just concluded. The LLM answers fluently, the data dashboard gleams, and even the most demanding executives can't find fault. The CEO makes the decision on the spot: sign. Contract worth millions, handshakes, photos, press release.

Nine months later, the project is dead.

Not dramatically — silently. The system is still running, servers still on, but no business unit is actually using it. The vendor delivered every feature in the contract; the enterprise paid every dollar. The only thing that didn't arrive was "value."

If you think this was just bad luck, MIT NANDA Lab's 2025 report *The GenAI Divide* will tell you: this is the norm. They interviewed 52 organizations, collected 153 executive surveys, and reviewed 300+ public enterprise AI projects. The conclusion is one sentence: of the $30-40 billion poured in, **95% produced no measurable financial return.**

Before citing this 95%, we need to establish the methodology. After the report's release, criticism focused on three points:

1. It defines "failure" as no measurable financial statement impact within six months — by this standard, almost all early internet and cloud computing investments would be "failures";
2. Its value measurement only counts profit, cost, and revenue — leading indicators like process speed and employee adoption don't count;
3. The sample skews toward large enterprises, and failure data comes only from project sponsors. Some commentators also noted a conflict of interest: NANDA Lab itself is researching agentic internet, and the report's prescribed solution conveniently points in their own direction.

These criticisms are all valid, but none overturn the directional judgment: enterprise AI projects are broadly underperforming — independent research by RAND Corporation, S&P Global, and others paints the same picture. So when this book cites 95%, it takes the direction, not the precise figure; a failure rate precise to the decimal point is itself a kind of false precision.

More interesting is the manner of failure. The report specifically notes: the problem isn't the models. Those dazzling models remain smart in production — they just "don't remember feedback, don't retain context, don't enter workflows" — they look like products but feel like exhibits.

Stanford's aggregate data from the same year corroborates: 88% of organizations use AI, yet only single-digit percentages of agentic applications actually run in production. McKinsey delivered the final blow: only 6% of enterprises can say AI contributes more than 5% to profit.

During the days *Fortune* magazine covered this report, a manufacturing COO's complaint circulated in the industry: "Online, everyone says everything has changed. Back in our workshop, nothing has moved." This cuts deeper than any data — his company doesn't lack budget or tools; it lacks someone to embed those tools into the workshop's real processes.

The report also contains a quieter comparison that directly votes for this book's theme: systems built internally by enterprises have only about one-third the success rate of externally purchased mature solutions. The lead author said almost every company they visited was trying to build tools themselves — and self-building is precisely the path that dies the most.

He also told a control-group story. Some nineteen- and twenty-year-old entrepreneurs built companies reaching $20 million in annual revenue using generative AI. Their approach is the opposite of established enterprises: pick one pain point, drill through it, and bind tightly to customers who actually use their product. Older companies try to eat the world in one bite; young people take one small bite, drill through, then take the next.

This divide wasn't dug in the AI era. China's enterprise software industry has been lying in this ditch for over a decade: big companies want customization, vendors lose money on every deal, code is delivered then abandoned, and the industry collectively becomes "the client's outsourcing company." A veteran of the podcast *Hard Land Hacker* put it bluntly: "Customization is the natural enemy of SaaS; this curse can only dissolve naturally when the market matures." America is more polite but the script is similar: sales signs the deal, implementation moves in, half a year later delivers a "fully featured but nobody loves it" system, followed by protracted disputes.

It comes down to the same wall: where software is built and where value is created are not in the same place. On this side of the wall, requirements are relayed through tickets, meeting minutes, and weekly reports — each relay distorts a layer; on the other side, the customer's real workflows hide in spreadsheets no one wrote down, in word-of-mouth conventions, in the tacit knowledge of "you need to ask Lao Wang for this." The software industry has invented countless ladders to climb this wall — requirements documents, user research, implementation methodologies, customer success systems — but the wall remains.

Until one company decided: we're not climbing the wall anymore; we're sending people over.

### 1.2 Palantir's Victory

In 2003, Silicon Valley was still climbing out of the internet bubble's ruins. Peter Thiel and a group of Stanford-educated young people founded a company named after a Lord of the Rings artifact — Palantir, the seeing stone that can glimpse distant places. Their ambition sounded like science fiction: build data analysis software for US intelligence agencies, connecting fragments scattered across countless classified databases into a picture that helps analysts catch terrorists.

This business had a premise that would make any product manager collapse on the spot. Years later, early executive Bob McGrew recounted the story vividly on YC's Lightcone podcast:

> "Our founding goal was to build software for the intelligence community — basically, to build software for spies. And one challenge of building software for spies is: I don't know any spies, and you probably don't either. Even if you happen to find a spy and ask them 'how do you actually work day to day,' they usually won't tell you."

No user interviews, no requirements documents, no usability testing. The first lesson of internet startup methodology is entirely void here. Co-founder Stephen Cohen's solution was adorably crude: build a demo, show it to intelligence people, ask what they think. They were merciless: "This is terrible, it has nothing to do with what we do." Cohen didn't retreat — he asked one more question: "So what would you want it to be different?" Then he took out a notebook, wrote down every item, went back, revised, and brought it back.

This clumsy cycle is the embryo of FDE. It contains two intuitions later proven worth a thousand gold: first, customers in complex domains don't know what they want until they see something usable; second, the fastest path to understanding what customers want is to put the people building things next to the people using them.

The one who elevated this intuition into company strategy was the 13th employee, Shyam Sankar. As Palantir moved from its first customer to the second and third, the team discovered a counterintuitive fact: each customer's needs were subtly but critically different. The standard approach is to extract commonalities, build a universal product, and say no to differences. But Palantir's customers were the CIA, the FBI, the US military on the battlefield — saying no meant being out.

Sankar went the other way: build a highly customizable platform, then station engineers at customer sites to complete the last mile.

His most critical move was changing the accounting. In the software industry's ledger, "customizing for a single customer" is called services — the enemy of profit margins. Sankar flipped it: on-site customization should be booked as product discovery. Every pitfall engineers step in at customer sites is a signpost for the platform's next evolution.

Sankar himself was the first Forward Deployed Engineer. His earliest field experience is the prototype scene for this role. Around 2007, the US military's Joint IED Defeat Organization (JIEDDO) — IEDs being the biggest source of casualties in Iraq — allowed Sankar to bring a small team and a "still rough" product into a classified information room for two weeks of co-located work. A classified information room is a physically isolated secure space where even speakerphones are forbidden. Sankar came up with a barbaric solution: strap a phone to his head with a rubber band, freeing both hands to code — one ear listening to analysts' feedback, the other ear listening to colleagues at Silicon Valley headquarters. Nineteen-hour days for two weeks: demo, connect data, collect feedback, revise on the spot. When it ended, the analysts said: this thing is useful. Sankar himself collapsed from exhaustion and called CEO Karp: "This is not sustainable, we're done." Karp's answer later became company culture: make this "unsustainable" thing into a system.

Years later, colleagues recalled that Sankar could criticize without emotion. Once, he was having a great conversation with colleague Ted Mabrey at an airport café, and Mabrey's inbox suddenly received a sharply worded criticism email — written on the spot, sitting right across from him. "No personal attacks, just one subtext: to win, I owe you these honest words."

This approach quickly proved itself on the battlefield. Stationed Palantir engineers discovered that soldiers didn't need fancy intelligence charts — they just needed a small tool to mark "this road is suspicious" on a map. IEDs were the patrol's biggest killer. The engineer cobbled together a crude map tool on the spot: soldiers tap once to mark a danger zone, visible to the entire team in real time. This tool saved lives and later became a standard platform feature. It could never have been born in any headquarters conference room — only in the moment when engineer and soldier looked at the same stretch of road together.

On the commercialization side, they died once first. Palantir's first enterprise-facing product, Metropolis, was a market flop — only a few financial companies barely used it. The second attempt, Foundry, finally took off. The turning point was Airbus: in the Toulouse factory, an A380 fuel pump failure kept recurring; Airbus's own engineers had investigated for two years with no clue. Palantir's people came in, connected sensor data to the platform, and cracked the case in two weeks — during climb, fuel sloshed away from the pump body. A trivial fix preserved an order reportedly worth tens of billions of dollars. Airbus's digital transformation head later publicly remarked: "The same problem, we used to need twenty-four months." Airbus became Palantir's most devoted European advocate, building its entire data platform Skywise on top, connecting tens of thousands of aircraft and over 50,000 users. The later trajectory is even more interesting: this platform went from customer to channel — today over 150 airlines run on Skywise.

There's also a piece of lore worth recording. It's widely rumored that Palantir's software participated in the 2011 operation that killed Osama bin Laden. This claim has never been confirmed nor denied — a journalist writing a Palantir biography deliberately left this ambiguous footnote. But true or false, the rumor itself is Palantir's best sales weapon.

By 2016, Palantir's Forward Deployed Engineers once outnumbered platform engineers. A software company with more than half its engineers not writing product at headquarters but scattered across customer sites worldwide. Wall Street didn't understand for years, dismissing it as "people sea tactics" and "more like a consulting company."

Then time gave the answer. In 2023 it launched its AI platform AIP, paired with a methodology called "Bootcamps" (detailed in Chapter 8), compressing enterprise software's 9-12 month sales cycle to weeks. In Q4 2025, its Rule of 40 — revenue growth plus adjusted operating margin, a software industry health indicator where 40 is passing — hit 127%; in Q1 2026, 145%. Single-quarter bookings of $4.26 billion (total contract value), Net Revenue Retention (NRR) of 139%, $7.2 billion in cash on hand.

Karp said just one sentence on the earnings call: "We are a species unto ourselves." Market cap once broke through $400 billion.

Those who mocked its people sea tactics were speechless. Palantir spent twenty years proving one thing: that wall can't be climbed by ladders, but people can climb over it. These wall-climbers got an official name — Forward Deployed Engineer.

The invention of this name was later publicly claimed by Sankar on the *American Optimist* podcast. His definition is anything but official: a Forward Deployed Engineer is someone who "takes the pain in, puts the product out."

Of course, there's another account of the origin. Some VCs have documented that embedding engineers at customer sites was done earlier by IT services companies than by Palantir — this controversy is tabled for now; Chapter 7 will return with data.

### 1.3 What Is FDE

#### One-Sentence Definition

The definition used in this book comes from the mode's best interpreter, Bob McGrew — early PayPal engineer, later Palantir executive, then OpenAI Chief Research Officer whose team produced ChatGPT and GPT-4:

> **A Forward Deployed Engineer is an engineer stationed at the customer site who bridges the gap between "what the product can do" and "what the customer needs."**

"Stationed at the site" means your work context is embedded with the customer: joining their groups, reading their data, attending their meetings, knowing the person who "understands why the process works this way" — not necessarily sitting in their office every day. The "gap" is the reason this role exists: where the product works out of the box, you're not needed; where the gap is deepest, you're most needed — intelligence, finance, manufacturing, healthcare, law.

"Engineer" is the most important qualifier: you write production code, not reports. Palantir deliberately kept "Software Engineer" in the title to emphasize to the world: this is not a consulting role. As for "Forward Deployed," it's a military term for forces deployed to the front line — putting the most combat-capable people closest to the problem.

#### What It Is Not

First, what it is not.

It's not pre-sales. Pre-sales work ends before signing, aims to win the deal, and its output is slides; FDE work enters deep water after signing, aims to win results, and its output is systems running in production. Pre-sales makes the customer believe "this can work"; FDE makes it actually work.

It's not on-site outsourcing — this distinction is especially important for Chinese readers, as "engineers stationed on-site" has too long and too painful a history in China. Qimeng Technology, one of China's first service providers to fly the FDE flag, drew the line in three sentences on its website:

1. On-site outsourcing bills by the hour; FDE delivers by phase and accepts by results;
2. On-site outsourcing writes from scratch; FDE brings a product foundation to do engineering;
3. On-site outsourcing stays longer and longer — when people leave, the system stops; FDE leaves when done, with capability remaining in the system and the customer's team.

Jove, head of FDE at Silicon Valley AI customer service company Cresta, drew the boundary in more detail in a video dialogue. His team is expanding from 30 to 100 people this year, and his judgment is: FDE must be bound to an AI platform to be meaningful — if you're just doing traditional data integration and system building, it's hard to distinguish from traditional implementation engineers or outsourcing. He also has a hard requirement for hiring: in the agent era, not being able to code is like being illiterate.

Another noteworthy mechanism is dual responsibility: FDE must not only make the deployment succeed but also carries the metric of "making the product more mature" — what's learned in the field must feed back into the platform.

It's not a consultant. Consultants deliver advice by project and aren't responsible for execution; FDE is responsible for the system's final operation, with the endpoint being "the customer's team can use it independently." Anthropic's collaboration with fintech company FIS is a specimen: engineers embedded at FIS to co-build anti-money laundering agents, compressing investigations from hours to minutes, but the explicitly stated goal of the cooperation was not delivering a system but "transferring knowledge so FIS can build agents on its own in the future." A consultant's business is built on customers' continued need; whether FDE succeeds is measured by the opposite standard — the day the customer no longer needs you is the day you've succeeded.

Buyers think the same way. A JPMorgan Chase technology lead said bluntly when discussing co-building with platform vendors: "What we want is not more consultants, but engineers who can build things that don't exist yet."

It's not a traditional product engineer. Product engineers face abstract users — personas, funnels, DAU; FDE faces specific customers — a bank's risk control department, an Iowa farm, a patrol team outside Baghdad. Palantir's official blog post "Dev versus Delta" gives the official division of these roles: platform engineers own "one capability, serving multiple customers"; Forward Deployed Engineers (internal codename "Delta") own "one customer, mobilizing multiple capabilities." Platform engineers pursue features that work everywhere; FDE pursues thoroughly solving the problem of the one customer in front of them.

Nabeel Qureshi, who spent nearly eight years as a Forward Deployed Engineer at Palantir, put this discipline in a crude phrase: "Fuck generalizability" — save this customer first; whether it can be reused for the next one is the platform team's business.

#### How the Wind Blew

A role invented in 2003 — why did it become a top trend only in 2025?

The most direct trigger is generative AI. LLMs created an unprecedented gap: anyone can make a stunning demo in five minutes, but connecting that demo into an enterprise's real data, permissions, compliance, and workflows is an order of magnitude harder. Model companies have gradually figured out: the next battleground is deployment capability. A logistics AI company's deployment lead put it more bluntly: AI landing rarely fails on the model — it almost always fails on context.

The demand-side vote is equally blunt. Goldman Sachs rolled out its self-built AI assistant bank-wide, covering tens of thousands of employees in internal testing; Klarna's AI customer service took on two-thirds of service conversations in its first month; even universities are acting — Syracuse University opened Claude to all faculty and students, requiring training completion before account activation.

This wind didn't blow overnight. As early as July 2025, Semafor published an article asserting that this "unremarkably named position" would change the AI industry.

The numbers trace the curve's steepness: according to Indeed's official statistics, in April 2025, only 643 positions with the FDE title existed nationwide in the US; one year later, 5,330 (Indeed's job matching methodology) — a 729% increase. Other organizations' methodologies are more dramatic — 800%, 1,165% — different statistical methods, completely consistent direction. On YC's job board, over a hundred startups posted this position that barely existed three years ago.

VC firm a16z directly called it "the hottest position in tech," with a vivid metaphor: enterprises buying AI is like your grandmother getting an iPhone — she wants to use it, but needs you to set it up for her.

The Financial Times's November 2025 reporting is the best slice for observing this trend. OpenAI's European FDE lead Fournier said the team was founded a year ago and is about to expand to 50 people — "demand has exceeded our expectations"; Anthropic's Applied AI lead De Jong said something more interesting: "A Fortune 500 bank's needs and an AI-native startup are two completely different species" — so her team expanded fivefold in a year. Palantir UK's head Prettjohn condensed the company's creed: "Software only has value when it truly matters to the end customer." Even model company Cohere's CEO Gomez came out to endorse: "We embed engineers from the very start of the contract, then step back once the customer is running smoothly."

The intensity of talent competition has a string of hard metrics. OpenAI's Forward Deployed function was publicly announced by Colin Jarvis on social media in January 2025, with a single-sentence mission: "help customers push systems into production"; the team started with 2 people and grew to 52 in a year. Salesforce, which wrote "we don't do implementation ourselves" into its textbook, publicly committed to hiring 1,000 FDEs; Google Cloud released 59 positions at once, with CEO Kurian personally recruiting online for "builders who want to stand at the center of the agent era"; Box's CEO Levy publicly asserted this would become one of the most sought-after positions in tech.

Databricks went further, reorganizing its entire professional services division into an FDE organization, serving over 1,900 customers in twelve months. Even Deloitte, which lives by selling consulting, established a dedicated FDE business line in December 2025. Europe hasn't been idle either — from Mistral to Lovable, star startups' hiring focus is shifting from research talent to deployment talent.

This wind even blew into government view. At the end of 2025, Shanghai held the nation's first FDE-specific training class, jointly organized by six entities including the Municipal Organization Department and the Municipal Economic and Information Commission. Interestingly, the first cohort's composition: not engineers, but leaders of municipal state-owned enterprises and key industry regulatory departments — training the demand side first, then the supply side. The supporting project's goals are equally blunt: connect a hundred enterprises, build a thousand agents, and drive ten thousand developers to transform.

The official positioning for this position is "special forces in the AI field." A position so hot that the government organizes training classes — this is rare in software industry history.

Then came the giants voting with their feet. On May 11, 2026, OpenAI announced the formation of a "Deployment Company": self-controlled, jointly with 19 top-tier capital firms including TPG, Bain Capital, and Brookfield, with initial investment exceeding $4 billion, media-disclosed pre-money valuation of approximately $10 billion, and the acquisition of a consulting firm with 150 deployment engineers. Hours later, Anthropic was reported to be forming a comparable joint venture with Blackstone. The two largest model companies, on the same day, elevated "deployment" from cost center to strategic asset — the capital market voted for FDE in the most expensive way possible.

Why is the capital market willing to vote this way? Foundation Capital laid out the math openly: they estimate this wave targets a $4.6 trillion market — half is what enterprises pay for sales, marketing, and engineering positions' compensation; half is IT services and outsourcing spending. In other words, software's billing target is shifting from "tool budget" to "labor budget." In a16z's words: software no longer just helps workers work — software itself is the worker.

Of course, there are cool-headed doubts. The Wall Street Journal put the question on the table in its reporting: this approach is more like consulting than software; embedded talent is too expensive — whether it can scale remains an open question. This is a serious challenge — Chapter 7 of this book will address it head-on.

The deepest reason is what McGrew saw through: "AI agents are a category that doesn't have a dominant player yet, so there's massive product discovery to be done." What CRM software should look like had a standard answer twenty years ago; what agents should look like, no one knows — including the customers themselves. The answer can only be found at customer sites. McGrew put it more bluntly on Sequoia Capital's Training Data podcast: Palantir's AI platform is valuable precisely because it's not a model, but the layer that "lives outside the model and deals with the rest of the enterprise" — the stronger the model, the more valuable this layer becomes.

Tech analyst Ben Thompson provided a longer historical coordinate: multi-year, deeply embedded delivery is not Palantir's quirk but the software industry's return to the norm of forty decades ago — his judgment is that services and integration teams will comprehensively return, and this generation of AI companies must learn to sell from the customer's top down.

In 2003, Palantir invented FDE because it "didn't know how spies work"; in 2025, the entire industry collectively embraced FDE because it "doesn't know how agents should work in enterprises."

### 1.4 FDE's Responsibilities and Traits

#### A Resume Born for This Role

If you want to answer "what kind of career is FDE," McGrew's resume is almost the standard answer.

His first job was at PayPal as an early engineer. That group later became known as the "PayPal Mafia," profoundly shaping all of Silicon Valley. After leaving, he joined early-stage Palantir, rising to executive, witnessing FDE's entire journey from emergency measure to company strategy. When he managed product and engineering teams, he proposed a famous metaphor: Forward Deployed Engineers repair "gravel roads" leading to value at customer sites; the product team is responsible for judging which gravel roads are worth widening and paving into "highways" serving the next ten customers. He later summarized the entire model in one sentence: do things that don't scale, at scale.

Later, he became OpenAI's Chief Research Officer, leading the development of ChatGPT, GPT-4, and the o1 reasoning model. In other words, this person has built platforms on this side of the wall, climbed over to the other side, and finally personally built the technology that made the wall higher.

An interesting scene occurred at a 2025 YC AI conference. McGrew originally expected entrepreneurs to surround him asking "how was ChatGPT invented," but everyone chased him with the same question: how exactly does Palantir's FDE model work? A person who invented ChatGPT was most questioned about delivery methodology.

#### Three Layers of Traits

Synthesizing twenty-plus job postings from various companies and practitioners' firsthand accounts, FDE's traits can be summarized in three layers.

**First layer: sufficiently broad technical generalist.** FDE doesn't need to be the deepest expert in any field, but must be able to independently solve full-stack problems at customer sites (from UI to database, one person handles it all): can write code, tune interfaces, understand data pipes, deploy to cloud, grasp LLM quirks, and understand enterprise environment "utilities" — SSO, permissions, compliance certifications. The job market has a clear price tag for this combination: GetPerspective's early 2026 *Forward Deployed Engineer Compensation Report* shows that mid-level FDE at top AI labs have median annual total compensation of about $385K, senior about $610K, principal over $1M — higher than most pure R&D positions at the same level, because the market knows how scarce such people are.

**Second layer: the ability to translate technology into business results.** This is the watershed between FDE and ordinary engineers. A frontline practitioner's widely quoted words: "The model is usually the cleanest part. The hard part is finding the workflow nobody wrote down, the data source people actually trust, and the person who knows why the process works this way." Palantir's hiring standard is more blunt: "The candidate's expressiveness, clarity, and communication ease should make me happy to have them lead a customer meeting."

Interviews also screen this translation ability. OpenAI and Palantir's FDE interviews have a signature segment called "problem decomposition": throw a huge, vague real enterprise problem at you, sixty minutes without writing a single line of code, watching only how you ask follow-up questions, how you define scope, how you build order out of chaos. The interviewer's advice: understand the problem before jumping in — slow is smooth, smooth is fast. In a normal interview, "I optimized the query by 40%" is a perfect answer; the perfect answer in an FDE interview is: "I optimized the query by 40%, which meant the customer's analysts got reports two hours earlier each day, and the team's processing volume tripled." Technical achievements must be converted into customer language.

**Third layer: ownership, plus a touch of "rebellion."** A saying circulates in the practitioner community, specifically describing the accountability this role requires: "The deployment goes down at 2 AM. You don't file a ticket, you don't blame other teams, you don't go back to sleep. You fix it. Period." Palantir has a more subtle expectation for business-side roles: both deep industry knowledge and the courage to be a "rebel" — able to see the absurdity in the customer's current state and push for tenfold, not ten-percent, improvements. CEO Karp's behavioral benchmark was the "French waiter": embedded in the service process, sensitive to real needs, yet with enough confidence and taste to guide customers from "what they think they want" to "what's actually good for them."

#### How a Day Goes

In daily practice, FDE's time breaks down roughly: 40-50% immersed at the customer side writing code and tuning systems; 20-30% aligning direction with customer management, decomposing problems, making architecture decisions; 10-20% distilling field-learned patterns back into the company's product line; the rest is evaluation optimization and knowledge sharing — writing playbooks, internal evangelism, training customer teams.

This schedule hides an important message: FDE is not "an engineer on assignment" but "an engineer with a two-way mission" — delivering results to the customer on one end, feeding intelligence back to the company on the other. This is the theme of the next two sections.

### 1.5 Everything Speaks Through Results

If you had to summarize FDE's work creed in one sentence, it would be: everything speaks through results. Palantir executive Mabrey broke it down into two plain questions: "Does it actually work? Does it actually matter?" — by his account, the FDE model is one of the company's "biggest secrets."

First, separate "data" from "results." Enterprise software history is never short of projects with beautiful data and terrible results: feature checklists 100% complete but only 5% of people using them; system availability of four nines (99.99% uptime) while business departments would rather keep using spreadsheets. The 95% failure projects in the MIT report mostly didn't lack data reports — the numbers were all there, but value didn't arrive, because no one was responsible for "that line on the financial statement."

The FDE model institutionally guarantees that "results" aren't diluted, specifically through three things:

- **Pricing aligned with results:** In Palantir's early government projects, they heavily used "pay only if it works" arrangements. McGrew recalled bluntly: "Early on, it was reasonable for a startup to bear all the risk — you pay us when it works." This logic has evolved more precisely in the AI era: Sierra charges per "resolved conversation" — no resolution, no charge; many FDE service providers deliver by phase and accept by results. Once pricing is bound to results, the delivery team's entire behavior gets re-sorted — you won't spend three weeks polishing a feature nobody uses, because "nobody uses it" comes out of your own pocket. Platform vendors are following: Databricks has written milestone-based, result-aligned pricing options into its official delivery model.

- **Success metrics front-loaded before starting work:** The first step of an FDE project isn't writing code — it's defining "what does success look like" with the customer. Palantir's Bootcamp requires customers to lock onto an extremely focused core battlefield — "reduce scheduling conflicts on a specific production line by 30%" rather than "explore AI empowering manufacturing" — specifically to prevent projects from drifting toward unfalsifiable under the guise of "exploration." OpenAI's collaboration with John Deere is a textbook demonstration: first review hundreds of real field operation cases with agronomy experts, build a custom evaluation system, then start iterating the model. The final "chemical usage reduced by up to 70%" wasn't post-hoc packaging — it was a target set before work began.

- **The final judge is behavioral change in the customer's organization:** The report has a sharp finding: only about 40% of enterprises provide official AI tool subscriptions for employees, while up to 90% of employees use personal consumer-grade products to solve work problems daily. This means many "successfully launched" projects are actually in a state of "official system idling, employees taking detours." In FDE philosophy, the milestone isn't the day the system goes live — it's the day the customer's team changes how they work. Sierra internally deliberately named the position "Agent Engineer"; head Meurer explained the selection criteria: only take two types of problems — genuinely hard ones, and genuinely impactful ones — both must hold simultaneously.

"Everything speaks through results" sounds like common sense, but executing it is an affront to the entire interest structure: 1) sales doesn't dare over-promise, because the delivery team is responsible for results; 2) the customer's IT department can't use "feature checklists" to report completion, because business departments' usage rates become acceptance criteria; 3) FDE themselves can't use "I finished per requirements" to avoid responsibility, because whether the requirements themselves were right is also on their ledger. Why this role is expensive, and why it's worth being expensive, are both here.

### 1.6 FDE's Four Faces in the Team

An FDE simultaneously lives in four worlds — they are the connector of these four worlds.

- **To the customer, they are "embedded product manager + full-stack engineer":** Both observing the customer's real work like an anthropologist — the most valuable discoveries often come from "watching," not "asking" — and building things directly at the observation site like an entrepreneur. Palantir institutionalized this two-person combination: Deployment Strategist (internal codename "Echo") reads the customer's mission, stakeholders, and adoption path; Forward Deployed Engineer (internal codename "Delta") handles technical implementation. Two people to a team — one diagnoses, one builds — neither dispensable.

- **To the company's product line, they are "forward scout and intelligence officer":** This is the most essential difference between FDE and traditional delivery teams. Traditional implementation costs are sales costs — every person-day billed must be earned back from the contract; a healthy FDE organization treats field work as R&D — three customers hitting the same integration gap isn't three troubles, it's product intelligence; five deployments all needing the same workflow should be abstracted into the platform's next standard capability. Former Palantir engineer Barry recalled that Foundry platform's key components were born at customer sites in Zurich, Houston, São Paulo, Toulouse, and other far-flung locations, growing bottom-up, eventually feeding back into a product generating billions in annual revenue.

- **To sales:** Enterprise customers have been let down too many times and are immune to all slides. FDE rebuilds trust with two actions: first, doing — building something runnable on the spot, on the customer's own data, in the customer's own environment; second, honesty — daring to say no to the customer's wrong premises. Palantir's Bootcamp production-ized this trust-building process: customers bring real data, a deployable prototype is built in one to five days, executives click and use it themselves. Early Bootcamp paid conversion rates were only 5-10%, while the company's disclosed later conversion rate approached 75%.

- **To the organization itself:** Palantir has produced a startling density of entrepreneurs — Lenny's Podcast interviews gave a figure: nearly one-third of product managers left to start their own companies. This is no surprise — FDE's daily training is end-to-end delivery of something valuable in resource-constrained, requirement-ambiguous, relationship-complex environments, almost a complete preview of founder training. Srinivas who later founded Decagon, Meurer who built Sierra's agent engineering team, and several authors of the industry's most widely circulated methodology articles all came from Palantir's Forward Deployed positions. One company's talent spillover became an entire industry's talent infrastructure.

These four identities combine into one thing: the way organizations understand customers has changed — from second-hand information relayed through layers to first-hand experience engineers personally touch in the field.

### 1.7 How to Hire FDE

First, a cold splash of water: FDE is one of the hardest positions in software to hire, because it requires a person to be simultaneously excellent in two dimensions that usually trade off against each other.

Former Palantir engineer Barry put it thoroughly in his memoir: Palantir's FDE hiring standard was "engineers who could get into Google or Facebook" — because they build systems at customer sites, not tune parameters; but technical skill alone is far from enough — Forward Deployed people also need creativity, judgment, and customer-facing charisma. He added a sharp note: this is far more expensive and difficult than hiring a traditional pre-sales team.

Breaking down hiring market practice, FDE hiring has three key links.

- **Candidate profile:** Hire "curious bulldozers," not "exquisite craftsmen." a16z's advice to startups used the term "curious doers": strong initiative, lack of reverence for the status quo, hunger for customer problems. McGrew was more specific: FDE teams need two types — "domain rebels": understand the industry but don't worship industry conventions; "prototype speedsters": speed over perfection, accept that version one will be thrown away and rewritten. Conversely, two types favored in traditional engineering culture are actually danger signals for FDE: "craftsmen" who put code elegance above customer results, and "loyal executors" who treat every customer word as scripture. Palantir early on put the filter at the very outside of the funnel: high-profile embrace of defense business, below-market salary, scary working hours — Qureshi called this the "bat signal," only effective on its own kind.

- **Interview:** Use "problem decomposition" instead of eight-legged essays. As mentioned earlier, this segment is the soul of FDE interviews: give the candidate a vague, huge problem with real business rough edges — "A bank's compliance team manually checks 30,000 transaction alerts daily, 90% are false alarms, what do you do" — then observe for sixty minutes. What's tested isn't the answer, it's the process: did they clarify constraints before acting, distinguish root causes from symptoms, remember that a real user sits at the other end of the system, can they clearly articulate trade-offs. Palantir also embeds about twenty minutes of behavioral questions in each technical round, and explicitly rejects technically strong but culturally unfit candidates — the most important cultural item is sense of order in the face of ambiguity.

- **Compensation structure:** Accept a hybrid of "engineer compensation + floating bonus tied to company operating metrics." Early 2026 market data can serve as anchor: Palantir Forward Deployed Engineer median annual total compensation about $215K; top AI lab mid-level FDE about $385K, senior about $610K; Anthropic's position base salary ranges $200-300K. Another noteworthy detail is bonus design: Palantir's bonuses are often tied to operating metrics like customer expansion, between engineering bonus and sales commission; a16z's advice is to align incentives with customer managers, but don't put hard sales metrics on FDE — that would steer behavior toward signing deals, not results. One author who scraped fifty job postings gave a simpler touchstone: look at whether the position's compensation package includes sales commission — high commission ratio mostly means pre-sales with a trendy title. Compensation structure is also part of role definition: how you pay affects how people behave.

### 1.8 How to Become an FDE

Switching perspective: if you're an engineer, product manager, or consultant wanting to enter this high-growth market, how do you get there?

First, self-test: the glamour and cost of this position are two sides of the same coin. In forum practitioner communities, discussion of FDE has a rare honesty. The positive part: the best combination of technical content and brand endorsement, one of the few positions that simultaneously accumulate technical, business, and customer resources. The cost part: 25-50% travel is normal, OpenAI's job posting explicitly states travel up to 50%; work rhythm defined by customer urgency, not your own schedule; and a repeatedly appearing reminder — the risk of professional burnout is real.

One comment: "Some treat it as a brand springboard, some say it's consulting with a cool title — both are right; the difference is whether your company feeds field learning back to product, or sells you as person-days." This is both a career selection criterion and the theme of Chapter 7.

Now the money in China. Those dollar salaries are just background noise for most Chinese readers; the first half of 2026's domestic job market has already put RMB prices on this position: ByteDance offers Doubao FDE 35-70K RMB monthly, 15 months; Ant Group's Ant Digital 40-60K, 15 months; Zhipu's FDE lead 60-80K; Tencent Cloud 35-65K (these two didn't disclose months); Alibaba Cloud 20-50K, 16 months. Converted to annual packages, these positions roughly fall in 300K to 1M+ RMB — "annual million" is reachable at the high end of top positions, but isn't the industry average.

The price difference under the same title is more worth looking at than level differences. An industrial software company in Tangshan hiring an "AI Delivery Engineer (FDE)" requires a master's degree, stationed in manufacturing, 8-16K RMB monthly — the price gap with Zhipu is nearly tenfold at maximum. Behind the price gap are differences in platform foundation, customer quality, and pricing model. So when looking at domestic opportunities, don't first look at whether the business card has the three letters FDE — use the ruler from Chapter 8 to measure: does this company charge by results or by headcount.

Next, practice translation: most engineers' technical foundation is sufficient, but scarce is the craft of "translation" — specifically three types: translating business problems into technical problems (Chapter 2), translating technical solutions into language executives understand (Chapter 3), translating field experience into knowledge the team can reuse (Chapter 7). To practice these three, attending classes is worse than getting on stage: join a pre-sales once, do a on-site shift once, train a real user once, then see in which discomfort you grow fastest.

For interview preparation, rewrite your resume to be "customer-result-oriented." The principle was stated before, emphasize again: every technical achievement on your resume must walk the last mile to customer language. "Built a RAG system" is engineer language; "The RAG system I built cut customer service first response from 4 hours to 8 minutes, and at renewal the customer proactively proposed expansion" is FDE language. Also prepare two types of stories: one experience where you built order amid unclear requirements, and one honest failure — Palantir-line interviewers have an obsession with "tell me a real failure," because the essence of this work is advancing amid uncertainty; people who don't admit failure have no evolution ability.

When choosing a company, ask three counter-questions. First, "what is your product platform" — FDE without a platform foundation is pure labor outsourcing. Second, "how does field learning flow back to product" — ask them to give a recent example of something from the field becoming a product feature; if they can't, there's a problem. Third, "who does FDE report to" — reporting to product or engineering lines usually means the mode is taken seriously; reporting to sales lines, be careful of becoming a pre-sales labor pool.

All the above is written for engineers. What about people who don't code? Positions exist, and Palantir left them long ago: in the two-person combination from section 1.6, the Deployment Strategist codenamed "Echo" doesn't write code — reading the customer's mission, stakeholders, and adoption path. Looking outward along this line, Chapter 4's change management, Chapter 5's "train the trainer" mechanism, Dewu's knowledge operations group that drills into business teams to transfer tacit experience, Chapter 3's technical content marketing — all are entry points for non-engineering backgrounds. The common requirement of these roles is exactly the specialty of operations, consulting, and content backgrounds: straightening out people's affairs.

The last question can only be answered honestly: how far can this path go? No one has walked it to completion. This position is too new; there's no sample of a complete cycle, only structure can be seen. The consumption side is real — the travel intensity and customer-urgency-defined rhythm mentioned above will grow heavier with age and family stage. The appreciation side is also real — customer trust, industry judgment, and cross-organizational prestige all compound with seniority.

There are roughly three exits: 1) return to the product line — people who've tempered the field into platform are natural candidates for product leads; 2) start your own company — nearly one-third of Palantir product managers left to found companies; 3) go to the buyer side — after reading Chapter 8's state-owned enterprise stories, you'll know the buyer side most lacks people who understand the seller's playbook. Which path holds will have an answer five years from now. What can be certain now is only one sentence: this profession prices "endurance," but the premise is you're at a company that treats field learning as an asset — otherwise what's endured is just years of service.

### 1.9 FDE's Common Toolbox

Finally, the current tool panorama for this position. Tools become obsolete, but the capability layering behind tools doesn't. Five layers, from ground to rear.

- **Platform foundation layer.** The premise of the FDE model is "bringing a platform to the field" — otherwise it degrades into custom development. Palantir's Foundry and AIP, the core is the thing called "ontology" — modeling enterprise data, logic, and actions into a semantic layer, letting AI run on a "business-aware" foundation; OpenAI's model interfaces and agent toolchain; Sierra's agent platform. When evaluating any FDE opportunity, this layer's thickness is the first priority.

- **AI engineering layer.** Post-2025 daily craft includes: prompt engineering and context management; RAG; evaluation systems — building quantifiable rulers for fuzzy business quality — this is the signature skill distinguishing FDE from traditional implementation engineers in the AI era; agent architecture: tool calling, multi-agent collaboration, human oversight at key links; and cost/speed engineering optimization.

- **Data and integration layer.** Almost every FDE project's first week is spent fighting this layer: data pipes, enterprise system connectors, permissions and authentication, vector databases for AI knowledge retrieval, data governance and desensitization. Qureshi also has a rule of thumb: in enterprise data problems, 95% is integration, cleaning, and association — not analysis — 70% of project progress is stuck in this layer, but demos can't see it.

- **Delivery and collaboration layer.** Working within the customer's security boundary means "dual adaptation": you must both use your own modern toolchain and be able to stoop to the customer's environment — possibly a physically isolated intranet, possibly only deployable in the customer's cloud environment, possibly unable to even access code hosting sites. Containerization, infrastructure as code, and contingency plans for "running the environment even in a disconnected meeting room" all belong to this layer.

- **Knowledge precipitation layer.** This is the most easily overlooked layer, but the one that determines whether the team can escape "revenue growing linearly with headcount": playbooks, component libraries, deployment checklists, and the writing habit of rewriting "one customer's solution" into "a pattern for a class of customers." Chapter 7 will expand on it specifically.

The five-layer toolbox combined is the complete outline of this position: platform as foundation, engineering as craft, responsible for customer results, while connected to the company's product line.

The next seven chapters enter the heart of methodology, starting from the most primitive choice of a project — how to ensure you're solving the right problem.

---

## Chapter 2: Solving the Right Problem

> "On the wrong problem, all execution is waste."

### 2.1 An Autopsy Report on the Proof-of-Concept Graveyard

Silicon Valley has a term: "PoC purgatory" (PoC = Proof of Concept; purgatory literally means "purgatory"). Projects that enter never come out: not dead enough to declare failure; not alive enough to increase investment. So they "continue progressing" in quarterly reports year after year, like a room full of patients on life support.

MIT NANDA Lab's researchers performed a systematic autopsy on this graveyard in *The GenAI Divide* report. They identified five major roadblocks on the path to scaling enterprise AI projects, ranked by frequency:

1. Employees unwilling to use new tools — while these same people use ChatGPT privately every day
2. Concerns about model output quality
3. Poor user experience
4. Lack of executive support
5. Change management difficulties

What's absent from this list is more worth noting: models not smart enough, compute not cheap enough, technology not advanced enough — none are listed. What kills these projects almost entirely happens at the "problem definition" and "organizational reality" level, not the technical level.

A company spent $50,000 on a professional contract analysis tool with an impressive feature list. But a senior lawyer at the company simply wouldn't use it — she continued using free ChatGPT to draft contracts. Her reasoning was simple: the purchased tool's summaries were too rigid, couldn't be customized to her habits. The procurement department's report says "deployed"; the daily reality is the official system idling while employees take detours.

This detail reveals the true cause of the first roadblock: it's not that employees are conservative — it's that consumer-grade products have spoiled them — people who use AI effortlessly at home can't tolerate "AI for the disabled" at the office.

There's also a more painful comparison: **projects done with external professional suppliers have about three times the success rate of internal self-built ones.** Why do external teams win instead? They can't afford to lose — people paid by results bear the cost of defining the wrong problem themselves.

A Japanese company's internal project is a typical cautionary tale: they pulled together three or four of their strongest engineers to form a task force, the demo was stunning, leadership nodded, but from day one no one could answer "by what standard do we measure this system's goodness." Half a year later the project quietly disappeared from reports — no one announced its failure; it just died naturally.

This is first principles: wrong problems in enterprises are far more numerous than imagined. So before writing the first line of code, you must first ensure you're solving the right problem.

### 2.2 PSF: Finding Problem-Solution Fit

Internet startup methodology has a core concept called PMF (Product-Market Fit): if the product is right, the market itself pulls growth. In the FDE world, the corresponding unit isn't "product and market" but "problem and solution" — I call it PSF (Problem-Solution Fit).

The difference is subtle and critical. PMF asks "does my product have market demand" — the perspective is on the supply side; PSF asks "is this specific customer's specific problem worth solving and can it be solved by our capabilities" — the perspective is on the demand side. Within one enterprise customer, there may be hundreds of "AI could do something" opportunities, but the ones truly worth doing must pass three gates simultaneously.

**Gate 1: Pain point verification** — Is this problem a specific person's specific pain? Note the two "specifics." "Improve customer service efficiency" isn't a pain point, it's a direction; "The customer service supervisor spends three hours every Monday morning manually aggregating last week's escalated tickets from four systems, when her real job should be analyzing escalation causes" — that's a pain point.

McGrew gave a sharper standard: go solve one of the CEO's top five concerns. The reasoning is realistic — only problems of this magnitude can crush through enterprise bureaucracy. Sierra's Agent Engineering head Meurer's standard is another phrasing of the same principle: only take two types of problems — genuinely hard ones, and genuinely impactful ones. Hard without impact is showing off; impact without hard isn't your job.

**Gate 2: Economic verification** — How much is solving this problem worth? Many pain points are real but not valuable; projects that can't calculate this math won't survive the next budget season.

You can roughly calculate: how many person-hours does this problem eat per week? What's the equivalent labor cost? What does one error cost? What can the saved staff do instead?

Palantir's Bootcamp front-loads this gate — customers must lock onto a "core battlefield" and give quantitative targets before starting: "reduce scheduling conflicts by 30%," "reduce inventory turnover days by 15%." The NANDA report has a widely cited finding that shows how easily this gate gets skipped: over half of enterprise AI budgets go to front-office sales and marketing, yet returns concentrate in back-office contract review, procurement, and risk control — the "unsexy" places. Everyone is solving "problems that demo well" rather than "problems that are worth money."

**Gate 3: Feasibility verification** — With our current capabilities and this customer's data reality, how far can we get? This gate is most easily drowned by enthusiasm. Two questions must be answered on-site: where is the data and what condition is it in? The answer is often worse than imagined — scattered across seven systems, three versions disagreeing, the most authoritative copy in some veteran employee's private spreadsheet.

OpenAI's FDE lead Colin Jarvis summarized field experience in one sentence: the problem customers describe during topic selection often doesn't match the real data and system situation on the ground.

The second question that must be answered on-site: what's the accuracy threshold? Between "99% usable" and "90% usable" lies an order-of-magnitude engineering investment, yet many business scenarios actually find 90% plus human review is the optimal solution — judging this requires not technology but understanding of business consequences.

"How far can we get" isn't guessed, it's measured — which is why experienced teams put "building the exam" before "going live." Morgan Stanley did exactly this: starting from three specific scenarios, having financial advisors and engineers score model outputs item by item, scores flowing directly into iteration, then re-running old exam questions daily — preventing the model from quietly regressing — intercepting quality decline before it reaches frontline advisors.

OpenAI's official enterprise deployment guide lists seven lessons, the first being "start with a test question bank." Why run daily? Because AI systems often don't error when they're wrong — they just quietly become unreliable — and by the time users notice, the trust bill has come due.

Only after passing all three gates do you touch problem-solution fit. And these three gates must be passed at the customer site — the errors described above mostly grow from judgments made in headquarters conference rooms against second-hand information.

Moreover, these three gates aren't a one-time pre-entry check — this verification must become a daily discipline. Enterprise spend management company Ramp's first principle for their FDE is called "always be topic-selecting": don't accept customer requests wholesale; for every requirement, first collect context, verify assumptions, evaluate impact on overall scheduling. This discipline was bought with tuition — they once spent weeks building an Android feature for a customer, only to discover before delivery that the company internally mandated iPhone-only, rendering weeks of work worthless. The cost of lax topic selection is measured in weeks.

### 2.3 Refusing the Expensive "Proof-of-Concept Graveyard"

In 2025, Qimeng Technology, a Chinese service provider focused on real estate and facilities management, wrote some rather fierce words on its website to turn away potential customers: those whose scenarios haven't been validated should go to demo events first; those whose data can be exported with one spreadsheet need only lightweight services; those who just want to understand AI should use free methods. The last sentence is the fiercest: "FDE is heavy investment. We'd rather you start later than start at the wrong time."

This passage states a counter-sales-intuition fact: refusing wrong projects is itself the FDE model's profitability.

Why are wrong projects dangerous? Because FDE's cost structure is front-loaded — the best engineers, the most expensive travel, the longest on-site investment, all happen before payment. Once stuck in quicksand, it's not a matter of losing one deal — it's an entire elite team being tied up, opportunity cost avalanching.

Former Palantir engineer Barry recalled: "We burned millions on customer pilots, many projects had literally negative infinite margins because we did them for free." The perspective he immediately added is the point: Palantir could afford to burn because it treated pilots as an R&D portfolio — like venture capital, most bets going to zero is fine, but the winners must win back everything. But if you have neither its capital thickness nor the mechanism to convert failed pilots into product assets, then every wrong pilot is pure blood loss.

So FDE teams need a "rejection mechanism," not just the courage to reject. Three operational defense lines.

- **Defense line 1: PoCs must have "graduation criteria."** Every verification project must specify at launch: after how many weeks, using what metrics, reaching what values, the project "graduates" into paid deployment; if not met, both parties part ways cleanly. Palantir's Bootcamp takes this logic to the extreme — it's not a PoC, it's an industrialized substitute for PoCs: one to five days, customers bring real data, a deployable prototype is built on-site, executives decide on the spot. Either see real results in days, or don't start. Traditional PoCs become graveyards precisely because they're "open-ended, metric-less, judge-less."

- **Defense line 2: Beware three types of high-risk signals.** Synthesizing practitioner experience, if two or more of three signals appear, be highly alert. First, "no-man's land" — the project has no clear business-side owner internally, only the IT department is interfacing. IT cares about compliance and stability, and compliance and stability are never reasons to do new projects. Second, "look but don't touch" — the customer demands you prove capability first but refuses to provide real data. Without real data validation, any success is just an illusion. Third, "universal requirements" — customers who want to "cover all scenarios across the entire company" in the first meeting often aren't ready to do any single scenario.

- **Defense line 3: Leave a graceful exit for "rejection."** Rejection doesn't mean severing ties. The best approach is translating "not doing it now" into "when to do it": "This scenario's data foundation still needs three things; we suggest doing another scenario first, which incidentally fills those three gaps, then come back next quarter." Packaging rejection as a roadmap both protects capacity and maintains the relationship — Chapter 3's "lighthouse customer screening" continues along this line.

These three defense lines are written for the vendor's sieve. Flip them over and they're the buyer's self-check table — and there are far more people buying FDE services than selling them.

If your project shows the "no-man's land" signal to vendors — group mandate pushed down, IT department leading, no business department signatory — experienced vendors will be wary, and you should be warier than them: even the supplier can see this project has no real owner.

If your procurement process naturally creates "look but don't touch" — security review demands the vendor prove capability first, yet not a single page of real data is provided — then whatever validation you buy can only be an illusion.

If the requirements you write into the tender are universal — "AI empowering the entire group" — you scare away the most knowledgeable vendors and attract the most boastful.

### 2.4 Pain Points: The Prime Mover of Deployment

Where do the right problems come from? FDE field experience says: from pain. And pain doesn't appear in conference rooms — it only appears at the work site.

Palantir wrote this methodology in blood twenty years ago. Recall the Iraq battlefield story from section 1.2: soldiers needed an IED early-warning tool — a need you could never extract in any interview, because soldiers didn't know they could "ask software for this"; they thought it was just part of patrol life. This kind of pain point users can't articulate themselves — it takes an engineer sitting beside them to see it with their own eyes. Stationed engineers went on patrols with convoys, personally seeing the hesitation and fear before suspicious road sections, and only then was that battlefield-changing crude map tool born.

This method has a name in anthropology — "participant observation"; in the Toyota Production System it's called "genchi genbutsu" — go to the site, see the real thing, get the real situation. FDE has turned it into an operable field method I call "shadow work."

Follow a real user through their real day. Not interviewing them — sitting beside them watching them work — watching which systems they open, which spreadsheets they copy-paste between, which steps make them frown, which "official processes" they route around.

OpenAI's FDE team did exactly this in the John Deere project: flying to Iowa, following agronomists and farmers into the fields, watching how they make spraying decisions, watching what information actually enters decisions, watching how the hard deadline of farming seasons governs everything. The old process they were going to replace originally took the form of agronomists calling farmers house by house, verbally giving equipment usage advice — this workflow appears in no document; you can only see it by going into the fields. That widely quoted practitioner maxim describes exactly what this method's discovery targets: "The hard part is finding the workflow nobody wrote down, the data source people actually trust, and the person who knows why the process works this way." All three can only be found on-site.

Going into the fields also confirmed something that could never be clarified in a conference room: farmers never wanted "AI" — they wanted to spray less chemicals and grow more grain — the product that eventually grew out of this simply charged by acreage with technology actually enabled, every cent the customer pays aligned with value received. Transplanting this pricing logic to China, the corresponding variant is charging by enabled production lines, stores, or outlets — within the procurement habit of project-based acceptance, it's the most easily accepted first step toward "charging by results."

Focus on observing "workarounds," not "processes." Official flowcharts tell you how the organization "should operate"; workarounds tell you how it "actually operates."

Why do employees insist on exporting data to spreadsheets to recalculate? Why does everyone in the department agree "for this table, ask Lao Wang"? Why does someone always manually verify numbers before decision meetings even though there's a data system? Behind every workaround is an unmet pain point, a system failure — and an FDE opportunity.

Beware of "translated pain points." If the requirements you hear have been relayed through the customer's IT department, procurement department, or consulting advisors, each relay distorts — IT translates business pain points into technical requirements ("need a data platform"), procurement translates them into compliance items ("need to meet standard X").

Traditional software disasters often start here: the vendor takes responsibility for the translation, not the pain point itself. So your first duty is to bypass translations and go straight to the nerve endings of pain. This is also the core responsibility of "Echo" in Palantir's two-person model — understanding the customer's "mission" rather than "requirements": what's written in requirements documents is the pain point after being relayed; the customer's mission is where the pain point originates.

Once you've found the real pain point, the next step is to verify at minimum cost: can our solution actually stop this pain?

### 2.5 Validating Value with "Minimum Viable Deployment"

Internet startup methodology has a famous concept called MVP (Minimum Viable Product): validate market demand with the smallest product. The FDE equivalent I call **MVD (Minimum Viable Deployment)** — using the smallest engineering investment, in the customer's real environment, against the real pain point, to verify that value actually occurs once.

One word different, different in the judge. MVP validates "should we build this product" — the judge is the market; MVD validates "can this solution produce value for this customer" — the judge is this specific customer's specific business.

A solution validated successfully at ten customers can still fail at the eleventh — different data foundations, different organizational inertia, different pain point shapes. This is the cruelty of enterprise delivery: value can't be inherited from the previous ten customers; it can only be re-verified on this one customer.

MVD has three iron rules.

- **Rule 1: Real data, no exceptions.** Validating with customer-provided "desensitized sample data" or self-constructed demo data is the first brick in the PoC graveyard. Real data hides every devil: field meanings that don't match documentation, 30% null values, three-year-old coding rules, and the most fatal — the data itself records wrong processes. There's also a more hidden devil: two mutually contradictory, each "correct" answers coexisting in the data. Salesforce used its own customer service agent as its first customer for a year, and the biggest pitfall was exactly this — when the agent encounters two fighting answers it tries to reconcile or even fabricate, and one outdated, unlinked old page is enough to pollute answers. This forced them to go back and integrate 600+ internal data streams into a single authoritative data source, leaving only one authoritative answer per question.

  - **The only hard rule for implementation: customers must bring their own real business data.** Palantir's Bootcamp wrote this into its rules; the John Deere project put "reviewing hundreds of real field operation cases" before modeling. OpenAI internally divides two positions along this line: Solution Architects can use anonymized sample data for demos and validation, while FDE must write production code on the customer's infrastructure with the customer's real data. Solutions that work on fake data will encounter fields that don't exist in documentation on go-live day — and by then, real money has been paid.

- **Rule 2: What you shrink is scope, not value.** A common mistake is understanding MVD as a "castrated version of the big solution" — cutting 70% of features, making it unrecognizable. The right approach is to not cut the solution's depth, only cut its coverage: don't pursue "AI customer service covering the whole company" but "only cover returns and exchanges, but do it end-to-end with no human intervention"; don't pursue "group-wide supply chain optimization" but "only do this production line's scheduling conflicts, but save 20 person-hours per week." Cut the incision small enough that value density is high enough to be visible to the naked eye and actively spread by the business department. Legal AI company Harvey's expansion path is a textbook of this approach: don't roll out firm-wide, first drill through one global business group, make the first batch of partners believers, then expand horizontally after six months of real combat.

- **Rule 3: Set a hard deadline, force trade-offs.** MVD's verification cycle should be measured in "weeks," not "months." Palantir's Bootcamp is one to five days; Sierra's publicly reported fastest go-live case is four weeks; Decagon's typical deployment is four to eight weeks. The point of deadlines isn't speed — it's forcing both parties to make honest trade-offs: anything that can't demonstrate value in these weeks isn't core value yet. A six-month "minimum validation" will almost inevitably regrow into a big project that wants everything — that's the PoC graveyard breaking ground again.

How much is this speed worth to customers? Scott Arnold, Chief Digital and Innovation Officer at Tampa General Hospital in the US, said it bluntly at an industry conference: "We can solve problems in hours and days, not months and years." When blood supplier OneBlood suffered a cyberattack, this hospital used Palantir's platform to build a blood inventory allocation application in hours, then handed it to Florida state for other hospitals to reuse. He also acknowledged Palantir's price premium, "but the premium is worth it" — week-level pace buys never just speed, but the certainty of having tools in hand the night something goes wrong.

### Bootcamp: MVD Industrialized

Palantir's AIP Bootcamp, launched in 2023, is currently the only MVD pipeline validated at massive scale.

First the numbers: starting from fewer than a hundred pilots in 2022, sessions multiplied year over year, media tracking shows cumulative sessions past a thousand, averaging nearly 6 per day at the 2025 peak; enterprise software's traditional 9-12 month sales cycle compressed to weeks; US commercial revenue grew 137% year-over-year in Q4 2025, which the company publicly attributes almost entirely to this.

Next the process: it breaks MVD into five standardized moves. Day 0, preparation: both parties lock onto an extremely focused core battlefield — "optimize a specific production line's scheduling," "reduce inventory turnover days" — rejecting all grand narratives. Day 1, integration: connect the customer's existing systems, extract isolated data, build an initial ontology model.

Days 2-3, construction: FDE and customer technicians write code back-to-back, configure rules, connect LLMs into business flows, produce automated workflows that can execute real actions. Days 4-5, demo and decision: the output isn't a report but a living software interface, business executives click it themselves, watching AI give recommendations based on their own company's data — after the shock, directly enter business negotiation.

Bootcamp's brilliance is that it simultaneously solves MVD's three classic problems: real data (customers bring it), deadline (five days max), judge (executives use it themselves). It also solves a deeper problem — trust. Letting decision-makers personally operate a system based on their own data, feasibility reports can be mostly skipped.

How fast are contracts signed after Bootcamp? Palantir disclosed a real pace on earnings calls that's hard for peers to believe: a large healthcare company attended Bootcamp in December, signed a five-year, $26M ACV deal five weeks later; a global bank signed a $2M initial contract one month after pilot, expanded to a three-year, $19M ACV deal four months later; pharmacy chain Walgreens piloted in 10 stores, improved in-store operational efficiency by 30%, then rolled out to 4,000 stores in eight months, with AI-driven end-to-end workflows automatically processing approximately 384 billion decisions daily that previously required humans. This set of numbers answers "what happens after MVD": validated projects don't grow slowly — they scale by leaps — the customer has already seen value with their own eyes in five days; what remains is just business process.

This "first ten, then four thousand" pace has a Chinese enterprise equivalent: first win one business division, one factory, or one regional company, then use usage data to knock on the group's door.

Of course, this model has a replication threshold: it needs a mature platform foundation behind it, otherwise you can't even set up the environment in five days. For teams without a platform, an executable simplified version is the "two-week sprint validation": week one — enter, connect data, define metrics; week two — build a prototype that solves only a single point problem but can run real business; weekend demo to business stakeholders and decide go/no-go on the spot. Form can be trimmed, iron rules cannot.

The two-week schedule can be broken down very specifically. Week one: Day 1 — entry alignment, write the "single point problem" into one sentence with the customer, write acceptance metrics into one number; Days 2-3 — connect data, only the minimum dataset this problem needs, permissions, desensitization, export method decided on the spot; Days 4-5 — build a skeleton that can query data and answer.

Week two: Days 6-8 — connect the prototype into real business flows, let one or two real users start using; Day 9 — collect usage traces and issue list; Day 10 — demo — not demoing features to IT, but demoing to business stakeholders "your problem, now looks like this," then decide on the spot: scale, adjust, or part ways.

Without a platform foundation, the toolchain uses whatever is at hand: model API calls, or open-source models for private deployment; open-source vector databases for knowledge retrieval; open-source frameworks for flow orchestration; the lightest frontend templates for UI. This "off-the-shelf" combination is enough to support a single-point validation. The only thing to guard against is turning the sprint into a technology selection conference — the only criterion for selection during validation is speed; reusability and extensibility are questions only worth considering after validation passes.

The customer side also has three cooperation requirements: 1) a business-side decision-maker present; 2) an internal data-savvy interface person accompanying throughout; 3) real data access permissions in place on Day 1, not "in process." Missing any one of these three, the two-week sprint will most likely slide back into a traditional PoC.

### 2.6 Should Early Stage Accommodate the Customer's Existing Environment

The MVD stage hits a disagreement almost every project encounters: the customer's existing technical environment — those twenty-year-old legacy systems, department-built tools, and strict security/compliance boundaries — to what extent should our solution accommodate them?

Both sides have reason. The "accommodation" camp says: validating within the customer's real constraints is real validation. The "reconstruction" camp says: deep adaptation for an old environment about to be replaced is wasting precious validation period on engineering destined for the trash.

FDE practice offers a middle path: data-level compatibility with old systems, but architectural non-accommodation with old systems — I call it "read old, write new."

At the data level, deeply accommodate the old environment. Read customer data wherever it is — even if it's on a mainframe, in shared drive spreadsheets, in some ancient system's private interface. Financial industry mainframes, healthcare's hundreds of clinics' heterogeneous systems — these have always been the core battlefield of deployment work. There's no shortcut for data compatibility, because data is the prerequisite for validating value, and data will never move to accommodate your architecture.

The good news is this layer of work is being changed by AI itself: field mapping that previously required manual interpretation, cross-system transport, extracting data from old systems without interfaces — can now be largely handed to agents — for example, using browser agents to simulate human operations to extract data from old systems without interfaces. Integration costs are dropping by orders of magnitude.

At the architecture level, resolutely don't become a parasite of the old environment. Validation-period systems should run within self-controlled boundaries, interacting with old systems through interfaces, not writing code into old systems. Three reasons: 1) validation-period solutions have better than even odds of being overturned and rewritten — the deeper the parasitism, the greater the waste; 2) writing into old systems requires going through the customer's change management process, measured in months, fundamentally conflicting with MVD's week-level pace; 3) maintaining an "evacuable" posture is itself a negotiating chip and an honest stance — FDE leaves when done; parasites can never leave.

At the process level, follow human habits, not system habits. This is the one technical teams most often get backwards. Technical environment can be tough, but human habits must be followed.

If users' core actions happen in spreadsheets and email, MVD's interface should appear in spreadsheet plugins and email, not require users to log into a brand-new portal. OpenAI's deployment at BBVA, entering from the ChatGPT interface already used by 120,000 employees rather than starting from scratch, is a model of following habits. The cause of death in section 2.1 still holds: employees' unwillingness to adopt new tools ranks first among five roadblocks. What new systems are truly up against is users' old habits.

### 2.7 "Actions Speak Louder Than Words" User Research

Finally, pull the camera back to methodology's source and discuss the difference between FDE-style user research and traditional research.

Traditional research's creed is "ask": surveys, interviews, focus groups. FDE's creed is "watch" and "do" — actions speak louder than words. Three reasons, progressively deeper.

**Layer 1: Customers don't know what they want.** This is a cognitive law. Facing entirely new categories — 2004's intelligence analysis software, 2025's AI agents — users lack a frame of reference to describe requirements.

Palantir's demo loop worked precisely because it doesn't ask "what do you want" but says "here's what I made, tell me what's wrong with it." People's ability to judge "what's wrong" is far stronger than their ability to imagine "what they want."

**Layer 2: What customers say and what they do are two different things.** The lawyer group example from section 2.1 is the best proof: survey research on "willingness to use professional legal AI" would tell procurement strong willingness — after all, they just spent $50,000 on the tool. But observing lawyers' actual behavior, they're using ChatGPT to draft contracts.

In enterprise contexts, "saying" is polluted by too many factors: political correctness, politeness toward vendors, protection of self-image. Only behavior doesn't lie. Shadow work observes behavior; MVD measures behavior — both built on "doing is truer than saying."

**Layer 3: The highest-quality research happens in joint labor.** In interviews, the customer is the "research subject" — guarded and performing; working side by side, the customer is a colleague — relaxed and real. Those two or three days in Bootcamp when FDE and customer technicians write code back-to-back, the information density exchanged exceeds any formal research — customers will casually say during debugging "actually we never trust this field" or "this process nominally goes through the system, but actually we still call."

These words never appear in formal interviews because they seem "informal." But they are precisely the intelligence critical to deployment success or failure.

Interviews themselves are being transformed by AI. Tezign's CTO Ding Xindong shared his approach: no longer sending structured surveys, but using agents to conduct autonomous interviews with all enterprise employees — differentiated communication based on different scenarios and different people's actual pain points, finally aggregating into a global diagnostic map of "what stage each product line is at, what the pain points are, what approach suits for推进." AI has brought down the cost of this all-hands deep conversation.

At this point, the right problem is locked and value is preliminarily verified. The next battlefield is turning validated single-point value into an actual contract and a truly beginning relationship — how to win the customer.

---

## Chapter 3: Winning Customers

> "Enterprises buying AI is like your grandmother getting an iPhone — she wants to use it, but needs you to set it up for her."
> — a16z

### 3.1 Screening Your Lighthouse Customers

The first lesson of internet product customer acquisition is screening seed users: 100 users who love you beat 10,000 who think you're okay. The FDE equivalent is lighthouse customers — those who not only give you revenue but send signals to the entire industry.

Lighthouse strategic value is multiplied in the FDE model for three reasons.

**First, lighthouses are the strongest sales asset.** Enterprise customers have long decision chains and high risk aversion, so peer endorsement is the shortest persuasion path.

Legal AI company Harvey's origin story is a textbook: its first major customer announced in February 2023 was Linklaters, a global elite firm with 3,500 lawyers and 43 offices. Once this lighthouse lit up, PwC, Clyde & Co and other major clients followed — the legal industry values pedigree most; winning Linklaters was equivalent to getting a pass to the entire elite law firm market. Palantir's early history is isomorphic: the CIA was its most demanding and most endorsement-valuable customer; intelligence community trust later became the key to opening Wall Street, manufacturing, and government markets.

Harvey's process of lighting this lighthouse is itself an FDE lesson.

In November 2022, Linklaters formed a dedicated group — the Market Innovation Group, led by partner David Wakeling — and began secretly trialing this then-unknown startup's product. They didn't watch your demo; they went firm-wide live. By pilot's end, 3,500 lawyers had posed about 40,000 real work questions to the system, covering 250 practice areas and 50 languages. Wakeling's conclusion is the quote repeatedly cited in the legal world: "I've done 15 years of legal tech, never seen anything this game-changing." Another partner demonstrated a specific scene to media: asking the system to prepare a ten-page memo for a US client on "how to open a bank in Luxembourg" — "it really did it."

**Second, lighthouses determine your product DNA.** In the FDE model, field learning flows back to product — which means your first ten customers are in fact participating in shaping your product. Once you choose the wrong lighthouse, the product gets pulled toward directions without universality. a16z's first advice to startups, "sell smart," says exactly this: young companies can't satisfy everyone, so choose an ideal customer profile (ICP) with at least some commonalities in system environment and use scenarios, so each delivery's learning accumulates rather than cancels out.

**Third, lighthouse quality matters an order of magnitude more than quantity.** Your capacity is naturally scarce — an elite team can deeply serve single-digit customers simultaneously; once you take a wrong one, the cost isn't "losing one deal" but a top team being occupied by quicksand for half a year. So Chapter 2's three high-risk signals (no business owner, refusing real data, universal requirements) must be checked here too, plus a lighthouse-specific test: agree early in cooperation whether they're willing to stand up after success — joint case publication, industry conference appearances, hosting your potential customers' visits. A lighthouse unwilling to speak publicly for you is worth at least half off.

### Beware of "Requirement Locusts"

Internet products must guard against "product locusts" — early users who swarm in, use up, and leave, while misleading product direction. The FDE equivalent species is "requirement locusts": ample budget,旺盛 demand, but customers who drain your team without producing any compound interest. Three identifying characteristics:

1. Requirements clearly偏离 from company strategic direction — done but no reusable capability accumulated;
2. Treating FDE as cheap outsourcing, assigning work by headcount rather than aligning by results;
3. Enormous internal political consumption — your main work becomes helping one department prove another department wrong.

Saying no to requirement locusts is hard — their contract values are often tempting. But Barry's math is: wrong pilots burn not just current costs, but team time, morale, and the product compound interest that could have grown on the right customer.

### 3.2 Start with the Dumbest Things

Famous incubator YC has an old maxim: "Do things that don't scale." For example, Airbnb's founders once went door-to-door photographing hosts' apartments; Stripe's founders personally helped users install their software.

McGrew, asked on the Lightcone podcast about FDE's relationship to this maxim, gave a precise formulation: the FDE model is doing things that don't scale, at scale.

This sentence breaks through the philosophical undertone of FDE customer acquisition: in enterprise markets, there's no scalable shortcut to trust — only dumb methods. Three layers, progressively deeper.

**Layer 1: People must show up.** a16z's advice list for Forward Deployed teams ends with just four words: show up in person. The reason is "cliché, but clichés become clichés because they're true" — showing up not only improves sales but can multiply success rates when untangling customer internal power relations and driving new tool adoption.

Enterprise customer trust is priced by "number of meetings" and "things experienced together." Video calls can build familiarity, but trust only grows after weathering things together.

**Layer 2: Hands must get dirty.** OpenAI's FDE followed agronomists into Iowa farm fields; Palantir's engineers stayed weeks on oil drilling platforms and aircraft assembly lines; Harvey's FDE did adoption demos partner by partner in law firms. None of these scenes are "efficient," but each produces something remote communication never can: personal feel for the customer's situation. Feel directly translates into solution quality — only by stepping in farm mud do you understand why that seemingly perfect mobile interface is unusable in outdoor bright light.

**Layer 3: First be a servant, then a mentor.** The most common mistake FDE makes early in entry is arriving with a "we're here to save you" posture. Once the posture is wrong, all intelligence channels close.

The correct order is to first do the most inconspicuous services: help the customer's analyst fix a data problem, help IT fill in an API doc, help the business team automate a weekly report. These "dumb things" buy three strategic assets: a real map of the organization (who has the final say, who is trusted, who are hidden key nodes), the truth about the data environment (which data is trusted, which is for show), and most importantly — identity certification that "this outsider is one of us." Once this identity is established, your words start to have weight.

The end of dumb methods isn't staying dumb forever. Chapter 7 will cover how to distill these dumb efforts into replicable playbooks — but before scaling, you must first wade through the mud to find the path worth replicating.

### 3.3 Trust Dividend: The Endorsement Mine of Benchmark Customers

Enterprise procurement is a market of "extremely severe information asymmetry, extremely high cost of failure," and decision-makers' trust hierarchy is clearly layered: vendor's own marketing < analyst reports < peers' public cases < peers' private recommendations. The last tier — "someone I know used it, said it really works" — conversion efficiency crushes all other channels. And the FDE model is precisely the best machine for producing "private recommendation material": what you deliver isn't a software license but a sentence from a customer executive at a peer dinner: "they really know their stuff."

Mining this deposit has three layers of action.

**Layer 1: Make delivery into "a story worth telling."** The premise of customer executives being willing to spread your name is that your delivery can be told by them as a story that makes them look good among peers. This requires delivery results to have three narrative elements: a specific number ("chemical usage reduced 70%," "AML investigations from hours to minutes"), a specific person ("our agronomists worked in the field with their team"), a specific contrast ("used to take three months, this time just five days").

At delivery's end, proactively help the customer's internal supporter prepare this narrative — one page, three charts, a 30-second version. How detailed the materials are determines whether others' retellings stay true.

**Layer 2: Turn customer success into the customer's social currency.** Pharmacy chain Walgreens is the sample: after deploying 4,000 stores in eight months via Bootcamp, it became a star at industry conferences; market research firm J.D. Power went further — after attending Palantir's Bootcamp as a customer, it started running Bootcamps for its own customers. This is the ideal state: the customer displays your methodology as its own industry leadership. Endorsement upgrades from "thank you" to "proud to use you."

**Layer 3: Beware the "backfire mechanism" of endorsement.** Enterprise markets hold grudges. One high-profile failed delivery spreads far faster than ten successes — because failure stories go better with drinks. This is why Chapter 2's "rejection mechanism" and Chapter 4's "activation discipline" are so important: the dead spot of lighthouse strategy isn't failing to find lighthouses — it's letting lighthouses go out in your hands.

### 3.4 Using Data to Map the Customer's Assets

Around FDE entry, there's a move called "entry due diligence" (hereinafter "due diligence"): before writing the first line of code, use structured methods to map out this customer's entire assets. A complete due diligence checklist contains five maps.

- **Data map:** What data sources does the customer have, who owns each, what's the quality, who manages permissions, is there dark data you'd never think of — some old employee's private spreadsheet, reports that only circulate in email, paper ledgers. The focus isn't "what exists" but "which is trusted." In almost every organization, the official data source and the data source employees truly trust aren't the same — the latter is what you need to connect.

- **Process map:** The real operation diagram of the target business process — not the version in process documents, but the version observed through shadowing, including all steps not written down, exceptions, and workarounds. Specifically mark three points: the step consuming the most time, the step where errors cost the most, the step with the most intense emotion. These three points are usually rich mines of value.

- **Organization map:** Who initiates, who pays, who uses, who can veto, who is the uncrowned king. The most common cause of death for enterprise projects isn't technology — it's miscalculating the organizational math — your internal supporter's position isn't high enough, or is too high (too busy to care about you), or the right people weren't included. Specifically look for "knowledge hubs": people not high in position but everyone goes to them with real problems. They're both the best source of requirements and seed nodes for future rollout.

- **System map:** The true face of the technical environment — list of systems to integrate and their interface status, security and compliance boundaries, change management processes. The system map determines your deployment architecture and schedule. Many projects' timelines are doomed from day one because no one asked clearly: releasing a version on the customer side takes a six-week process.

The last map is the most sensitive and most critical: the political map. It answers three other questions: whose cheese does this project move, is the target process to be automated some department's source of power, whose work will look redundant after the solution lands. Imagine a specific scenario: on the system go-live demo day, the fully cooperative business department is applauding, but in a corner another department's director is silent — the process he's responsible for maintaining is exactly the one being automated away. The *GenAI Divide* report lists "employees unwilling to adopt new tools" as the number one roadblock, and the root of resistance is mostly not laziness but fear — fear of being replaced, fear of being proven incompetent, fear of losing reason to exist.

The political map's function is to identify these fear carriers in advance and arrange "new paths" rather than "dead ends" for them in the solution design. Chapter 5's renewal topic will return to this: people you designed as "victims" become the most determined opponents at renewal.

With all five maps complete, you've truly "entered." This due diligence usually takes one to two weeks, conducted separately by "Echo" (Echo, the user research business team) and "Delta" (Delta, the stationed engineer team) with daily syncs. It looks like pure cost, but the math should be calculated this way: two weeks of due diligence saves three months of running hard on the wrong battlefield.

### 3.5 Technical Content Marketing: Building a Continuous Trust Engine

Content marketing is a classic weapon for internet company customer acquisition. FDE companies' customer acquisition logic gives their content marketing a unique positioning: not pursuing traffic, pursuing "pre-sale of professional trust."

The way enterprise customers find you isn't by seeing your ads, but: encountering a problem, searching, inquiring, discovering a company has extremely professional public writing on this problem, then concluding — "they know, find them." Content's role here is "qualification pre-screening" at the very front of the customer decision chain. Palantir has long published scenario-based technical articles; OpenAI and Anthropic make enterprise customer cases into detailed technical narratives; a16z's *Trading Margin for Moat* set the tone for the entire track — these aren't brand promotion, they're carefully managed trust assets.

FDE company content marketing has three iron rules distinguishing it from regular enterprise content.

- **Iron rule 1: Write "trench perspective," not "booth perspective."** Regular enterprise content talks about how strong the product is, how big the vision is; FDE content talks about how hard the problem is, how we waded through. Why did former Palantir engineer Barry's article *Understanding Forward Deployed Engineering* go viral in the industry? Because it wrote all the things you can't see from the booth: the waste of reinventing wheels, negative-margin pilots, burned-out engineers — and as a result, this "self-exposing" article became the best evangelism for the Palantir model. Truth from the trenches carries its own penetration, because readers can tell: who's talking marketing speak, who's talking about the reality they live in every day.

- **Iron rule 2: Open-source methodology, create "qualification to be cited."** Publicizing your methodology for discovery, validation, and delivery — short-term looks like teaching peers, long-term is defining industry standards — when the entire industry's customers start using your framework to ask questions ("how do you build your evaluation system?" "what does your deployment checklist look like?"), you've gone from supplier to question-setter. In 2026, practitioner open-source communities like OpenFDE emerged and quickly aggregated popularity, precisely showing this industry's knowledge hunger is far from satisfied; whoever systematically satisfies it first holds the definition power. This book's writing is, in a sense, a practice of the same logic.

- **Iron rule 3: Make the customer's internal supporter the hero in content.** Case articles' attribution logic is subtle: the protagonist should be the far-sighted manager on the customer side, and your team is "the partner who helped him succeed." Giving the supporter a stage is equivalent to handing an invitation to the same role in the next potential customer — "become him."

Beyond content, two other types of assets can "work" long-term on customer engineers' desktops.

One is open-source tools and components. The initiator of enterprise procurement is executives, but technical veto power sits with engineers. Open-sourcing the general modules distilled from delivery — evaluation frameworks, connectors, deployment templates — is equivalent to pre-burying trust votes at the technical end of the decision chain. Anthropic made the Model Context Protocol (MCP, an open standard letting models connect external tools) a public specification, and FDE's deliverables at customer sites are built on this protocol — the first lesson customer engineers learn is Anthropic's tech stack. Resource-limited teams also have a lightweight version: a quick-start pack that lets customer engineers connect sample data and run through in an afternoon is the best sales engineer.

The other is engineer community presence. In target industry tech communities, your engineers' continuous presence — answering questions, sharing pitfalls, submitting code. This presence's conversion path is long, but it reaches exactly the people who hold technical veto power. FDE company hiring and customer acquisition are unified in this action: the best candidate pool and best customer leads often come from the same community.

### 3.6 Procurement, Legal, and Security Review: The Art of Passing Gates

Enterprise market's "gates" are procurement, legal, and security review committees. Many technically successful FDE projects die at these three gates, and die without any technical dignity: contract terms collapse, data processing agreements get stuck, security questionnaires fill to month four.

The key to passing is how you view these three gates: as obstacles, you'll crash at the last kilometer; as part of delivery, they can build advantage — most tech companies answer security questionnaires to month four, while you submit in two weeks, and you've won.

**Procurement gate:** Give them "reportable" tools: clear phased pricing (giving discounting steps), comparable market benchmarks (giving approval basis), measurable result commitments (making "bought too expensive" accusations untenable). Result-based pricing has unexpected advantages here: procurement's hardest approval is "spending where you can't say what you'll get," while "X yuan per resolved ticket" is instantly understandable to procurement.

**Legal gate:** Polish the data processing agreement like a product. Enterprise AI projects' legal focus is highly concentrated: is data used to train models? Where is stored, who can access? Who pays for security incidents? Who's liable for wrong output? Smart teams productize standard answers to these questions — pre-built agreement templates, model usage statements, tiered incident liability frameworks. Palantir survives in the intelligence community by making "permissions and audits" a product core (who viewed what data, fully traceable); Anthropic made "traceable, auditable" a selling point in financial customer cooperation. This gate's trust is mainly designed in advance through product and process, with limited gains from last-minute negotiation.

**Security review gate:** Use a "pre-answered white paper" to gain two months. Efficient teams proactively maintain a security white paper: deployment architecture diagrams, data flow diagrams, encryption and permission schemes, compliance certifications, standard answers to all questions asked in historical reviews — 80% of most questionnaires can be copy-pasted directly from it. Your response speed itself is the most intuitive signal of security maturity.

### 3.7 Ecosystem Bundling: Standing on Channels' Shoulders

FDE era's ecosystem strategy borrows three types of partners' shoulders.

**First: cloud vendors and large platforms.** AWS, Azure, GCP are themselves one of the total entrances for enterprise AI procurement. Entering their joint sales system is equivalent to getting a direct pass to enterprise procurement lists. Cloud vendors' marketplaces also solve a practical pain point: customers can use existing cloud committed spend to purchase your services, bypassing new supplier procurement processes.

**Second: consulting firms and system integrators.** This is 2026's most dramatic ecosystem change. OpenAI's newly established delivery entity "The Deployment Company"'s founding partner list prominently includes Bain & Company (a separate company from Bain Capital), Capgemini, and McKinsey — the world's largest consulting and integration giants, from "potential competitors" to "shareholding allies."

The logic is clear: model companies have technology, consulting firms have customer relationships and industry depth, integrators have delivery manpower — three parties converging can eat the giant "AI transformation" market whole. For startups, the revelation is twofold: both guard against consulting giants eating your delivery layer in ecosystem's name, and see the real dividend of allying with regional and industry integrators — they hold customer relationships you couldn't build in three years.

Almost the same script played out simultaneously in China. In July 2026, ByteDance's Volcano Engine signed strategic cooperation with one of the Big Four accounting firms, EY: co-building solutions around data governance, financial management, marketing growth and other core scenarios, most notably, both parties plan to build a thousand-person FDE team, "creating an AI-native delivery team." Volcano Engine president Tan Dai's words were blunt: the FDE team should "put engineers with both technical and industry backgrounds forward to customer sites, deeply participating in the full process of solution landing." On one side, consulting giants with customer relationships; on the other, model platforms lacking industry depth — FDE became the welding point for both.

**Third: customers' customers.** The highest-level bundling is embedding into the customer's own value chain. After J.D. Power attended Palantir's Bootcamp, it started running Bootcamps for its own customers — Palantir's capability spilled outward through J.D. Power's customer relationships, customer acquisition cost approaching zero.

When designing your delivery, you can pre-bury this "re-deliverability": can this solution let the customer serve its customers? If yes, you're embedded in the customer's business model.

### 3.8 Scheduling: Who Goes First Is Itself Strategy

Scarcity can create allure — invitation-only, queue mechanisms are classic internet product plays. FDE's scheduling problem is opposite in shape but connected in principle: your capacity is always less than demand, so "who goes first" itself becomes a strategic tool.

First the brutal reality constraint. A qualified Forward Deployed squad (one business-side plus two-three tech-side) can typically deliver no more than two projects simultaneously at high quality. Another industry metric can corroborate: one CSM can manage 8-12 customers simultaneously, while one FDE deeply embedded customer is only one to three, single customer deployment often means 30-60 days of daily on-site presence. OpenAI started with 2 engineers in early days, Sierra's deployment cycle is measured in months, Harvey's single-firm deployment takes six to nine months — elite delivery capacity is naturally scarce.

Capacity scarcity can't be avoided; what can be managed is what price you set for this scarcity.

The first red line of pricing is contract size. Investor Tomasz Tunguz did the blunt math: assigning a $200K/year FDE to a $10K contract never adds up — this model only starts working above approximately $100K per contract. The various scheduling calculations to follow must first cross this bottom line before discussion. Converted to the Chinese market, this red line roughly corresponds to projects at the several-hundred-thousand to million-RMB level — the 10-person squad math from section 7.8 can be used to check your own numbers.

The first principle of scheduling is to rank by strategic value, not contract amount. The decision matrix has only two dimensions: this customer's lighthouse value (industry signal strength) and this customer's learning value (how much reusable capability can be accumulated). Customers high on both dimensions can even should be done at a loss with priority — Barry recalled Palantir's early free pilots burning millions, betting on exactly this matrix. Big contracts low on both dimensions are the most dangerous: money looks plenty, but it ties up an elite team for half a year.

The second principle is to productize "waiting." Customers queue three months before entry — don't let these three months go to waste: give them data preparation checklists (speed up on entry), organizational warming suggestions (which key people to win over first), lightweight remote diagnostics (maintain temperature, sweep mines ahead). A well-managed waiting period can shorten post-entry delivery cycle by a third — queuing goes from customer experience burden to part of delivery quality.

The third principle is never promise parallelism beyond capacity. Your delivery quality depends on the same team's continuous focus — each project carries a full set of customer context, switching once requires reloading once, multi-project parallelism losses far exceed imagination. Rather let sales sell "our schedule is booked to next quarter" as scarcity (this can often raise prices), don't let the team run ragged between three customers. The better business gets, the more tempting to take more orders. And the cost of collapsing from over-ordering is often far greater than the cost of one less order.

### 3.9 Writing Proposals and Validation Plans

The highest unit-price text in enterprise markets is proposals and PoC plans.

The bad news is most technical teams' proposals make the same mistake: all about "what we'll do" rather than "what you'll get." A good FDE proposal follows a strict inverted pyramid structure.

**Layer 1: Business results, one paragraph.** The proposal's first paragraph must be business results in customer language: "Within eight weeks, reduce your bank's AML investigation average processing time from 4 hours to 15 minutes, releasing investigation capacity equivalent to 2.5 times the existing team." Without this sentence, customer executives won't read what follows.

**Layer 2: Value validation path, how you'll prove it was achieved.** Specify acceptance metrics, measurement methods, baseline data, and exit mechanisms for each phase. This layer's signal is "we dare to be tested" — in an enterprise market hurt by over-promising, daring to be tested is the scarcest sincerity.

**Layer 3: Delivery method, how we do it.** Only at this layer does the technical solution appear, and the writing must let non-technical readers follow: architecture diagrams with business annotations, milestones with decision points. Specifically state what the customer needs to cooperate with — data access, key personnel's time commitment. Writing clearly what the customer should do both sweeps mines ahead and screens customers.

**Layer 4: Risks and countermeasures, we've thought about how we might die.** Most proposals avoid risks, as if mentioning them is bad luck — while mature buyers choosing suppliers look precisely at whether you dare to spell out how you might die: what if data quality is substandard, what if key personnel change, what if accuracy doesn't meet threshold. This layer is the proposal's trust amplifier, and also Chapter 2's "refusing the expensive PoC graveyard" philosophy embodied in text.

PoC plans have a special feature: they carry the "graduation criteria." The plan must specify cycle limits, acceptance metrics, and two follow-ups after graduation or parting. Vaguely written validation plans are equivalent to issuing a construction permit for the PoC graveyard.

This "dare to be tested, write dead standards" approach has a precedent from a decade before the AI era. Data analytics company Looker from 2013 did heavy pre-sales implementation during free trial periods, with one principle: the demo is the PoC — always ask potential customers for real datasets to play with, never perform with carefully prepared sample data. At the same time, they calculated the math to the end: about $25,000 per customer per year, two thousand customers is $100 million in annual revenue, enough to reach the IPO threshold. Their then-CEO's words were direct: if you can't say whether you need two thousand or a hundred thousand customers, you're burning VC money.

How bold a validation plan can be written depends on how clearly the math behind it is calculated.

The buyer-side standard is also hardening in the same direction. HR software company Rippling, when selecting vendors, wrote "suppliers must invest dedicated engineering resources" into hard standards — the custom interface workflows they wanted couldn't be done without vendor engineers on-site. Collaboration docs company Notion is the same: it's itself an AI-first company, yet after weighing still chose to buy rather than self-build, its RFP listed five standards, the last being: not just a supplier, but a team that can co-build. Facing such buyers, however beautiful the proposal is isn't enough — Chapter 2's "three gates must be passed at the customer site" starts from the bidding moment.

### 3.10 From On-Site to Remote: The Boundaries of Hybrid Delivery

FDE delivery has undergone an important evolution in recent years: from pure on-site to a hybrid model of "remote-first + on-site at key milestones." Palantir's official line also confirms that many projects today are mostly executed remotely, with on-site concentrated at key milestones.

Hybrid model's rhythm design is a craft. What must be physically present? Experience boils down to three types: 1) early relationship building (first meetings, shadowing, trust-building with executives — trust can't be built through screens, must meet); 2) high-intensity co-creation (Bootcamp-style joint building, key architecture decisions' whiteboard assaults); 3) politically sensitive periods (solution rollout, department coordination, change management — these moments, you need to read the air in the meeting room).

What's actually better remotely? Deep coding, documentation, routine iterations — work requiring undisturbed flow.

Hybrid model also has two hidden dividends. First is cost structure: on-site is one of the largest variable items in FDE costs; a reasonable hybrid ratio can pull delivery profit margins out by more than ten points.

Second is talent sustainability: teams with half their time traveling year-round have significantly higher burnout rates — forum practitioners' complaints about travel rank top. On employer review sites, Palantir's FDE position reviews spell out this split clearly: compensation and benefits 4.0/5, but work-life balance only 2.8/5, with frequent complaints about work rhythm being constantly interrupted (third-party aggregate, not verified item-by-item against original pages). Hybrid model isn't slacking — it's organizational endurance insurance.

But the bottom line must be drawn: projects where you never meet in person lose not just relationships but first-hand cognition of the field. Remote maintains existing trust and context — but they must first be created in the physical world.

Push the boundary further and it's going global. American companies' globalization is demonstrated by giants: OpenAI's FDE hiring map has spread from San Francisco, New York to London, Tokyo, Singapore, Abu Dhabi — the team's geographic distribution precisely traces the global map of enterprise AI paying ability. The Chinese context has different logic: past difficulties were "product DNA" — domestic vendors long did highly customized project-based business, mismatching the standardization and productization overseas markets want. But the FDE model gives a reverse perspective — Chinese engineers' delivery culture is precisely closest to FDE's requirements; the real question is whether the platform foundation behind them is thick enough.

Local reference systems have been quietly running for a long time. 53AI has charged by results since 2023 — paying only when the customer's business actually improves, earlier than Silicon Valley peers. Tuition was also paid: early on they let prompt engineers single-handedly deliver, couldn't see through the customer's business, the founder spent half of a year and a half putting out fires everywhere; after changing to business experts entering first to thoroughly understand the business, then bringing engineers in to build, the situation turned around. The hardest evidence comes from a controlled experiment: a top online education customer, the "sales plus agent" group's output reached 3 times the pure human group. More worth recording is the customer's reaction — after efficiency improved, the customer didn't lay off people, but used the same people to grab more quality leads in the market.

On specific going-global strategy, FDE has one innate advantage and one innate constraint. Advantage: the "lighthouse to endorsement" logic works equally in global markets, and developed countries' enterprise customers' willingness to pay and contract spirit are more mature. Constraint: FDE is a heavily localized business — language, time zones, compliance, local trust networks, each requires local teams, not remote support. This means FDE going-global's cost structure is naturally higher than SaaS going-global, and the pace must be more restrained: first stand firm with remotely deliverable products, then build local delivery teams in key markets, country by country.

These ten things boil down to one sentence: winning customers, in a market let down countless times, means achieving trust. Signing the contract is just an entry ticket — next, the real hard battle begins: making the system come alive, making people use it.

---

## Chapter 4: Activating Deployment

> "The model is usually the cleanest part. The hard part is finding that workflow nobody wrote down."
> — A frontline FDE
>
> "No matter how technology evolves, the human nature and power dynamics within organizations remain a more complex problem than technology."
> — Shen Yue, frontline FDE practitioner

### 4.1 Go-Live Doesn't Equal Activation: The "First-Day Curse" of Enterprise Deployment

"Activation" in consumer internet means new users complete key behaviors and experience the product's "aha moment." In enterprise deployment, activation means **the target user group forms stable usage habits in daily work** — not applauding at the demo, but the system still being used at high frequency three months later with no one pushing.

In other words: enterprise software's "go-live" only completes the procurement and acceptance administrative process; "activation" happens in users' behavior. Go-live day is worth celebrating, but whether the project ultimately succeeds depends on whether anyone's still using it three months later.

MIT NANDA Lab's *GenAI Divide* report has a set of numbers: only about 40% of enterprises provide official AI tool subscriptions for employees, while up to 90% of employees use personal consumer-grade AI tools for work daily. This means many enterprises' real state is "dual-track": official system idling, shadow AI rampant. System went live, but activation never happened.

Why do enterprise deployments universally die at the activation stage? Because it must pass three gates — completely different gates from consumer internet products. Consumer products die from "not fun"; enterprise deployments die in users' hands — users find it not smooth: one extra step beyond old habits and nobody uses it; users find it not trustworthy: one mistake and trust goes to zero; users find it irrelevant to themselves: then nobody touches it.

None of these three gates can be solved at headquarters — you can only pass them in the customer's meeting rooms, workshops, and workstations. So activation is FDE's home turf, and its biggest difference from traditional "deliver and leave" implementation: traditional implementation treats the acceptance form as the endpoint; FDE treats change in customer behavior as the endpoint.

### 4.2 Rapid Iteration: The "Hotfix" Culture of Deployment

Internet product iteration relies on A/B testing, approaching optimal with small fast steps. But enterprise deployment scenarios can't do strict A/B testing — samples too small, interference too much. Yet its spiritual core — fast, small-step, evidence-based iteration — becomes a way of working during deployment: rapidly responding to every small user complaint like repairing a production incident. I call this "hotfix."

Consumer internet products' iteration rhythm is measured in "versions" — weekly, biweekly. FDE deployment-period iteration is measured in "days" or even "hours": morning, business user says "this output is missing the vendor code field," afternoon the field is added; today the workshop director says "this interface can't be tapped accurately wearing gloves," tomorrow the button doubles in size. This response speed's meaning to users far exceeds the feature itself — a problem raised in the morning fixed by afternoon builds more trust than any promise. Users form a judgment in the first month: "this team is for real" or "another deliver-and-leave."

This rhythm isn't just slogans.

Brand performance marketing company Skai took on such an urgent requirement: thousands of products needed unified classification across multiple e-commerce platforms. In the past, this meant pulling in the data science team for scheduling — "they have tools, but capacity is limited, getting into the roadmap takes a long wait." This time, a small team facing customers doing custom features directly called models on the data platform: day one wrote prompts and ran through on the customer's product library, day two published to production — the same work by traditional methods would take at least a month. The VP leading it summarized afterward: "I don't need to become a prompt engineer, nor an LLM expert." The confidence for hotfix is that the toolchain has been laid next to the problem.

Hotfix culture has three execution essentials.

**First, feedback must reach the person writing code directly, with no relay in between.** Previously, user feedback went through customer success, product manager, scheduling, and finally reached engineers — each relay loses half the context, by the time it's scheduled a week has passed and the user's heart has cooled. In FDE mode, feedback reaches the person writing code directly, ideally the person writing code sits right next to the user — this isn't rhetoric: First American's VP of Data and AI Prabhu Narsina recalled collaborating with platform engineers, his exact words: "They almost met with us daily, wrote code together, debugged together." Palantir shortened exactly this loop: Forward Deployed Engineers can build, test, learn, and feed back on-site, without waiting for a formal product requirement to go through process.

**Second, iteration priority is ranked by "usage blockage," not "feature importance."** Deployment-period trade-off logic is opposite to product period. Product period ranks requirements by strategic value; deployment period asks "what's blocking tomorrow's usage" — a color scheme issue that makes workshop workers think "this is made for office white-collar" is the highest priority; a powerful prediction feature users can't use currently gets scheduled after activation completes. Deployment period first gets usage rate up; feature depth goes after.

**Third, at each day's end ask one question: which moment of the user's tomorrow did today's change make smoother?** Fixing this way isn't just "responsive to every request" — every fix is a conscious act of activation design: you're dismantling friction points between user and system one by one. The friction point list hides in the entry due diligence's process map and daily observation.

OpenAI's FDE work method has a corresponding rhythm division: early co-creation (on-site whiteboard alignment), validation (building evaluation systems, i.e., evals), delivery (multi-day on-site construction). Note that the delivery phase still uses "multi-day on-site" as its unit — the reason it can be fixed this fast is people guarding next to the problem.

### 4.3 Iterating in the Customer's Environment: Evaluation-System-Driven Quality Improvement

Speed is solved; the direction problem remains: what to fix, and what counts as "good"? In AI deployment, the carrier answering this question is a practice that only became mainstream after 2024: **evaluation systems** — continuously scoring the system's output with a set of standard cases.

Traditional software quality has only two states: feature right or wrong, test passed or not. AI system quality is continuous, probabilistic, scenario-dependent — the same answer that dazzles in a demo can be a disaster in a specific business context. Worse, the definition of "good" sits with the business side, not the engineering side: an answer the model considers perfect, a business expert might spot as amateur at a glance. Without this evaluation ruler, AI deployment iteration is running blind: tuned for half a month, whether quality rose or fell, no one can say.

The engineering practice of evaluation systems has solidified into three steps in leading teams.

**Step 1: Grow from real cases.** Evaluation sets can't be fabricated by engineers — they must come from the customer's real business material. The essence of this step is making business experts' implicit judgment explicit and executable rulers.

**Step 2: Make the business side the judge.** Evaluation systems aren't engineers' self-indulgence tools — reviewers must include the business side. The best approach is making evaluation into a form business experts can participate in: side-by-side output comparison, simple good/bad annotation, regular review meetings.

This process has dual dividends: evaluation sets get more accurate, and the business side's understanding of the system deepens — they watch the system answer better each time on their own cases, trust accumulation is seen with their own eyes, not obtained from reports. Chapter 2's Morgan Stanley did exactly this: the ones scoring the system aren't engineers but the financial advisors who use it daily.

**Step 3: Connect the evaluation system to the production loop.** Go-live isn't evaluation's endpoint. Continuously collect real input/output in production, sample-evaluate regularly, alert immediately when scores drop — this turns "quality" from a one-time pre-launch acceptance into continuous lifecycle care. After all, users aren't most sensitive to average quality but to quality stability: one system error causing trust collapse needs ten correct answers to fill back.

What does evaluation-driven quality improvement look like on a curve? Customer service software company Intercom's public case gives a rare complete rising curve: its AI customer service product, first generation resolved only 23% of conversations on average, after switching the underlying model rose to 51%, then deep customization for specific customers reached as high as 86%; Anthropic itself using it for customer service, continuously tuning since its 2024 launch, resolution rate (conversations resolved without human intervention) rose to 79%, resolving about 560,000 conversations monthly. The same climb, Salesforce also walked: tuning its own customer service agent for a full year, the "can't answer" ratio was pressed from 30% to below 10% (Chapter 2 expanded on the other side of its self-use pitfalls).

Go-live day's score is just the curve's starting point, and activation-period quality iteration is measured in quarters.

The John Deere collaboration is the most complete public sample of "evaluation system first." This company wanted to solve herbicide waste: traditional sprayers cover the whole field, while its "See & Spray" technology uses 36 cameras plus machine vision to spray only weeds at speeds of 12-15 mph — covering three football fields per minute. The precision agriculture ideal is huge: the US grows 12 trillion corn and soy plants annually, the best farmland yields 200 bushels per acre, top growers can do 600 — "if every plant could be individually cared for, yield could be transformative." This is John Deere tech executive Justin Rose's original words.

But farmers don't want technology — they want trustworthy advice. OpenAI's Forward Deployed Engineers flew to Iowa, followed agronomists into the fields, first reviewed hundreds of real field operation cases with experts, built a custom evaluation system, then rapidly iterated the model — and had to catch farming seasons, missing planting season means missing a year.

Final result: chemical usage reduced by up to 70%, farmer interaction frequency increased 6 times. First having the evaluation system's definition of "good" — only then these two numbers.

The deeper meaning of evaluation systems is turning the old master's mental "what counts as good" into scoring standards the system automatically executes daily. This is precisely the FDE model's microcosm — customer knowledge is no longer just words in requirements documents but rulers living in the system.

### 4.4 Alternative Paths: Lowering the Usage Threshold

Letting users reach value with the fewest actions is common sense in product design. But enterprise systems' usage threshold is often barriers outside the system. Deployment practice's repeatedly verified "threshold-lowering" techniques are four.

**Technique 1: Parasitize in users' existing interfaces.** Wherever users' main battlefield is, your system should appear there: they work in spreadsheets, you make a spreadsheet plugin; they approve in email, you make approval happen in email; they work in ticketing systems, you embed AI suggestions into ticket cards. Requiring them to log into a new system is equivalent to adding a wall they must climb daily between you and them.

OpenAI at BBVA entered from the ChatGPT interface already used by 120,000 employees; Anthropic through MCP lets models enter customers' existing workflow tools — same logic.

Home retailer Lowe's took this logic to the store floor: employees' AI assistant wasn't made a new system but directly installed in the handheld terminals they already carry, voice to ask about products, inventory. This assistant rolled out to 1,700+ stores, answering over 5 million employee questions cumulatively. The project lead's original words: "If you haven't spent time on the store floor, you can't design for store teams."

BBVA is the best sample of "entering the organization along old habits." Starting May 2024 with OpenAI cooperation, the first step distributed only 3,300 ChatGPT Enterprise accounts — not an all-hands movement, letting seed users play on their own. Employees soon spontaneously created over 20,000 custom assistants (GPTs), of which about 4,000 were used at high frequency; management didn't ban "shadow AI" but did the opposite: "We give everyone a safe platform, let them try with confidence." Simultaneously supporting structured training: 250 executives (including the chairman himself) took classes first, the bank built an "AI Pioneer Network," cultivating a batch of senior users internally called "AI Geeks." Data a year and a half later: employees saved about 3 hours per week on average, 83% weekly active usage, accounts expanded to 11,000. In December 2025, both parties announced bank-wide rollout: 25 countries, 120,000 employees, launching an end-to-end transformation roadmap called "Eight Things." From 3,300 to 11,000 to 120,000 — each expansion happened after the previous step's usage data was published — this is "letting habits walk on their own" activation.

This approach's localized version has a key difference: Chinese enterprises rarely have "employees freely choosing tools" soil, so seeds aren't "distributing accounts for employees to play" but first winning a business division or a line's special budget — the first batch of organizationally distributed accounts is itself legitimacy.

**Technique 2: Default values hide activation rate.** New users facing a blank system's first reaction is "and then?" — most churn happens in these three seconds. FDE's solution is pre-loading "first use": preset templates, prefilled examples (based on the customer's own data), preset guidance (on first opening, there's already a to-do belonging to them). The system on day one should understand what they might want to do better than they do — what you observed in the first few days of stationed observation comes in handy here.

**Technique 3: Translate "asking AI" into "clicking a button."** Enterprise users' proficiency with "talking to AI" is far more uneven than imagined. So letting users organize questions themselves is transferring engineering burden to the least appropriate people.

The mature approach is packaging high-frequency scenarios into one-click actions: "generate last week's anomaly report," "verify this batch of invoices," "draft this customer letter" — behind the button is a complete prompt and process tuned through evaluation. Conversational interaction left for exploration; button-based interaction left for daily use.

The most aggressive practitioner of technique 3 is vendors practicing on themselves first. Salesforce's own help site accumulated over 740,000 knowledge articles; in the past customers had to search themselves when encountering problems; they packaged the Q&A agent directly into the help site, completing launch in two months with low-code tools — today 76% of inquiries are resolved without human intervention (August 2026 access). ServiceNow similarly cut itself first: according to its own disclosure, its own assistant in 120 days since launch ran out about $10 million in annualized value.

Self-activation first is both the best testing ground and the most convincing sales material.

**Technique 4: First be "copilot," then talk about "autopilot."** Facing high-risk, high-resistance processes, don't push automation all the way. Let the system first exist as a "suggestor" — AI drafts, humans confirm; AI annotates, humans adjudicate. Users in confirmation after confirmation build trust calibration of the system's judgment; when confirmation pass rate rises to a certain level, automation comes onto the agenda.

John Deere's solution to this day retains the agronomist's final decision power; financial compliance scenarios' agent designs universally retain human oversight; healthcare even more so — Tampa General Hospital's sepsis early warning to this day is system prompts, doctor adjudication (Chapter 8 will expand on this case that saved hundreds of lives). Copilot first, autopilot later — trading a bit of activation rate for risk-controlled steady progress.

But "human confirmation" has a counterintuitive failure mode: too many confirmations and people stop looking. Anthropic's engineering team published a set of telemetry data: users approve about 93% of permission requests — the more they see, the less carefully they look, approval fatigue makes oversight a dead letter; in one internal exercise, a "help me run this" phishing email succeeded 24 times in 25 attempts.

Their solution is moving the boundary from "expecting people to carefully click allow every time" to the system's bottom layer: default deny, incidents can't breach the wall. High-risk content scenarios push this boundary before go-live: TIME's interactive AI experience for Person of the Year first had red teams simulate thousands of attack methods before release. Copilot needs never just a "confirm button" but also a boundary that doesn't depend on human attention.

### 4.5 The Long War of Integration

Every FDE veteran has a body of scars — they all come from the same war: the integration war with customer "legacy systems" — those old systems running in enterprises for years that no one dares touch.

The war's cruelty exceeds anyone who hasn't been on the front line's imagination. a16z's description in *Trading Margin for Moat* hits the nail on the head: the context AI applications need — historical records, business logic, permission systems — is all locked in enterprises' internal databases, interfaces, and workflows, and connecting them "is never an elective but a required course." Financial industry mainframes, healthcare's hundreds of clinics' heterogeneous systems, manufacturing's dozens of self-governing workshop systems — these environments share: outdated documentation, broken interfaces, half the people who understand them already retired.

This war's strategic points have four.

- **First, treat integration as a campaign, not chores.** Integration work is written as one line "system integration: 2 weeks" in most project plans, then balloons to four months in execution. The root error is treating integration as technical chores — actually it's both technical archaeology and organizational politics, plus data governance — a real hard fight. Correct posture: draw the system map during entry due diligence, grade and schedule integration risks, chew the hardest bones earliest — integration has the most uncertainty, each day of delayed start is a day the entire project timeline runs naked.

- **Second, data problems solved before model problems.** The report has a widely cited insight: many AI projects fail at the bottom because "garbage in, garbage out" — AI connected to ungoverned data sources, the same document randomly hitting ten versions, output naturally untrustworthy. Palantir's solution is ontology: first model enterprise data assets into a layer with business semantics, clarify "which field is authoritative, which version is valid, who has right to see what," AI runs on this foundation. This path's universal revelation is: data governance can't be done once before starting work but runs through the entire project — many AI projects at the end, the main work is actually governance. Even Palantir itself stumbled on this: an internal system was crashed by 2.3 million data entries exhausting memory, the retrospective's first sentence was "we never saw the data this system was really going to process."

The US Navy's "Ship Operating System" is this revelation's most spectacular footnote. In December 2025, the Secretary of the Navy and Palantir's CEO jointly announced a $448 million contract: first covering two large shipyards, three naval dockyards, and a hundred suppliers. Shipbuilding's data environment is a textbook disaster: ERP systems, decades-old databases, paper drawings coexisting. And two pilot-stage numbers shut everyone up: at nuclear submarine manufacturer General Dynamics Electric Boat, **submarine scheduling went from 160 manual hours to under 10 minutes**; at Portsmouth Naval Shipyard, **material review time went from weeks to under one hour**.

The Secretary of the Navy specifically emphasized: "This is not a concept, not a pilot, not research — this is already happening."

First spend great effort connecting data into a unified semantic layer — efficiency miracles can only happen — not the other way around.

The same logic reproduces in three completely different industries. Fast food chain Wendy's: syrup shortage scheduling across 6,450 North American stores previously took 15 employees a full day to check, after connecting to the data platform a five-minute solution. Mortgage giant Fannie Mae: using AI to identify mortgage fraud, detection rate exceeds 99%, far surpassing the original rules system. Citibank: customer credit approval from hours to minutes — AI reads through credit history, transaction habits, industry risk, and affiliated companies in one breath.

Three industries, one common premise: first arrange scattered data into a semantic layer machines can understand — intelligence has somewhere to land.

- **Third, use AI to fight AI's integration war.** One important post-2025 variable: integration work itself is starting to be automated by AI. a16z's envisioned scenario has partially become reality — old systems without interfaces, use browser agents to simulate humans to extract data; field mapping, format conversion, interface document interpretation, largely handed to models. Leading teams' self-requirement: "automate the integration process as much as possible — process mining, data pipes, system integration, interface documentation — this speed advantage compounds." Using AI to do AI deployment work might be this position's most wonderful aspect.

- **Fourth, know when to route around, not conquer.** Not all legacy systems deserve frontal integration: some systems' correct solution is "shadow reading": read-only snapshots, nightly sync; some are "manual ferrying": keep manual steps in transition; some simply "declare isolation": explicitly tell the customer that process's data isn't in this project's scope. Engineer's self-esteem always wants to conquer every fortress, and FDE's judgment is precisely shown in choosing battlefields — the project wants customer results, not technical total victory.

### 4.6 Change Management: Getting the Customer Organization to Speak for You

Activation's biggest soft resistance isn't in technology, it's in the organization. Of the report's five roadblocks, "employee resistance" and "change management" together account for nearly half. Getting the system running, engineers suffice; but getting human behavior to change requires mobilizing the entire organization.

Change management in the FDE context, the core is managing three groups of people.

- **Supporters: your internal allies.** Behind every successful deployment stands a customer-side supporter: they genuinely believe in this thing, willing to stake their reputation to clear the path for you. Linklaters' David Wakeling is typical — as the firm's Market Innovation lead, he was Harvey's in-firm counterpart, advocate, and umbrella. Supporter management essentials: give them presentable material (stories worth telling), give them battle achievements (turn their far-sightedness into career highlights), give them security (when failing, you take the front). A well-treated supporter is worth ten product presentations. Lowe's simply institutionalized this: every AI project must fall into one of three categories — "how customers buy, how stores sell, how employees work" — and must have SVP-level business owner endorsement — "if they're not in, we don't do it."

- **Influencers: informal opinion leaders.** Every organization has a batch of uncrowned kings: senior analysts, workshop masters, the "just ask him" person in the department. They don't hold power but control trust. Their one "this thing actually works" is worth three all-hands emails from management; their one "doesn't work" and the next day no one in the workshop clicks. So activation period deliberately manages this group: invite them to be first testers, take every complaint seriously, make their suggestions visible — "this field was added per Master Wang's suggestion." Making influencers co-authors is the shortest path to cracking the "I don't use things I didn't build" mentality. Device management company Jamf is an extreme sample: after rolling out to 16 departments company-wide, the biggest surprise was "the ones driving the broadest adoption weren't engineers" — the performance conversation tool was built by a business colleague in under 45 minutes, while similar projects used to take a team three months. When the building threshold drops to this level, influencers are no longer just word-of-mouth nodes but direct builders.

- **Harmed parties: interest groups the solution touches.** Automation necessarily redistributes work, and redistributing work necessarily creates harmed parties: approval positions compressed of their sense of existence, departments penetrated of information barriers, old employees replaced of their "unique craft." If ignored, they become the system's most stubborn underground resisters — passively uncooperative, spreading incident cases, voting no at acceptance. Mature change management designs "paths for the harmed" in advance: direct released manpower to higher-value work (with public no-layoff commitments), transform "gatekeepers" into "coaches" (old masters' experience used to train the system), let harmed parties see their place in the future. This is both humanitarian and purely utilitarian — the cost of resistance far exceeds the cost of appeasement.

Ticketing platform Vivid Seats' collaboration with Sierra shows what "all-hands mobilization on the customer side" looks like during activation. After deciding to introduce agents, this company's product, customer experience, and engineering teams all went all in — "once the decision was made, we went 100% in, all-hands retesting." Result: from start to launch in under four weeks, problem resolution rate up 40%, CSAT up 35%.

But more valuable is the follow-up change: after routine questions were taken by agents, the customer experience team shifted from "queuing to put out fires" to root-causing process problems, even having capacity to do service beyond customer expectations; and agent conversation data started feeding back into product — "if ten thousand people ask about the same feature in a month, we can immediately put it on priority. The best moment is: a pattern-driven product improvement means users don't need to ask for help at all." Activation taken to the extreme, users actually need help less and less — this case also foreshadows Chapter 7's "field feeding back to product."

The mobilization structure can also be designed in reverse: not just the customer mobilizing, but the vendor also embedding resources into the customer organization. Lyft's collaboration with Anthropic is a three-piece set: both parties co-build product, Lyft gets early access to new capabilities for testing, Anthropic provides training for Lyft's engineers — result: customer service average resolution time down 87%, thousands of requests resolved directly by agents daily. The cheapest and most easily skipped of the three-piece set is the third, and often it's exactly what determines whether mobilization can take root in the customer organization.

Chinese companies' corresponding samples are also emerging. E-commerce company Dewu's Head of Efficiency Engineering Ren Xiliang broke a ten-thousand-person company's AI transformation into three steps: first build consensus across all staff, lower tool thresholds, let everyone use it first; second divide enterprise scenarios into four quadrants by fault tolerance, high fault-tolerance scenarios (like business analysis) prioritized to AI; third set up a dedicated knowledge operations group, drilling into business teams, moving experts' tacit experience from individual brains into AI-visible space. Consensus, scenarios, knowledge — order can't be reversed: first people willing to use, then pick the right places to use, finally give AI something to work with.

Change management's ultimate test standard is only one: after your team withdraws, is the system still being used. If it's bustling when you're present and rapidly cools after you withdraw, that's not activation — that's dancing accompaniment. A truly activated organization walks forward on its own.

### 4.7 I, Robot — Automating the Delivery Work Itself

Delivering automation to customers is the product itself; automating your own delivery work is efficiency. The latter is FDE team's first lever for escaping "revenue growing linearly with headcount."

FDE's daily work has a startling proportion of templatable repetitive labor: new customer deployment environment initialization, standard data integration pipes, security review questionnaire responses, pre-launch checklists, periodic customer reporting formats. Every action done a second time should trigger a question: "can this become a script, template, or checklist?"

Leading teams' approaches have solidified into four types of assets.

- **Deployment templates:** Package environment setup, permission configuration, monitoring integration into one-click Infrastructure as Code (IaC). New customer entry, day one can pull up a standardized environment in the customer's cloud, rather than configuring from zero for a week. Decagon can compress simple scenario deployment to 15 days, behind which is a highly templated integration layer.

- **Integration component library:** Connectors for mainstream enterprise systems, written once, reused everywhere. Palantir's ontology model essentially takes this logic to the extreme: data integration's output isn't a one-time pipe but reusable, business-meaningful data assets.

- **Checklist culture:** Security review checklists, launch admission checklists, withdrawal handover checklists. This set of checklists shows its value most on the day before withdrawal: stationed engineers and customer's handover person sit down, go through the handover checklist item by item, checkboxes done, only then do people withdraw. Checklists turn "relying on personal experience" into "relying on organizational memory."

- **Automated reporting:** Weekly reports to customers, field intelligence to the company, should be semi-automatically generated. FDE's time unit price is too high to spend on copy-paste — and even less should "forgot to report" sever the field-to-product loop Chapter 7 will cover.

Automation also has an easily overlooked use: handing quality checks to machines too. DoorDash is typical: its AI customer service system handles hundreds of thousands of calls daily, behind which is automated test capacity increased 50 times — without such test capacity, day-level iteration simply doesn't dare run on such large traffic. This is also one of the reasons DoorDash could, together with external expert teams, complete from solution design to deployment in eight weeks.

How considerable automation's compound interest is can be seen from one side: a16z lists "build or buy tools to automate service delivery" as key advice for building Forward Deployed teams, and judges this is the key variable for this generation of AI companies to run faster and with lower unit-price thresholds than the previous generation of enterprise software companies. Sierra's publicly disclosed customer data also corroborates: fastest from start to launch under two weeks, slowest six weeks, some customers resolving over half of inquiries on day one; Palantir compressed the sales cycle from nine months to weeks — none of this is through engineers working overtime, but through turning yesterday's delivery into today's scaffolding.

Former Palantir engineer Barry put this logic more bluntly: the company burned millions on customer pilots, many pilots' margins "literally negative infinite," but management booked it under R&D, not cost — every implementation is first a build-and-learn opportunity, and only secondarily a business deal. "99% of founders and investors can't swallow this." First acknowledging delivery as investment, only then can it produce compound interest.

"FDE is just people sea tactics" — this most common challenge now has its answer here. People sea's problem isn't many people, but everyone doing non-reusable one-time labor. Every delivery is building roads for the next delivery — this way, the same team gets faster round after round.

The system is running, and people are using it. But enterprise business's cruelty is: activation only lets the project survive the first year; whether it can survive long-term depends on renewal. Next chapter: retaining renewals.

---

## Chapter 5: Retaining Renewals

> "If it's bustling when you're present and rapidly cools after you withdraw, that's not activation — that's dancing accompaniment."

### 5.1 Renewal and Churn

Doing business requires math first: acquiring a new customer costs several times retaining an old one. Enterprise business magnifies this math by two orders of magnitude: one large customer's acquisition cost — months of sales cycle, Bootcamp-style investment, PoC costs — often hundreds of thousands of dollars, while renewal cost approaches zero. Renewal rate is the key to whether this business's math works.

First look at churn. Enterprise customer churn is completely different in shape from consumer internet products: consumer product churn is silent uninstalls; enterprise customer churn is a slow death — first usage rate declines, then at meetings someone starts questioning "is this thing really worth it," then renewal negotiations are endlessly postponed with "let's look next year," finally in some budget season it's uprooted entirely. More terrifying is collateral damage: Chapter 3 said enterprise markets hold grudges — one publicized failed delivery gets chewed over for years in the industry's small circles.

Enterprise customer churn causes can be summarized into five categories, ranked by preventability.

- **Value evaporation:** System still running, but no one remembers what problem it solved. This usually stems from value narrative breaks — after the original business problem was solved, no one continuously restates to the organization (especially newly appointed managers) "why we have this system." Value isn't proven once; it needs continuous re-proving.

- **Supporter departure:** Your internal ally gets promoted, transferred, or leaves; the successor didn't experience the original choice firsthand, naturally indifferent or even hostile to the system — "the predecessor's vanity project." Enterprise software has a dark saying: "When the supporter moves, the contract hangs."

- **Quality drift:** Business is changing, data is changing, models are updating, system output quality slowly declines, users' trust slowly collapses — when collapse is noticed by management, it's usually already late.

- **Cost backlash:** System usage grows, bills grow, finance scrutiny intensifies. If value narrative can't keep up with bill growth, "success" becomes a renewal obstacle instead.

- **Supplier withdrawal reaction:** Customer wariness of "being locked in." Gartner analyst Alex Coqueiro gave a stunning prediction in industry media: by 2028, 70% of enterprises will be forced to abandon FDE-led agent solutions due to excessive supplier costs and insufficient internal skills (media report of analyst's personal view, not Gartner's formal prediction report). This prediction itself is a warning to all FDE teams: if your mode makes customers feel kidnapped, the market will collectively resist.

Now look at how to measure "retention." Consumer internet products look at retention rate; enterprise business must look at three layers (complete metrics in Appendix A): usage and activity depth (behavioral layer), Health Score (relationship layer), Net Revenue Retention (NRR; financial layer, measuring whether the same batch of old customers pay more or less this year than last). NRR is the final judge: above 100% means even without signing a single new deal, existing business is growing — this is also "delivery as operations" most direct proof.

What does top-tier look like on this metric? Palantir's Q4 2025 earnings gave three numbers: NRR 139% — old customers automatically growing nearly 40%; Remaining Performance Obligations (RPO, signed but not yet recognized revenue) also up 145% — no worry about business in coming years; single-quarter total contract value $4.26 billion, a record. Management specifically explained one detail: the 139% figure doesn't include revenue from customers signed in the last twelve months — it's purely "old customers' trust appreciating." This company early on was most mocked for "project-based, no repeat purchases" — twenty years later, it proved with the same batch of customers: if intimate delivery can continuously create value, renewal is no longer a sales problem, just a matter of time.

Each of these churn risk types has a corresponding defense line: performance and stability guard against quality drift; lossy service guards against cost backlash; onboarding and training guard against value evaporation at the behavioral layer — usage decays with personnel turnover; organizational maintenance guards against supporter departure; Health Score and early warning intervention mechanisms are the master defense against all five risk types.

### 5.2 Optimizing System Performance and Stability

Consumer internet products' law: one second slower loading, retention drops a chunk. Enterprise systems' performance problems have different pathology: enterprise users' tolerance for "slow" is actually higher than consumers (they're used to old systems' sluggishness), but tolerance for "unreliable" approaches zero. Enterprise system output enters real business decisions — one wrong inventory recommendation's loss may erase a year of system value; errors also get amplified and spread — system errs once, the story circulates in the department for three months; getting it right a hundred times, no one remembers. Trust builds slowly by quarters; destroying it takes minutes.

FDE team's four fortifications for guarding reliability.

- **First:** Clear SLAs (commitments on availability, latency, error rates), and make them visible. These commitments aren't just written in contracts — they're made into monitoring dashboards customers can see themselves. Turn "system is stable" from a position you need to defend into facts customers can check anytime.

- **Second:** Design guardrails for AI's "probabilistic nature." AI systems can't be 100% correct — engineering accepts this reality, product manages this reality: outputs the model isn't sure about must be flagged or routed to humans; high-risk actions must have human oversight; every major model update must re-pass evaluation to prevent old problems recurring — the evaluation system built in Chapter 4 becomes part of production guardrails here.
  - **Guardrail model:** Anthropic in financial institution cooperation made "auditable, traceable" a core design — every agent decision can replay its evidence chain. In financial, healthcare scenarios, auditability isn't a bonus, it's an admission ticket.
  - **Anti-drift model:** The other half of guardrails isn't just blocking errors, it's continuously fixing right. A legal tech company made this into a closed loop: the system tracks contract clause extraction recall rate, each miss automatically generates annotation samples entering nightly fine-tuning tasks — within a month, key clause recall rate went from 92% to 98%, service didn't interrupt a single day. Fighting quality drift relies not on one-time fixes but on making the system self-repair daily.

- **Third:** On-call and response must make customers feel you're always there. System goes down at 2 AM, FDE's reaction speed is the customer's felt temperature of this relationship. Chapter 1 quoted that practitioner's iron rule: "The deployment goes down at 2 AM. You don't file a ticket, you don't blame other teams, you don't go back to sleep. You fix it. Period." This spirit must land in mechanisms: on-call rotation, incident retrospectives, and honest incident reports to customers after each accident — enterprise customers can accept incidents, can't accept concealment.

- **Fourth:** Capacity and cost planning in sync. Usage growth is happy trouble; handled poorly, it becomes a renewal assassin. Performance teams must always run half a step ahead of the usage curve: before customer peak season arrives, capacity, rate limiting, degradation plans are already in place. Eliminate slowness before customers feel it — performance work done well is inherently unnoticed by people.

### 5.3 Lossy Service — Letting Go of Unnecessary Persistence

"Lossy service" is a concept in internet product design: actively degrading in extreme scenarios to preserve core value. This concept has a deeper variant in the FDE context — it concerns the eternal tug-of-war between customization and standardization.

The background is the gravity every FDE team encounters: customers exist, requirements exist; requirements exist, customization never stops. Three months later you look back, this customer's deployment is overgrown with custom features, half used by only three people, maintenance costs all on your shoulders. This math is actually tighter than you think: by market rates, one fully-loaded FDE can only serve three to five customers simultaneously, amortized single deployment annual delivery cost starts around $75K — every bit of long-tail customization eats from this thin margin. Left unchecked, you're carrying a "customization debt" — it gnaws your profit (maintenance costs eat contract income) and binds your feet (one platform upgrade might step on custom landmines).

Here we must separate two commonly conflated figures, or the math goes wrong. The $75K figure is single deployment's amortized direct delivery cost, from industry media's single-source estimate, best treated as a lower bound; Chapter 1's $385K is top lab mid-level FDE's median annual total compensation.

Calculate by the latter: $385K compensation, plus benefits, travel, and toolchain amortization, one mid-level FDE's fully-loaded annual cost approaches $500K; divided by simultaneous customers (fully-loaded at three to five; section 3.8 said deep embedding is one to three), single deployment's amortized labor cost is $100-170K — and this is the ideal state without project gaps and pre-sales investment. Two figures side by side, single deployment's true full cost broadly falls in the $75K-$170K wide range, specific position depends on company compensation level and team reuse rate. Chapter 3's Tunguz "single contract $100K minimum" red line sits right above this range's lower edge — calculated, it's the break-even position. How to calculate from single deployment to an entire team, Chapter 7's final section continues.

The wisdom of "lossy" is actively subtracting on three dimensions.

- **Feature dimension: dare to say "no" to long-tail requirements.** The judgment criterion isn't whether the requirement is reasonable (most requirements are reasonable in isolation) but two questions: does its user count times frequency justify its lifetime maintenance cost? Can it generalize into platform capability (if yes, enter Chapter 7's feedback channel)? Requirements where both answers are no, the best response is providing workarounds, not code. FDE isn't an order-taker — order-taker culture is precisely the obsequiousness the "French waiter" model (Chapter 1's Karp behavioral benchmark: embedded in service process, yet with confidence and taste to guide customers toward truly good directions) opposes.

- **Commitment dimension: tiered commitments, not uniformly highest.** Not every feature deserves four-nines availability. Core transaction links guarded to highest standard; reporting and exploratory features generously accept degradation — degradation strategies (turning off heavy computation during peak hours), off-peak strategies (heavy tasks run at night), and tiered commitments stated to customers in advance. Concentrating reliability resources on vital points is more honest and more sustainable than uniformly mediocre reliability.

- **Cost dimension: proactive usage bill management.** 5.1 said "cost backlash": usage grows bills grow, when value narrative can't keep up, success becomes renewal obstacle instead. Proactive FDE teams act before bills become painful: give cost optimization solutions (caching, batch processing, model tiering — using cheaper models for simple requests), redesign pricing structure (from pure usage to "platform fee plus usage" smooth structure), and most importantly — before the customer's finance lead asks, first calculate "the value account corresponding to this bill" for them. Being called to explain bills puts you on the back foot; teams that proactively calculate accounts for customers are much more composed at renewal negotiation.

The essence of "lossy" is acknowledging resources are always finite, continuously betting limited resources on what customers truly care about. It's in the same lineage as Chapter 2's "refusing the expensive PoC graveyard."

### 5.4 Guiding New Users to Quickly Get Started

After system activation, the user base doesn't stay static: new employees join, organizational adjustments, new departments enter usage scope. Enterprise systems' "new user onboarding" is a never-ending rolling process. Well-designed onboarding mechanisms, usage rate rises over time; poorly designed, usage rate naturally decays with the initial trained cohort's attrition.

Enterprise scenario onboarding is fundamentally different from consumer internet products: consumer product onboarding is one-time self-service; enterprise system onboarding is "person-to-person transmission" organizational engineering. Three reusable structures.

- **Tiered training:** One-size-fits-all all-hands training is the biggest waste. Effective tiering is three layers: deep training for administrators and internal supporters (their future role is internal experts); scenario-based training for regular users (not teaching features, teaching "how to do your daily three things with the system," 30 minutes max); one-sentence training for executives ("open here, this number is the answer"). Tiered training's spirit is in the same lineage as section 4.4: each role only learns the part relevant to them.

- **"Train the trainer" leverage:** FDE teams will eventually withdraw; training work must be handed over before withdrawal. Identify enthusiastic molecules in the customer organization, cultivate them into internal trainers and internal answerers — give official certification, dedicated support channels, and exposure opportunities in front of executives. Anthropic's cooperation with FIS's core design is exactly this: "transfer knowledge so FIS can independently build and expand its own agents." Delivery taken to the end is teaching customers to teach themselves.

Two "person-to-person transmission" scaled trainings are worth comparing. BBVA pushing 120,000 people online relied not on the vendor's training team but two internal roles: a bank-wide "AI Pioneer Network" responsible for workshops and scenario mining in various business departments; a batch of senior users called "AI Geeks" by colleagues, hand-holding people around them. Consulting giant Accenture's cooperation with Anthropic is another order of magnitude: thirty thousand consultants received systematic Claude training, forming one of the world's largest AI practitioner networks — Accenture then brings this team into its own customers. The structure is the same: in the end, the vendor really only needs to train one type of person — people who will go train others.

- **Documentation and self-service systems:** Enterprise documents mostly go unread after writing, unless they meet two standards: organized by task not by feature ("how to handle an abnormal refund" not "refund module feature description"), and embedded in product not standalone (appearing where users get stuck). Documentation is both a handover artifact to customers and a scaling asset for yourself — the next similar customer's training system, 70% can be inherited.

### 5.5 Organizational Maintenance and Single-Point Dependency

"Supporter departure" is the second biggest killer of enterprise renewals, worth singling out for dedicated handling — its universality and deadliness are both severely underestimated.

Single-point dependency forms almost naturally: the project was initiated by the supporter, the relationship maintained by the supporter, the success narrative spoken by the supporter — then one day he leaves. The successor arrives with his own agenda, your system doesn't make his top twenty to-dos, renewal season arrives, no one speaks for you, the contract dies silently. Countless "clearly used well but got cut" systems in the industry die from this script.

What this script looks like on the ground: at the renewal review meeting, the newly appointed lead flips to the system page, asks "what is this," no one in the room can answer — people who use it don't dare speak for budget, people who can speak haven't used it. Contract expiration day, no disputes, no complaints, just no one initiates the renewal process. Servers still running, monitoring dashboard all green.

Defense works must be built in three places.

- **Relationship gridding:** From the day you become aware of single-point risk, systematically broaden the relationship net: beyond one supporter, develop at least two independent relationship lines — business line's daily user community (internal trainers are natural nodes), and a higher-level executive sponsor. High-level relationships don't need frequent maintenance but must stay visible at key nodes (quarterly reports, before renewal). Relationship grid's test standard: any single person leaving, information channels don't interrupt.

- **Value organizationalization:** Rewrite the system's value from "supporter's political achievement" into "organizational asset." Specific actions: regular all-hands briefings on value data (letting using departments feel indispensable themselves), repeated telling of success cases at customer internal meetings (forming collective memory), and embedding the system into process documents (when the system is written into standard operating procedures, replacing it requires rewriting processes, cost skyrockets). The goal is making any newly appointed manager conclude "this system is fixed asset here" in their first week.

- **Departure should also be made a ritual:** When supporters leave, most vendors' reaction is passive lament. The correct reaction is treating it as a relationship-building opportunity: hold a dignified "achievement" ceremony for the departing supporter (thank-you letter, achievement summary, gift him portable professional capital — like qualifications to share cases externally), while immediately starting handover with the successor — with "helping the successor quickly produce results" as the entry point, not "persuading him to keep our system." Departing supporters going to new employers are potential entry points for your next customer; treating departees well is converting churn risk into customer acquisition channel.

### 5.6 Designing Health Score and Early Warning Intervention Mechanisms

The final section gathers all renewal-guarding actions into one system: the customer health score system. Its goal is making "relationship deterioration" from a sudden death into a slow curve detected long ago — you always have time to intervene.

Health score's view, enterprise customers and consumer internet products are different. Consumer products watch retention, DAU suffices; enterprise customers must simultaneously watch four types of signals: usage signals (weekly active user trend, what percentage of key functions are used by people, real use or check-in), value signals (how are the originally defined business metrics now, whether the ROI story still holds), relationship signals (supporter employment status, executive contact frequency in last 30 days, customer response speed to your team), commercial signals (usage-to-bill ratio trend, contract expiration time, competitor movements). Synthesize these four signal types into one health score, alert when dropping below warning lines. Health score's biggest use isn't the score itself — it forces the team to review all customers one by one weekly.

**Quarterly Business Review:** Turn "what value we created" into a fixed quarterly program. QBR (quarterly meeting where vendor and customer align value and plans) is enterprise services' most important renewal engineering, yet often becomes a meeting where the vendor unilaterally shows slides while the customer looks at phones. Good quarterly reviews have three disciplines: 1) speak the customer's language, not your product language ("how many person-hours we saved you this quarter" not "what features we launched this quarter"); 2) let the customer's business side be the protagonist, not the audience (the supporter tells his team's story, you provide data ammunition); 3) close with "next quarter's value plan."

What counts as "speaking the customer's language"? Education publisher Wiley's quarterly story is a model: 213% ROI, seasonal customer service onboarding training speed up by half, plus an unexpected gain — ticket classification data let it hold distributors accountable with ticket turnaround time (TAT). Such quarterly reviews, customer executives will move their own chairs to attend. Breaking renewal into quarterly value alignment, signing on expiration day often becomes just a formality.

**Early warning and intervention:** Usage declined, what to do. Consumer internet products rely on push notifications and email to wake users; enterprise customers' "wake-up" is another set of rules — churn warning and intervention must rely on "people plus data" combined tactics: health score drops, tiered response immediately activates: mild decline (a department's usage decreased), corresponding internal trainer home visits; moderate decline (overall activity down 30%), FDE team launches special diagnosis — usually one of business change, personnel change, or quality drift, treat accordingly; severe decline (near abandonment), executive level intervention, honest dialogue "is it still worth continuing" — sometimes the answer is a graceful exit or downgrade, preserving relationship and reputation, leaving a door for future reunion.

There's another layer of wake-up that happens inside your deployed system. Sierra discovered agents' most unexpectedly strong suit is negotiating retention: a travel platform it serves had agents proactively intervene at users' "swing moments" of hesitating to cancel — helping users clarify package benefits, explore alternatives, dig out overlooked value — package retention rate rose 5%. When your system starts guarding its customers for them, your identity at the renewal table changes: from a cuttable cost to a golden-egg-laying goose.

At this point, the five defense lines for guarding renewal are complete. But enterprise relationships that only defend without attacking will shrink — within customer organizations, there's always the next unsolved problem. Next chapter, offense: how to grow the business on the foundation of a successful deployment.

---

## Chapter 6: Expanding Revenue

> "The sign the FDE model works is: each subsequent customer's customization volume decreases."
> — Bob McGrew

### 6.1 The World of Free Validation

The internet economy turned "free" from gimmick to strategy. FDE can't avoid this "free" hurdle either, just the hurdle looks different: in the enterprise AI era, free proof-of-concept is the most expensive kind of free.

First look at this free economy's scale. Palantir's AIP Bootcamp essentially made free validation into an assembly line: customers bring real data, a deployable prototype is built in one to five days, charged zero or nominal. Starting from fewer than a hundred sessions in 2022, sessions multiplied year over year, averaging nearly 6 per day at the 2025 peak — counting several top engineers per session per day, this is tens of millions of dollars annually in free investment. Former Palantir engineer Barry recalled earlier days more bluntly: "We burned millions on customer pilots, many projects had literally negative infinite margins because we did them for free."

Why does free validation work? Three math books add up.

**First book, customer acquisition.** Traditional enterprise software relies on sales armies for acquisition: travel, dinners, tenders, long negotiations — money spent abundantly and uncontrollably. Bootcamp changed the game: don't persuade customers, let customers persuade themselves — executives clicking a system running on their own data beats a hundred pages of slides.

Palantir's sales cycle compressed from 9-12 months to weeks, US commercial revenue up 137% year-over-year in a single quarter, free Bootcamps being the recognized main engine. Free validation isn't pure cost: it's converting sales expense into engineer expense, and engineer expense can precipitate into product.

**Second book: power of risk pricing.** McGrew's advice is early startups should actively bear risk: "you pay us when it works." Confidence comes from product strength, and from a cold calculation — enterprise customers' biggest doubt about new suppliers is "are you capable," free validation is this doubt's solvent. When doubt dissolves, subsequent pricing power returns to your hands: customers no longer buy "a gamble" but "certainty personally verified" — certainty can be premium-priced.

**Third book: even failure must make failure valuable.** Free validation inevitably has failures — this is portfolio investment common sense. The difference is where failure goes: traditional sales failure leaves a pile of travel invoices; FDE-style free validation failure leaves an understanding of an industry, a batch of reusable components, a set of evaluation data. As long as you've built Chapter 7's feedback mechanism, failed validation is also depositing for the company.

But free validation has one fatal prerequisite: the graduation (conversion) day must be designed — cycle limits, acceptance metrics, expiration-to-paid agreements. Without these, free becomes indefinite residence. This leads to the next section.

### 6.2 The End of the Free Lunch

Free is the means, charging is the purpose; conversion design determines where all prior free investment ends up. In the FDE world, "validation to paid" is the most critical kick, and the industry's highest-accident segment — the "PoC graveyard" repeatedly mentioned in earlier chapters, mostly not because of technical failure, but because no "ending" mechanism was designed.

From free to paid conversion, there are five switches that must be pre-designed.

**Switch 1: Graduation criteria before starting work.** The "design the graduation day" requirement must be written in black and white at validation project launch, not added after starting. Palantir's Bootcamp took this design to the extreme: on the Day 4-5 schedule, "demo" is immediately followed by "decision." Conversion isn't a post-hoc event, it's a slot on the schedule.

**Switch 2: Make free boundaries explicit.** Customers must clearly know: free until what date, covering what scope, how excess is priced. Blurry free boundaries cultivate "free is normal" expectations; when charging day arrives, the other party's feeling isn't "starting to pay" but "getting ripped off" — same money, different expectation, experience worlds apart.

**Switch 3: Make internal supporters into salespeople.** This switch is most counterintuitive: after validation success, the one who really knocks on the budget door isn't your sales, but the customer-side supporter who personally witnessed value. What he can produce when he walks into the finance lead's office determines whether this door opens.

The finance lead looks up, usually asking only three questions — what has this thing brought now? What would be lost if stopped? Why pay more next year? How many of these your supporter can answer depends on how much ammunition you saved for him during the free period. Meetings where he can't answer end with "let's look next year."

Your job is to arm him: a one-page value report (numbers, comparisons, colleague testimonials), Q&A for financial challenges, and "if we don't continue" opportunity cost statements. Internal people selling has an internal trust level external people can never reach.

**Switch 4: Pre-bury price anchors.** Start talking value during the free period — "this system released about 120 person-hours for you this month." Value narrative runs through the free period; when the quote appears, customers already have anchors in mind; while free period only talking features not value, the quote is a sudden shock.

**Switch 5: Design a graceful exit for "not converting."** Not all validation should convert; forced conversion is poison contracts. For substandard or untimely customers, give a "pause but retain" option: retain data and configuration, agree restart conditions, maintain lightweight contact. Enterprise markets are small; today's "next year" is often the year after next's big deal — provided you make the farewell professional.

Five switches combined are essentially one sentence: design "free to paid" from a thrilling leap into a gentle slope.

### 6.3 Charging by Results: Customers Pay for What They Get

FDE's pricing principle is blunt: customers get how much value, you charge how much money.

SaaS era's mainstream pricing is per-seat — paying for "right to use." This logic is being eroded in the AI era: when one agent can do 10 people's work, per-account charging becomes a joke — pay for 0.1 accounts? So "charging by results" has risen, Sierra charging per "resolved conversation" being the most eye-catching sample: customers don't pay for software, they pay for "problems solved."

Charging by results' evolution chain has four tiers, each higher tier closer to value, and harder to execute.

**Tier 1, by usage:** Charged by tokens, API calls, processing volume. Advantage is clear and measurable, disadvantage is it tracks cost not value — high usage might mean high value, or system inefficiency. Model API per-volume charging is the industry's common baseline, but application-layer companies rarely use it as sole pricing.

**Tier 2, by task (per-action):** Charged per "completed a return processing" or "generated a compliance report." A step beyond usage, pricing unit starts having business meaning.

**Tier 3, by results:** Charged per "successfully resolved conversation" or "recovered bad debt." Sierra's per-resolution charging, some risk-control companies' commission on recovered losses, are at this tier. Execution difficulty is attribution — "resolution" determination requires mutually agreed judgment criteria (this is exactly Chapter 4's evaluation system's commercial use: technical evaluation system, simultaneously billing infrastructure).

**Tier 4, by value share:** Commission on financial value created for the customer — costs saved, revenue recovered, capacity released. This is the ultimate form closest to value, and hardest: requires customers opening financial data, requires anti-cycle trust, requires extremely strong value measurement ability. Currently only appears in some deeply bound high-unit-price scenarios.

Companies charging by results must dare to make results public. Sierra's own published customer data constitutes an interesting report card (all vendor self-reported): property management company Funnel Leasing, resolution rate 94%; fintech company Ramp, 90%; mattress brand Casper, 74% with customer satisfaction up over 20%; WeightWatchers, about 70%, satisfaction 4.6/5; even the worst-performing customer has 64%.

Third-party estimated price points have also surfaced: annual contract threshold about $150K minimum, first-year budget including deployment fee commonly $200-350K, large customers can reach millions per year; reportedly, per successful resolution pricing is $1-2. In other words, every cent the customer pays corresponds to a "problem actually solved" — Sierra dares charge this way because its evaluation system can prove "resolved" to customers. Pricing method and evaluation system are two sides of the same coin here.

Charging by results' ceiling is "results" themselves becoming revenue. Window treatment brand Hunter Douglas's customer service agent crossed this line: according to Decagon's published customer case, it has over $1 million in revenue from conversations fully handled by AI, never transferred to humans — the customer service department, a traditional cost center, for the first time has its own revenue attribution. Vendor case page numbers need a grain of salt, but "customer service becoming revenue" direction is real.

When choosing pricing tier, there's a plain judgment principle: the closer the pricing unit to customer value, the higher your pricing ceiling, but the higher your measurement and trust costs too.

There's another consequence few people calculate carefully: what pricing tier does to your financial statements. Per-seat subscription, revenue stable and predictable, capital markets give software valuation; charging by results, revenue fluctuates with customer resolution volume, payment rises and falls with acceptance rhythm — revenue recognition timing, accounts receivable days, cash flow predictability, all worsen. Sierra's model equals taking usage risk originally borne by customers onto its own shoulders: customers use less, your revenue is less, while your engineer costs don't diminish a penny. This isn't opposing charging by results — its value to customer relationships was stated earlier — but a reminder: companies choosing high-tier pricing, cash flow reserves and cost structure must withstand revenue fluctuation. Pricing space is traded for volatility; first confirm you can afford the trade.

"What value metrics written into acceptance criteria" looks like in contracts? An executable clause specifies at least five things:

- **Metric definition:** "Resolution" means end-user accepts answer and doesn't escalate to human within 24 hours.
- **Baseline and measurement window:** Pre-launch 8-week average as baseline, measured quarterly.
- **Judge and data source:** Based on mutually agreed dashboard, not vendor's unilateral report.
- **Dispute arbitration:** When data disagrees, third-party audit or joint review, not renegotiation.
- **Abortion clause:** When customer data foundation is substandard, metrics can't be measured, how costs and responsibilities are shared.

The most often omitted of the five is the last, and the one that hurts most when incidents happen. Missing any of these, "charging by results" at the acceptance table degrades into "charging by relationship."

For Chinese market readers, a realist footnote: domestic enterprise customers' acceptance of "subscription" is still limited to this day, "buyout plus implementation" and "pay by project acceptance" remain mainstream. FDE model's landing in China pricing often needs East-West fusion: phased delivery acceptance (accommodating project-based habits) + value metrics written into acceptance criteria (injecting results-based genes). Pure subscription is ideal here, while mixed system is the survival path.

### 6.4 Existing Account Deep Cultivation: From One Department to a Large Network

Enterprise markets have an iron law: the biggest revenue growth isn't in new customers, but inside old customers. The industry uses NRR (see Chapter 5) to measure this; excellent FDE-driven companies' NRR stands above 120% year-round — even without signing any new deals, existing revenue naturally grows 20%. Palantir's commercial story is essentially an existing account deep cultivation story: from one intelligence group to the entire agency, from one factory to the entire group, from government departments to commercial empire.

Existing account deep cultivation's approach has an industry vivid phrase: "land and expand." Landing relies on the previous five chapters; expansion has three directions.

- **Horizontal: from one team to adjacent teams.** You helped customer service build smart tickets; the neighboring after-sales department, technical support department are your next easiest wins. Horizontal expansion's most persuasive evidence sits inside the customer: same company, same data environment, neighboring department colleagues speaking from experience — this is expansion with smallest sales resistance, almost no need to rebuild trust. Harvey's expansion in law firms is this rhythm: single business group entry, six months of real combat validation, horizontal expansion to the whole firm.

- **Vertical: from execution layer to decision layer.** Initial projects usually serve frontline executors; vertical expansion transmits the value chain upward: analysis and early warning for middle management, decision dashboards for executives. Vertical expansion's significance isn't just revenue, it's security — Chapter 5 said systems only loved by grassroots have no defenders at budget season; while systems entering executives' view enter the organization's "fixed asset" ranks.

- **Depth: from auxiliary tool to core process.** The deepest expansion is making the system from "helping tool" into "indispensable process" — from "giving suggestions" to "executing business actions," from "optional" to "part of standard operating procedures." Each step of depth expansion comes with greater responsibility and higher trust threshold, but also builds the deepest moat: replacing a tool just requires changing software, while replacing a process-embedded system equals surgery.

Two "land and expand" report cards are worth comparing. Harvey from Linklaters one law firm start, by 2026, users exceeded 100,000 lawyers, 1,300 organizations, covering most of the US top 100 law firms, 500+ corporate legal teams and 50 asset management companies, across 60 countries; ARR from about $100M in August 2025 to about $190M in January 2026 — nearly doubled in five months. Industry surveys show 68% of surveyed law firms use Harvey's agents in production, deep users average saving 11 hours weekly. Valuation jumped four times in one year: $3B, $5B, $8B, $11B. While Palantir's NRR 139% report card was covered in 5.1 — two tables together illustrate existing account deep cultivation's logic: new contracts driven by marketing, but revenue growth mainly grows from inside old customers.

Expansion also has a quieter form: eating others' line items on the customer's budget. According to Decagon's published customer case, ClassPass's AI customer service after launch, actual auto-deflection volume was 10 times expected; then a small thing happened — its AI translation quality surpassed the originally hired localization vendor, whose contract expired unrenewed. Customer's budget didn't grow, just changed owners. Depth expansion to a certain depth, your competitors are no longer peers, but other vendors on the customer's budget sheet.

These expansions share the same rhythm discipline: expansion must be led by value, not sales metrics. Chapter 5's health score system has offensive use here: departments with high usage depth and clear value are the next expansion targets; and moments in the customer organization when "seeing others use it well, proactively asking" are expansion's golden windows — at this point you're not selling, you're responding to demand.

### 6.5 Watch Anthropic and FIS Play the Financial Services Card

2026's enterprise AI market's most specimen-worthy cooperation deserves a complete look — Anthropic and fintech giant FIS co-building financial crime agents.

FIS is a global financial technology infrastructure giant, serving banks' core systems worldwide. In May 2026, FIS released financial crime detection agents, first customers being Bank of Montreal and Amalgamated Bank. What this agent does: compress anti-money laundering investigations from hours to minutes — automatically compiling evidence across bank core systems, presenting to investigators sorted by risk, fully auditable and traceable throughout.

In approach, four moves interlock.

**Move 1: Embed, not deliver.** Anthropic sent Applied AI team and Forward Deployed Engineers, directly embedding into FIS, co-designing with FIS experts. Note: FIS isn't the end customer, but a channel-level partner — Anthropic's agents will enter hundreds of banks behind FIS's products through FIS's products. This is one deal, and also the entry to a hundred deals.

**Move 2: Knowledge transfer as selling point.** Official statements specifically note: embedding's goal includes "transferring knowledge so FIS can independently build and expand more agents in the future." Writing "teaching the customer" into the contract — this is both a preventive response to "vendor lock-in" concerns (echoing 5.1's "supplier withdrawal reaction"), and a sophisticated binding: when customer's tech stack grows on your methodology, separation costs only rise higher.

**Move 3: Auditability as product feature.** Financial compliance scenarios, regulators require every decision replayable. Anthropic made "fully auditable, traceable" the agent's core selling point, not an add-on feature — this gives all regulated industries a template: what others see as compliance cost can be your pricing reason.

**Move 4: Ecosystem amplification.** Same day as the FIS case announcement, Anthropic also announced financial services connectors and "ready-to-use" templates, plus a dozen similar cooperations — a single case, immediately abstracted into replicable product assets. Around the same time, market reports surfaced of it forming an enterprise AI services company with Blackstone, reportedly about $1.5 billion, directly competing with OpenAI's Deployment Company.

This card game also has a hidden line — CIOs' alertness. CIO-facing tech media CIO.com quoted consulting firm strategist Mahapatra's reminder in reporting: "The most structural problem in this model is who bears the Forward Deployed cost — this is the question CIOs should ask but mostly haven't." Gartner analyst Alex Coqueiro predicts 70% of enterprises will abandon such solutions by 2028 due to supplier costs and skill hollowing. This reminds us: FDE model's revenue design hides a long-term balance — the value you create must continuously exceed the cost and dependence your presence brings. Earning money from "creating value," business lasts long; earning money from "customers can't leave you," will eventually be liquidated by customers.

### 6.6 Turning Punishment into Reward: Pricing Psychology of Usage and Expansion

Good mechanism design can turn punishment into reward. In FDE business models, this wisdom applies to a subtle scenario: what happens when customer usage exceeds expectations.

The crude approach is "punitive overage": after contract usage is exhausted, excess is charged at punitive high prices, or the system directly rate-limits and slows down. This was common in early cloud computing, with disastrous results — customers actively suppressed usage to avoid overage, usage rate declined, value shrunk, both sides lost at renewal. What you punish is precisely what you want most: deep usage.

The "turn punishment into reward" design approach redefines "overage" as "badge of growth." Three specific techniques.

**Technique 1: Tiered pricing, cheaper the more you use.** Higher usage, lower unit price — customers receiving overage get not a penalty ticket, but a discount. This is same as telecom's tiered data pricing, but must be expressed clearly in contracts: customers don't see "using more costs more" but "using more lowers unit price, we're better off." Same bill, different narrative, relationship direction differs.

**Technique 2: Overage warning + proactive upgrade.** When the system detects customers approaching overage, don't quietly charge, but proactively visit: "your usage is growing fast, at this trend, upgrading one tier saves 15%." Turn billing events into consultative sales opportunities — customers feel cared for, not calculated. This move also has a hidden benefit: it forces your team to continuously watch customer usage health scores, naturally converging with Chapter 5's health score system.

**Technique 3: Give customers credit for "saved" money.** Usage optimization (model tiering, caching, batch processing) reduced costs, so proactively calculate this account for customers: "this quarter through architecture optimization, we saved you about X." In customer finance leads' eyes, helping me save money and waiting for my overage are two completely different types of vendors — vendors who proactively help customers save money, at renewal harvest trust premium far exceeding that fee.

Pricing psychology's foundation is a plain truth: pricing structure tells customers "what kind of relationship we are" daily. Punitive structure says "we're watching you," reward structure says "we grow together with you."

### 6.7 Building a Value Measurement System to Punch Above Your Weight

There's another infrastructure project that can't be bypassed: building a value measurement system running through all customer deliveries — turning "how much value we created for customers" from impression into data, from data into assets.

This system gathers the scattered components from earlier: "economic verification" is its input (value assumptions at project initiation), evaluation system is its micro-foundation (quality data), health score is its operations interface (customer relationship data), pricing and expansion is its commercial exit (revenue data). Put together, it can help you do four things.

**To customers, it's the evidence library for renewal and expansion:** Every quarterly review, every renewal negotiation, every upgrade suggestion, behind it are value reports output by this system — person-hours saved, error rate decline, processing volume increase, corresponding converted financial figures. Chapter 5 said value needs continuous re-proving; this system is the "proof" assembly line; renewal negotiations with data in hand, compared to renewal negotiations by gut, deal closure rate is a notch higher.

**To the company, it's a delivery quality diagnostic:** Aggregating value data across customers, you can answer questions vital to the model's survival — which scenario type has the highest value density (where should sales firepower be directed)? Which customer type has the highest delivery cost (should pricing or approach be adjusted)? Which deployments are creating value vs. spinning wheels (should resources be reallocated)? Without this system, your answers to these are all guesses.

**To product, it's a feedback intelligence amplifier:** Value data combined with usage data is the hardest basis for product decisions — which feature has the highest value output (increase investment), which feature has no users (decisively cut), which scenario is repeatedly customized (platformization signal). This connects to Chapter 7's theme: value measurement system is essentially the "field to product" feedback pipeline's dashboard.

**The fourth thing is to the market.** A potential customer first remembers you often not by meeting your sales, but by encountering a number — "chemical usage reduced by up to 70%," "investigation time from hours to minutes." These numbers that make the entire industry remember you all come from value measurement system's accumulation. Case marketing's most effective isn't telling stories, it's showing data; and data doesn't appear from thin air at the negotiation table — it must start being collected on delivery's first day.

Building this system, three practical suggestions. First, collect baseline from day one — without pre-transformation data, there's no post-transformation value proof, and baseline only exists at project launch moment, miss it and it's gone forever. Second, metrics must be co-built with customers — metrics they don't recognize have no negotiation效力 no matter how brilliantly calculated; the moment agreed at the project initiation meeting, metrics become your common language. Third, restrain metric count — three to five core metrics per customer suffices; too many metrics equals no metrics.

The revenue chapter ends here, landing on only one point: FDE model's revenue, in the final analysis, is the result of value creation.

Next chapter is the book's "last mile": how to make all this not depend on heroic individuals, but precipitate into replicable organizational capability — scaling replication.

---

## Chapter 7: Scaling Replication

> "If you don't convert field learning into product assets, all you get is a pile of custom projects."
> — Barry, former Palantir Forward Deployed Engineer

### 7.1 Using Replicability to Leverage Delivery

Internet growth's most ideal state is one user bringing more users — growth engine shifting from purchased to endogenous. FDE must answer the same question: after completing each customer, the next customer should be easier — not by adding people, but by saving last time's experience.

This proposition is the book's "last mile," because it's the last line of defense between the FDE model and the consulting/outsourcing industry. Remove the scaling link from the approaches described earlier, what's the outcome? An elite team that can fight hard battles, taking one customer, delivering one customer, earning money covering costs, then taking the next — revenue growth and head growth completely linear. Congratulations, you've reinvented the consulting company.

Barry put this dividing line most fiercely in his memoir: "If you don't convert field learning into product assets, all you get is a pile of custom projects." McGrew's formulation is from another angle: the sign the FDE model works is "each subsequent customer's customization volume decreases" — if your customization work doesn't decrease with customer count, you're not doing FDE, you're doing per-person-day outsourcing.

Replicability's lever has three levels, each harder than the last, and each more valuable.

- **Level 1 lever: knowledge replication (playbooks).** Write "how to do it" into documents — playbook templates, checklists, training materials. It turns reliance on personal experience into reliance on organizational memory: new person onboarding cycle compresses from one year to three months. This is the most basic lever; most teams stop here.

- **Level 2 lever: component replication (tools and code).** Turn "what's been done" into "what can be directly used" — integration connectors, evaluation frameworks, deployment templates, industry data models. The next team's starting point is no longer zero but the previous project's shoulders. The automation assets from section 4.7 belong to this level.

- **Level 3 lever: product replication (platform capability).** Abstract "repeatedly appearing customization" into platform standard capabilities — from then on this requirement needs no engineer on-site at all. Palantir's ontology (the semantic layer letting models work on enterprise data), Decagon's Agent Operating Procedures (AOP), Sierra's agent platform, are all Level 3 lever products. This level lever changes the entire business's cost structure: the first two levels reduce delivery cost; the third level eliminates delivery cost.

And these three levels' progression is McGrew's "gravel roads and highways" complete version: FDE repairs gravel roads (solving the immediate problem), component teams lay gravel roadbeds (making the next vehicle's path smoother), platform teams pour highways (from then on everyone can pass).

### 7.2 Bad News Travels Far — Retrospective Propagation of Failed Deployments

Turning incidents into assets is an organization's scarce capability. FDE organizations' attitude toward failure determines whether they can possess replication capability: failure is replication's raw material; organizations that cover up failure are burying gold mines as garbage.

First make one thing clear: failure in the FDE model isn't an accident, it's inevitable. Barry's recollection is merciless: "Failures are plentiful — plenty of time, money, and travel expenses, burned spectacularly." Palantir simply wrote accepting failure into its system: pilots are played like venture capital, most will die, and after death must retrospect. Barry specifically reminds: for those projects that crashed, teams that worked in vain, engineers burned out, also say thank you — lessons were bought with their money. This is hardest to learn, because engineers' nature is to celebrate success and hide failure.

Turning failure into organizational assets requires three mechanisms.

**First, retrospective decriminalization:** The only rule in retrospective meetings is addressing issues not people. Once retrospectives are tied to performance, people start embellishing failure — and embellished failure has zero teaching value. Decriminalization isn't not pursuing responsibility, but redefining "responsibility" as "whether lessons were honestly and completely extracted." An honestly retrosped failed project lead's contribution to the organization may exceed one who succeeded by luck.

**Second, lesson structuring:** Retrospective output can't be "be careful next time" type sighs, must be searchable, executable knowledge — what are this customer type's high-risk signals? Which integration assumption was overturned? Which evaluation metric was designed wrong?

Answers to these questions should enter the playbook's "minefield" chapter, enter new project due diligence checklists, letting the next team's entry due diligence automatically carry historical lessons. Failed lessons only enter process will they be truly used by the next team.

**Third mechanism is most counterintappropriate: moderate external propagation of failure** — desensitize failure lessons then share externally. Section 3.5 covered that Barry's "self-exposing" article became Palantir model's best evangelism. That article had no success studies, all about plenty of burned time, money, and travel expenses, project after project crashing; precisely this writing made readers instantly recognize someone who came from the trenches — enterprise customers have heard too many booth speeches, they can tell what's rhetoric and what's truth. A team daring to publicly dissect failure sends the signal "we've already paid tuition for this industry's detours" — this is exactly what enterprise customers most want to hear.

With three mechanisms covered, walk through a complete failed autopsy. The script below, all components come from real cases earlier in this book, assembled in this industry's common death pattern.

A manufacturing enterprise's AI project died in month 9. Month 1, initiation was sick: group mandate to do AI, IT department leading, no business department signatory — section 2.3's "no-man's land" signal, the vendor saw it, pretended not to, because contract value was tempting. Months 2-4, validation period ran beautiful metrics on sample data — customer's security review wouldn't release real data, "look but don't touch," the second high-risk signal also lit, the project manager chose to build first and say more later. Month 5, demo meeting great success, acceptance passed. Month 6 onward, real data connected, model started giving self-consistent but wrong answers against three-year-old coding rules; the business department that already had no one claiming this project now even less willing to clean up. Months 7-8, usage rate declining, at meetings people started asking "is this thing really worth it." Month 9, budget season, contract uprooted entirely — no incident, no dispute, just no one spoke for it.

This type of project's retrospective minutes, the cause of death column usually reads "customer organization immature." This is embellished failure. Honestly retrospect per section 2.3's checklist: three high-risk signals lit two, each visible before signing. The real lesson is only one sentence: this project's death sentence was decided in month 1, the following eight months were just process. Autopsy to this depth, next time's due diligence checklist, "business owner signatory" and "real data in place" will become hard thresholds from suggestions.

### 7.3 Riding the Wave: Standing on the Industry's Wind

Borrowing external events' attention for yourself is classic marketing. FDE track's teams are standing on an epic wind, and the wind's window won't stay open forever.

2025-2026's industry wind formed from several air currents converging: 1) *The GenAI Divide* report made "95% failure rate" every CIO's heart disease — customers' heart disease is your opportunity; 2) OpenAI forming Deployment Company, Anthropic reported forming comparable joint venture, both news same day, pushing "deployment" onto financial headlines — giants' market-education money, entire industry benefits; 3) FDE position's 729% annual hiring growth made this role a regular in tech media — even "should we hire FDE" became a corporate anxiety. These three air currents together created a rare situation: customers actively looking for you, discussing what you want to sell.

**First layer of riding the wave is "defining the agenda."** The wind's attention is public resource; whoever's content defines the agenda harvests attention. VC firm a16z set the tone for the entire track with an industry essay; communities like OpenFDE, while aggregating practitioners, also aggregate definition power. For specific companies, the best way to grab agenda definition power is making your bottom-of-the-box stuff public: playbooks, failure retrospectives, value data — exclusive first-hand knowledge is agenda definition power's only currency.

**Second layer is "binding industry agenda."** Enterprise AI procurement's biggest driver is upgrading from "efficiency" to "survival" — CEOs being pressed at board meetings "what's our AI strategy," this anxiety transmits into budget. Translate your solution into "board language": not "we can help you optimize customer service processes" but "we can let you present a quantifiable AI report card at the next board meeting." Same delivery, different agenda level anchored, different budget pool reached.

**Third layer is "building assets during the wind, not consuming the wind."** The wind will stop. Discussion stirred by the report will cool, media buzzwords will pass.

So the wind period's most precious isn't signing more deals, but converting the wind's attention into long-term assets: lighthouse cases, industry methodology's discourse power, replicable delivery systems. When the wind stops, teams with cases, methodology, and delivery systems in hand stand firm.

### 7.4 Building Cross-Customer Propagation Loops

Propagation not through advertising but through word-of-mouth, in the FDE industry mainly happens through three circles.

**Circle 1: practitioner community.** FDE is a forming professional community — in 2025 it was still scattered inside companies, by 2026 it already had dedicated communities like OpenFDE, dedicated salary reports, dedicated interview guides. Professional community's formation is a godsend for first-movers: contributing content to the community (methodology, tools, data), your name binds with this emerging profession. Concept propagation paths have always been this way: pioneering evangelists eventually became the concept's synonym.

**Circle 2: customers' industry communities.** Every industry has its own small circles — bankers' forums, law firm partners' annual meetings, hospital executives' summits. Section 3.3's trust dividend mainly flows in these closed circles.

Entry ticket to these circles isn't advertising but invited-speaking customer supporters — your job is making him have something worth telling, told well. Ten minutes of sharing by the customer at his industry summit beats your hundred-day booth at an industry expo.

**Circle 3: ecosystem partner network.** Section 3.7 covered ecosystem bundling's customer acquisition value; here emphasizing its propagation attribute: cloud vendors' solution architects, consulting firms' consultants, integrators' project managers, these people flow across different customer sites daily — the "reliable team" list in their mouths spreads fastest and most accurately. Managing this circle's essential is making them "win": let ecosystem partners gain performance, cases, and reputation in cooperation with you. People who help others succeed are remembered by the entire network.

Ecosystem bundling in 2026 also grew deeper forms: AI companies embedding Forward Deployed teams directly into partners' bodies. Coding agent company Cognition (Devin's developer) and global IT services giant Cognizant's cooperation is the model — an embedded Forward Deployed Engineer team stationed in the other, responsible for project screening, engineer mentoring, and effectiveness measurement, leveraging Cognizant's decades of customer relationships to scale its product into healthcare, financial, and insurance large enterprises. Databricks when reorganizing professional services entirely into Forward Deployed teams, similarly listed its global network of hundreds of partners as one of four scaling elements. Reaching this point, what partner networks propagate is no longer just word-of-mouth, but people you station in the other's office.

Three circles combined's flywheel (self-reinforcing positive loop) is: delivery creates stories, stories propagate in circles, propagation brings new opportunities, new opportunities create new stories. This flywheel's difference from traditional marketing is its fuel is all "delivered value" — word-of-mouth propagation's essence is making every past effort make future acquisition easier.

### 7.5 Product-Embedded Fission Factors

Good products propagate themselves — a line in an email signature "from so-and-so's mailbox" is the earliest self-propagation design. FDE-delivered systems can also pre-bury "built-in diffusion mechanisms," making the system itself a salesperson for expansion.

**Factor 1: Visibility design.** System outputs naturally get circulated — weekly reports, analysis results, approval flows. Make every output carry "origin": "generated by so-and-so system" in report footers, handling entry links in anomaly alerts.

When a beautiful analysis report gets forwarded to the neighboring department director, viewers naturally ask "what's this made with." Visibility design's essence is making system's value self-exhibit in daily workflows, not relying on dedicated reporting.

**Factor 2: Collaborative admission.** Design features requiring cross-role collaboration: investigator-annotated cases need supervisor review, analyst reports need business-side confirmation — every collaborative action naturally introduces the system to a new user. Collaboration-brought new users aren't "promoted to," they're "brought by the work itself" — acceptance completely different.

**Factor 3: Self-service exploration layer.** Beyond core delivery, leave a low-risk practice area (sandbox): customer employees can try "have AI do an analysis for me" themselves. Practices grown in the sandbox are often the most vital expansion leads — scenarios an employee in some department discovers by themselves have more roots than scenarios sales pushes ten times. Let all staff do discovery for you, while the FDE team focuses on hard battles.

Two 2026 new products made this factor explicit. Sierra in March launched "Ghostwriter": customers upload their own standard operating procedures, historical conversation records, even a whiteboard photo, or describe a goal in plain language, the system automatically generates a production-ready agent, covering voice, conversational, email three channels, thirty-plus languages — customer business personnel for the first time can "self-build agents," Forward Deployed teams shift from "doing every one personally" to "acceptance and backstop." Decagon's Agent Operating Procedures earlier walked this path: customer service supervisors write processes in natural language ("returns over 30 days, first check membership level, process if policy-compliant"), without waiting for engineer scheduling — reportedly, Chime's resolution rate reached 70%, Duolingo's problem deflection rate 80%, fitness platform ClassPass's customer service cost down 95%. When customers start building themselves, your role shifts from construction team to design institute.

**Factor 4: Cross-boundary value evidence.** Auto-generate "quarterly value reports" each quarter, let them naturally flow to customer executives. This report is both Chapter 5's renewal engineering and vertical expansion's knocking brick — every number executives see is planting seeds for "where else is this system worth using."

All-hands rollout itself is also an engineering project, its capacity bottleneck equally needs unlocking. Booking.com is the sample: rolling out enterprise search platform to 14,000 employees, the company's first company-wide adopted AI platform; supporting this rollout's training and promotional materials also sped up — single promotional video production cycle compressed to a quarter of original. System delivery's value turned around to become system's own rollout capacity.

Built-in factors' common principle is: wanting others to propagate for you, first let them actually use value out. Any design propagating for propagation's sake is recognized as "vendor's little trick" and resented in enterprise scenarios. Enterprise markets have no viral propagation, only "word-of-mouth chain reactions" — slow, but every step solid.

### 7.6 Grasping Organizational Politics in Scaling

On the scaling path, what blocks you is usually people's territory — technology is actually easy to solve.

When a system expands from one department to ten, you're actually rewriting the organization's internal power map: information monopolies broken (data one department exclusively had, now visible company-wide), approval authority compressed (things AI answers in seconds no longer need three days of layered signatures), professional barriers leveled (senior employees' "unique experience" encoded into the system). Every change is making silent enemies.

Responding to organizational politics, FDE veterans distilled three mental methods.

- **Mental method 1: Expansion must bring "locals."** Each time entering a new department, first find that department's "local boss" — the most prestigious senior employee, invite him into the adaptation process: "this scenario, what's different about your department?" His answer makes the solution more accurate, his participation makes the solution smooth on his turf. People won't oppose things they participated in building — this is one of organizational behavior's few reliable levers.

Harvey's expansion in elite law firms is a classic teaching case for reading organizational politics. Three groups coexist in firms: partners — the ones who pay, but don't personally work; associates — the ones who work, but don't sign; knowledge management lawyers — neither, yet see both sides' blind spots. Generic survey research compresses three groups into the same set of dropdown options, getting a pile of distorted averages; Harvey's Forward Deployed team designed interviews and demos separately for three groups: show partners "how much money this deal makes," show associates "three fewer overtime hours this week," show knowledge management lawyers "the firm's tacit experience finally has somewhere to precipitate." One deployment must simultaneously make three groups feel they're beneficiaries — missing any group, the system gets quietly shelved at the corresponding link.

- **Mental method 2: Make every expansion step have "beneficiaries."** Before expansion, calculate clearly what each related department gets: departments penetrated of data barriers get globally visible analysis capability; departments compressed of approval authority get focus power on exceptions (AI handles routine, humans focus on hard cases). Before expansion, think clearly what each related department gets, and say it clearly — expansion where you can't think this through, in the other party's eyes is grabbing territory.

- **Mental method 3: Always leave dignity for the "old order."** Processes replaced by the system were once designed by some capable person; encoded experience was once some expert's life work. In rollout messaging, respect for the old order is respect for the old order's maintainers: "this process supported the company for the past ten years, now we're going to amplify its ten years' experience a hundredfold." People who give the old order enough dignity, when the new system goes live will have half the hidden resistance.

Three mental methods all speak to the customer's organization. There's another layer of politics on the scaling path, hidden inside your own company: sales and delivery's authority and responsibility.

This layer's root is incentive misalignment: sales' bonus hangs on contract value, delivery's reputation hangs on results — the impulse to sign deals and the discipline of delivery naturally fight. Handling it relies on three written tables.

- **Division of labor table:** Sales is responsible for "sign or not," delivery for "can it be done"; custom requirement veto power belongs to delivery, but veto must come with alternatives — if only allowed to say no without giving paths, delivery becomes "the one blocking business" in sales' eyes.
- **Money-sharing table:** First-deal commission belongs to sales, renewal and expansion bonus must be shared with delivery — section 5.1 calculated, renewal cost approaches zero, value entirely from delivery quality; if renewal bonus all goes to sales, the company is using its wallet to tell everyone "signing is more important than doing well."
- **Blame table:** Delivery incidents are assigned by "who made the promise" — incidents caused by sales over-promising go into sales' assessment; holes delivery dug itself go on delivery's head.

Three tables need not be complex, but must be written; unwritten authority and responsibility will concentrate-explode in the year with most orders and biggest team.

### 7.7 Using Playbooks to Precipitate Replication Efficiency

Level 1 lever's playbook engineering details are most easily underestimated — most teams' playbooks, the day written is their highest-read day.

- **Playbook's first attribute: grow in process, not lie in knowledge base.** A playbook only searchable in a document system equals nonexistent. Effective approach is embedding it in workflow: new project's due diligence phase, system automatically pops up that customer type's due diligence checklist; deployment phase, checklists are hard gates in the task system; retrospective phase, playbook update is retrospective's required output. Knowledge not embedded in process is just archaeology. This path's end is process starting to execute the playbook itself: Ramp's engineering team has AI assistants first do multi-round clarification with customer managers, then draft requirements documents, according to its disclosure, saving about 20% of requirements definition time.

- **Playbook's second attribute: organized by "scenario" not "feature."** Failed playbooks are written by company organizational structure ("delivery process," "technical specs"), while successful playbooks are written by customer scenarios ("financial AML scenario playbook," "manufacturing scheduling scenario playbook," "law firm knowledge base scenario playbook"). Each scenario playbook contains a fixed seven-piece set: 1. typical pain points and fit verification points; 2. due diligence checklist (high-risk signals specific to this scenario); 3. known minefields for data and integration; 4. evaluation and acceptance metric templates; 5. change management role map; 6. pricing and expansion reference structure; 7. historical retrospective lesson library. Harvey's law firm scenario playbook being replicable to PwC, Clyde & Co relies on writing first customer (Linklaters)'s experience into inheritable scenario assets.

- **Playbook's third attribute: it must be "alive" — has owner, has version, has depreciation.** Each scenario playbook designates an owner (usually the most senior delivery team), every project end forces review and update, every half year does an overall overhaul — delete outdated, merge duplicates. Playbooks without owners, a year later new people following them will step into long-fixed pits — worse than no playbook.

Playbook's relationship with Level 2 lever (component library) and Level 3 lever (platform) is: playbook manages judgment (what to do in what situation), component library manages craft (tools directly usable), platform manages capability (functions not needing people on-site). With all three complete, a newly formed FDE squad can reach 80% of an old team's combat power in two weeks — this is replication's true meaning.

These three all solve "thing" replication. The FDE model's scarcest asset is people who go to the field — and such people barely exist in the hiring market — Vinoo Ganesh, who designed Palantir's rotational training program, put it bluntly: "You can't build a real FDE organization through hiring, only through cultivation." After all, traditional engineering positions deliberately separate engineers from customers' reality; field judgment can't grow in offices.

"Cultivation" doesn't mean not selecting seedlings. Palantir interview's signature segment is throwing candidates a deliberately vague real problem — like "design a system routing city emergency calls to the correct responder" — letting them decompose on the spot, almost no code; by candidates' common feedback, the most common mistake is preparing for this interview as a pure software engineer interview. What it screens is people who can first decompose structure facing a fog.

Cultivation's method is rotation: sending engineers in batches into real customer deployments, over 250 engineers through this path to the field, alumni now scattered in OpenAI, xAI, Anduril and other companies. This training program's most critical improvement is aligning rotation positions with products engineers will build after returning — first be a user, then be a builder. For companies without conditions for rotation, he left a six-month self-cultivation checklist:

1. First two weeks shadow customer calls, recording not feature requests but "how this person's day goes";
2. Second month end-to-end own one customer incident;
3. Third month go on-site, find a small pain point fixable within a day, fix it that week;
4. Final months, maintain a weekly "what I learned from customers" update.

This checklist is also a playbook — a playbook for cultivating people.

"Cultivation's" starting point is "hiring" — where seedlings come from, first have a map. Practitioner experience's three highest-conversion pools: 1) big tech's solution architects — understand technology, seen customers, lack experience being responsible for results; 2) consulting firms' technical consultants — understand business, can speak, lack hands-on; 3) customer-side star users — understand pain points best, poaching them is "Echo" natural candidate. Be cautious with pure backend R&D instead — not ability issue, they're too far from customers' reality, field judgment must grow from zero.

The last sieve before hiring is section 1.7's "problem decomposition" interview. Same question — "A bank's compliance team manually checks 30,000 transaction alerts daily, 90% are false alarms, what do you do" — good and bad answers' gap looks like this. Dangerous answers go straight to technology: "build a classification model." Three sentences expose him: he didn't ask how alerts are generated, who bears misjudgment costs, what compliance officers trust. Good answers start with questions: who defined false alarm rules? Who's responsible for missing a real alert? Which step of current process is slowest? Then give minimum incision — "don't do judgment first, only pre-sort, put most-likely-false-alarms last, humans check high-risk first"; finally proactively state trade-offs — "false positives still there, but manpower halved, and every suggestion traceable."

### 7.8 Product Planning and Polishing

Level 3 lever's culminating work is crystallizing field experience into product.

First look at the most spectacular success case: Palantir's Foundry. Today this platform generating billions in annual revenue, supporting company's hundreds of billions market cap, its core components were born at customer sites in Zurich, Houston, São Paulo, Toulouse, Baku — Forward Deployed Engineers in various places each building tools to solve local solutions, through years of natural selection and platform incorporation, finally growing into unified product. Barry recalled this process as "completely bottom-up": 2014's company product strategy literally was "strong opinions, loosely held," letting the field bloom freely, survivors collected into core.

This process isn't pastoral, it has rigorous internal logic, extractable as "productization four questions."

- **Question 1:** Is this field solution "individual" or "common"? Judgment criterion: has the same type of problem independently appeared at three or more customers? Three customers' same pain point is product signal, while one customer's special requirement may just be a quirk. Palantir's rule of thumb is letting "multiple Forward Deploying teams reinventing wheels" naturally expose commonality — when three teams each built similar things, the platform team knows: collection time has come.

- **Question 2:** Is generalization's cost less than benefit? McGrew reminded: field code is "fast and rough," generalizing it "often costs more than writing the first version." Productization decisions must calculate this math: generalization investment vs. future several customers' saved customization cost. If math doesn't work, stay at component layer, don't force platformization — every capability in the platform is a lifetime maintenance commitment.

- **Question 3:** Can it be used by "people who can't code"? Field tool's users are engineers; platform capability's users are everyone. Productization's hardest step often isn't technology but interaction: turning engineers' scripts into business personnel can configure features. Decagon's Agent Operating Procedures (letting operations define processes in natural language) is this step's model — once the abstraction layer is chosen right, user population can expand a hundredfold.

- **Question 4:** After collection, is there still room for the field? This is the most subtle balance: platform collecting too much, field teams degrade into configurers, FDE model's soul (field creativity) dies; collecting too little, scaling lever can't rise. Palantir's solution is maintaining "radical authorization of field over base" — high-level only sets goals, approach belongs to the field. Platform making common things easy, field teams then have spare capacity to chew hard bones originally impossible.

Four questions answered, platform built, the final discipline just appears: the order of expanding openness. Latin American e-commerce giant Mercado Libre made it a textbook. This company's internal platform opened self-service to 17,000 developers: any team assembles AI applications with nodes and skills, built-in testing, but never sees source code — cognitive load pressed to minimum, safe bets all placed on platform guardrail quality.

Expanding openness's pace is nearly conservative: first use AI on low-error-cost tasks — product cataloging, translation, review summarization — cataloging alone, in two years processable product volume increased a hundredfold; after accumulating enough data and organizational trust with low-risk tasks, only then let platform touch money-involving customer service dispute mediation, and first open about 10% at a single major site, humans retaining copilot and escalation channels. Its COO said bluntly: cataloging and summarization "fun and useful, but not transformative," real transformation is letting systems autonomously handle complex, high-risk work. But such systems must first be fed by years of low-risk tasks.

Skeptics of this flywheel, the most powerful rebuttal is always gross margin (proportion of revenue remaining after direct costs): sending people to the field, how can gross margin be high? History has answered three times. ServiceNow at IPO gross margin 63.2%, criticized as "too much like a services company" — ten years later 79%, market cap near $200 billion; Workday at IPO 54.1% — now 76%; Palantir at IPO 79%, 2025 reached 82%, more beautiful than most "pure software" companies.

Insight Partners' summary hits the nail on the head: these companies that heavily invested in implementation and services during platform transition were precisely the companies that persisted when everyone ran in the opposite direction. The secret is gross margin can climb year by year — as platform precipitation thickens, customers can do more implementation work themselves (Bootcamp mode lets lots of integration work be done by customer side), service cost continuously amortized — openings all look bad, but run forward gets lighter.

Negative specimens are equally ready. Bessemer Venture Partners dissected India's IT services industry: industry leader TCS's revenue doubled in the past decade, employee count nearly doubled too, but per-capita revenue stayed at about $49K — growth still entirely relies on piling people. Services companies that don't complete platform transition, ten years later are just a bigger services company — "reinventing consulting companies" at industry scale.

Beyond gross margin, there's a more intuitive ruler: per-capita revenue. Put three together — TCS still that $49K; Accenture FY2025 about $89K ($69.7B revenue, 779K employees); Palantir 2025 about $1M ($4.48B revenue, 4,429 employees). From outsourcing to consulting to FDE, per-capita output differs by an order of magnitude.

On the startup side, multiples are more direct: Harvey's about $190M ARR, supporting $11B valuation, about 58x — the market is obviously pricing it as software, not services. Whether this pricing is right will be known in five years, but at least it shows: capital markets are willing to pay software multiples for delivery models whose "per-capita output aligns with software." This set of comparisons is also the hardest answer to "is FDE consulting in disguise": isn't, don't look at titles, look at which direction per-capita output and gross margin climb.

Pull the camera from giants back to ground, calculate a 10-person squad's rough math — this book's deduction, every assumption laid out, you can swap in your own numbers and recalculate. Cost side: per section 5.3's calculated standard, US market one fully-loaded FDE's annual cost approaches $500K, 10 people is $5M; Chinese market per Chapter 1's salary levels converted, cost side several million to over ten million RMB. Capacity side: section 3.8 calculated, one squad simultaneously delivers at most two projects at high quality, 10 people split into three squads, over a year, approximately deeply serve 10-15 customers.

Revenue side: deep service projects at $100K-$300K per contract, 10-15 customers a year, revenue $1M-$4.5M. Put against US standard $5M cost, first two years mostly can't cover; swapped to Chinese standard cost, barely breaks even. This is FDE business's first two years' normal: pure labor period, gross margin 20-40%, possibly negative.

Profit-turning levers are only three: reuse rate — components and platform, pressing single-project hours down; pricing tier — lifting unit price up; renewal rate — making second year's revenue not need first year's cost. Each lever up ten percentage points, gross margin roughly climbs from 30% to 60% — the ServiceNow group's ten years earlier climbed exactly these three levers. McGrew's "each subsequent customer's customization volume decreases" speaks precisely of this machine's tachometer: customization volume decreasing speed is the speed a labor business becomes a software business.

Finally, tell a story about "betting on the right direction." In late 2022 ChatGPT burst onto the scene, everyone was guessing what Palantir would do. Sankar made a bet later repeatedly cited: LLMs will rapidly commoditize, value will aggregate to both ends — one end is compute chips, the other end is ontology. He pressed the company's majority of engineers onto AI platform AIP. Result: Palantir's stock rose from single digits when he took over as CTO to around $200; US commercial revenue consecutive quarters of triple-digit growth. This bet's logic is exactly the book's opening main line: the stronger and cheaper models get, the more valuable the "connecting models to reality" engineering layer becomes.

Productization four questions' endpoint is the entire FDE business model's convergence: field detects the real world for you, platform amplifies what's detected, finally precipitates into product, continuously regenerating. This is a mutually feeding cycle: field makes platform more solid, solid platform lets field dare take on more distant jobs. Once this flywheel turns, you're no longer a "send people to do work" company, but a "continuously transform the world's complexity into software assets" company. This kind of company's resume, the gross margin math earlier already wrote it for them.

Next chapter is the complete case study collection: returning to these methodology's original field sites.

---

## Chapter 8: Complete Case Studies

The previous seven chapters' methodology was all distilled from real practice sites; here we reconstruct them completely: five groups of cases, from the mode's inventor to its newest inheritors, from Silicon Valley to China.

### 8.1 Palantir: Twenty Years to Forge a "Dumb Method" into a Moat

#### Founding: Building Software for "Users You Can't Ask"

Silicon Valley in 2003 was still lying in the internet bubble's ruins. Peter Thiel pulled together a group of Stanford-educated young people to do something that sounded crazy: build data analysis software for US intelligence agencies. The company's name came from Lord of the Rings' seeing stone Palantir — the stone that can glimpse distant places.

This thing's hardest part, from day one, was users. Bob McGrew's widely circulated recollection years later makes the dilemma clearest: "One challenge of building software for spies is: I don't know any spies. You probably don't either. Even if you happen to find a spy and ask them 'how do you actually work day to day,' they usually won't tell you."

The software industry's entire methodology — user interviews, surveys, usability testing — collectively failed before this user group. Co-founder Stephen Cohen's response was adorably crude: build a demo, show it to intelligence people, ask what they think. The answer was merciless: "This is terrible, it has nothing to do with what we do." Cohen didn't retreat, but asked: "So what would you want it to be different?" Then wrote down every item, went back, revised, brought it back. Cycle repeated.

This cycle is FDE's gene fragment, containing two intuitions later proven worth a thousand gold: customers in complex domains don't know what they want until they see something usable; the fastest path to knowing "what they want" is putting the people building things next to the people using them.

#### Formation: From Emergency Measure to Organizational Strategy

Early Palantir followed "one customer, one customization" forward, quickly hitting the problem every enterprise software company hits: the second customer's needs were "subtly but critically different" from the first.

The standard solution is extracting commonalities, building a universal product, saying no to differences. But Palantir's customers didn't accept "no" — they were the CIA, the US military on the battlefield. The one who truly led the company out of this deadlock was early employee Shyam Sankar (later company President and CTO). His solution was considered heresy at the time: don't build two products, nor one rigid product, but build a highly customizable platform, station engineers at customer sites, complete the last mile.

Sankar's most critical move was heresy on the ledger. In software industry's financial language, "customizing for a single customer" is called service cost — the enemy of profit margins, to be minimized. Sankar redefined it as "product discovery" — on-site customization isn't spending, it's collecting intelligence for the product's next evolution. One noun's change altered a company's capital allocation logic: what others saw as cost center became Palantir's R&D center.

Organizational form solidified accordingly. Forward Deployed Engineers (internal codename "Delta") embedded in customers, "one customer, mobilizing multiple capabilities"; Deployment Strategists (codename "Echo") responsible for understanding customer mission and organization; platform engineers at the rear, "one capability, serving multiple customers." By around 2016, Palantir's Forward Deployed Engineers outnumbered platform engineers — a software company with the majority of its forces at the "front line."

#### Trials: Battlefields, Hurricanes, and Oil Fields

FDE model's value was repeatedly proven at extreme sites.

Iraq and Afghanistan battlefields, IEDs were the patrol's number one killer. Stationed Palantir engineers discovered soldiers had zero interest in exquisite intelligence charts — they just wanted to "mark this road suspicious on a map." The engineer cobbled together a crude map tool on the spot: soldiers tap once, risk zones visible to the whole team. This tool directly reduced casualties, later precipitating into platform standard features. This tool can't be pieced together in headquarters conference rooms. It can only appear in the moment engineer and soldier look at the same stretch of road together.

And this approach's prototype site predates the map tool. Around 2007, Sankar brought a small team into the US military's Joint IED Defeat Organization (JIEDDO)'s classified information room, co-located for two weeks. Even speakerphones are forbidden in classified rooms; he strapped a phone to his head with a rubber band, freeing both hands to code — one ear listening to analysts' feedback, the other ear listening to Silicon Valley headquarters colleagues. Nineteen hours daily: demo, connect data, collect feedback, revise on the spot.

Two weeks ended, analysts said: this thing is useful. Sankar himself collapsed from exhaustion, called Karp: "This is not sustainable, we're done." Karp's answer later became company culture: make this "unsustainable" thing into a system.

2012 Hurricane Sandy disaster relief site, Palantir's Forward Deployed Engineers pieced scattered rescue data into real-time maps, coordinating rescue resource deployment. Oil drilling platforms, aircraft assembly lines, bank trading floors — engineers took "stationed presence" to unprecedented depth in the software industry. Former Palantir engineer Barry recalled that Foundry platform's core components were born in Zurich, Houston, São Paulo, Toulouse, Baku — a world map, every point a field creation.

Costs were equally real. Barry's record is required reading for understanding this model's negative side: top engineers, global travel, massive wheel-reinvention, free pilots, "many projects had literally negative infinite margins"; 2014's company product strategy literally was "strong opinions, loosely held," chaotic enough to keep stockholding employees awake at night. Palantir could swallow these costs relying on two things: sky-high contract values' capital thickness, and the "pilots as venture capital" mindset — most bets going to zero is fine, but the winning few must win back everything.

Commercialization also died once first. First enterprise-facing product Metropolis was a market flop; second attempt Foundry finally took off. The turning point was Airbus: in the Toulouse factory, an A380 fuel pump failure kept recurring; Airbus's own engineers investigated for a full two years with no clue. Palantir's people came in, connected sensor data to the platform, cracked the case in two weeks — during climb, fuel sloshed away from the pump body. A trivial fix preserved an order reportedly worth tens of billions.

Airbus digital transformation head Marc Fontaine later publicly remarked: "The same problem, we used to need twenty-four months." Airbus became Palantir's most enthusiastic European evangelist, building its entire data platform Skywise on top, connecting tens of thousands of aircraft and over 50,000 users.

This platform approach proved itself again at life-and-death sites. Florida's Tampa General Hospital had co-built a sepsis early warning tool with a vendor, which was classified as a regulated medical device by the FDA and forced to stop. For ordinary customers, the story ends here; Tampa General's choice was to rebuild on Palantir's platform themselves, led by Chief Digital and Innovation Officer Scott Arnold. By mid-2025, this self-built sepsis center had saved 569 lives, sepsis patients' hospital stays shortened by 30%.

#### Explosion: Bootcamp Ignites the Commercial Empire

In 2023, generative AI exploded. All enterprises wanted to "use AI," all enterprises were stuck at the same place: didn't know how. Palantir's answer was compressing its twenty years' stationed methodology into an industrial machine — AIP Bootcamp.

Rules extremely simple: customers bring real data and real problems, Palantir's Forward Deployed Engineers accompany, one to five days to make a deployable AI application prototype, free or nominal charge. Day 0 lock onto an extremely focused core battlefield; Day 1 connect data, build ontology model (modeling customer business objects and relationships into a semantic layer); Days 2-3, engineers and customer technicians write code back-to-back, connecting LLMs into business flows; Days 4-5, executives personally operate the system, decide on the spot.

This machine's conversion efficiency stunned the entire industry: starting from fewer than a hundred pilots in 2022, sessions multiplied year over year, averaging nearly 6 per day at the 2025 peak; enterprise software's 9-12 month sales cycle compressed to weeks; pharmacy chain Walgreens deployed 4,000 stores in eight months via Bootcamp; market research firm J.D. Power, after learning, started running Bootcamps for its own customers — the mode began self-replicating. Post-Bootcamp contract pace is so fast peers barely believe: a large healthcare company, five weeks after attending Bootcamp, signed a five-year, $26M ACV deal; a global bank, one month after pilot first signed $2M, four months later expanded to three-year, $19M ACV.

Financial results exploded accordingly: Q4 2025 US commercial revenue up 137% year-over-year; Rule of 40 reached 127%, Q1 2026 hit 145%; single-quarter bookings $4.26 billion, NRR 139%; market cap once broke through $400 billion. Wall Street analysts who mocked its "people sea tactics" began rewriting research reports overnight.

The biggest single vote of trust came from the US Navy. In December 2025, the Secretary of the Navy and Karp jointly announced the "Ship Operating System" contract: $448 million, first using Foundry and AIP to transform the submarine industrial base — two large shipyards, three naval dockyards, a hundred suppliers. Pilot data covered earlier: scheduling from 160 hours to 10 minutes, material review from weeks to one hour. The Secretary of the Navy specifically stated "this is not a concept, not a pilot, not research" — it skipped PoC and went directly into production, because prior embedded pilots had already proven value. Same year, the US Army also packaged 75 scattered service contracts into a single ten-year $10 billion framework agreement to Palantir. Government trust is twenty years' stationed presence's compound interest.

An engineer named Nabeel Qureshi who was stationed in Toulouse for a full year left a more vivid footnote: four days a week he soaked in the assembly workshop, with manufacturing workers, writing software for the A350 production line — he called it "building an Asana for airplanes" (editor's note: Asana, Silicon Valley's popular project collaboration software). A Silicon Valley engineer, living in a foreign factory for a full year.

#### Methodology Reconstruction

Looking back at the previous seven chapters, the Palantir case has correspondences almost everywhere: the demo loop and "customers don't know what they want" correspond to Chapter 2; lighthouse customers' strategic value corresponds to Chapter 3; free pilots' portfolio investment logic corresponds to Chapter 6; field tools growing bottom-up into platform corresponds to Chapter 7. The bottom-line creed runs through the entire book: complexity cannot be eliminated remotely, so someone must show up.

### 8.2 OpenAI: When the People Who Built ChatGPT Start Moving Bricks in the Field

#### Turning Point: From "Model as Product" to "Deployment as Strategy"

OpenAI's first seven years were a pure technology epic: GPT series racing forward, ChatGPT setting the fastest user growth record in human history. In such a company narrative, "enterprise delivery" sounds like a neighboring industry's business.

The turning point came in 2024. Enterprise market data illustrated something that couldn't be ignored: the "95% failure rate" from *The GenAI Divide* report was playing out; meanwhile, enterprise LLM market's share map was dramatically shifting — Menlo Ventures' industry tracking showed Anthropic climbing to about 32% in enterprise markets, OpenAI falling from early about 50% absolute lead to about 25%. Model capability gap was narrowing, and enterprise customers' voting standard with real money quietly became another question: **"Who can help me actually use this thing?"**

OpenAI's response had two steps. First, 2024 formed the Forward Deployed Engineering team — starting from 2 engineers, Colin Jarvis leading, rapidly expanding to a global network across San Francisco, New York, London, Dublin, Munich, Paris, Zurich, Tokyo, Singapore, Sydney, growing from 2 to 52 people in a year. Job postings unabashedly stated: "embed into customers where model performance is critical, delivery is urgent, ambiguity is the default state," travel up to 50%. European lead Fournier put it more bluntly: "Market demand has exceeded our expectations."

Second, on May 11, 2026, formed "The Deployment Company" — a joint venture controlled by OpenAI, with 19 top-tier capital firms (TPG leading, Advent, Bain Capital, Brookfield co-leading, Goldman Sachs, SoftBank, HPE etc. participating, Bain & Company, Capgemini, McKinsey as founding partners), initial investment exceeding $4 billion, media-disclosed pre-money valuation about $10 billion; simultaneously acquired applied AI consulting firm Tomoro, about 150 deployment engineers merging en masse. COO Brad Lightcap personally took charge.

This new company's structural design deserves business school textbooks because it welded "where customers come from" and "how capital returns" together. The investors are PE giants, and these giants hold hundreds of portfolio companies spanning healthcare, manufacturing, financial, retail, logistics — they are the Deployment Company's ready-made customer pool; in exchange, reportedly OpenAI promised these PE investors a five-year 17.5% annualized preferred return (media report, OpenAI unconfirmed), while itself retaining super voting rights, controlling strategic direction.

Acquired Tomoro was no nobody: this UK applied AI consulting firm's engineers had previously done enterprise landing at Tesco, Virgin Atlantic, game company Supercell. In one day, OpenAI collected all three cards: "engineers, channels, capital."

A company valued at hundreds of billions, holding humanity's strongest models, separately forming a $10 billion company for "sending people to customer sites to work" — this is the heaviest weight in FDE model's history.

#### Field: John Deere's Farmland

OpenAI FDE methodology's best display window is the collaboration with John Deere. This nearly-two-century-old agricultural giant wanted to solve a problem grown from the land: weed control. Traditional practice is whole-field herbicide spraying — high cost, heavy phytotoxicity, large environmental cost. Precision agriculture's ideal is "spray only when seeing weeds," but identification difficulty lies in: every field's weed composition differs, crop growth differs, seasons differ.

OpenAI's Forward Deployed team's approach is this book's Chapters 2 and 4 methodology's complete demonstration: flying to Iowa, following agronomists into fields, understanding precision agronomy's workflows and constraints (including that non-negotiable hard deadline — farming seasons); reviewing hundreds of real field operation cases with experts, encoding "what's a good spraying suggestion" into a custom evaluation system; rapidly iterating model and system under the evaluation system's care. Final result: chemical usage reduced by up to 70%, farmer interaction frequency increased 6 times. Pricing also aligns with value: not per-device flat fee, but subscription by acreage with technology actually enabled — in 2024 alone, this system saved 8 million gallons of herbicide mixture, 2025 coverage exceeded 5 million acres.

Three lessons: first, the hard deadline is farming seasons, not project scheduling — FDE's rhythm must obey customer's business cadence. Second, evaluation system precedes model optimization — first define "good," then pursue "good." Third, the 70% figure isn't post-hoc packaging, it's a target set with experts before work began.

#### Field: BBVA's 120,000 People

Another benchmark is BBVA. Cooperation's starting point wasn't stunning — deploying ChatGPT Enterprise. But FDE model's compound interest lies in: entering from one tool, ultimately transforming the entire organization. Starting from 3,300 accounts, employees spontaneously created over 20,000 custom assistants (GPTs), 83% weekly active usage, average 3 hours saved per week; a year and a half later, deployment expanded to a system covering 25 countries, 120,000 employees, the bank's goal upgrading to "building an AI-native global bank." From "giving a tool" to "co-building an organizational form" — this is Chapter 6's "existing account deep cultivation" extreme form.

#### Methodology Reconstruction

OpenAI case's revelation lies in "model companies' self-awareness": when model capability converges, capability becomes the main battlefield for differentiation; when product form is undefined (no one knows what agents should look like), the field becomes product discovery's only site. Its three-phase work method (co-creation, validation, delivery), its engineering obsession with evaluation systems, and the Deployment Company's capital structure innovation (using PE capital's industrial network as customer channels) are all products of this self-awareness.

### 8.3 Anthropic, Vertical Three, and Platform Vendors: FDE's Four Variations

If Palantir invented the mode and OpenAI pushed it onto headlines, then Anthropic, a batch of vertical AI companies, and data platform vendors show FDE's four variations in different soils.

#### Variation 1: Anthropic — Safety Genes and "Auditability" Differentiation

Anthropic's FDE sits under the Applied AI team, with two noteworthy qualifiers in job postings: first, "safety and reliability" — all deliveries must meet Anthropic's safety standards; second, "defending the company's mission on the front line" — FDE are simultaneously values ambassadors. In 2025, this team expanded fivefold in a year, head Kate De Jong's explanation: "A Fortune 500 bank's needs and an AI-native startup are two completely different species."

Differentiation's direct product is "auditability" becoming a product feature. Cooperation with fintech giant FIS is the benchmark: Anthropic's Forward Deployed Engineers embedded in FIS to co-design financial crime detection agents, AML investigations compressed from hours to minutes, every decision fully replayable and traceable, first deployed at Bank of Montreal and Amalgamated Bank. In strongly regulated industries, every AI decision must be explainable to regulators — can't explain, can't enter — Anthropic made this admission line into a selling point.

"Safety paranoia" becoming enterprise market killer evidence is written in customer evaluations. Cybersecurity company Palo Alto Networks deployed Claude to 2,500 developers, engineering director's evaluation direct: "They care more about security than others — every meeting discusses security impact. As the largest cybersecurity company, this matters to us." Result: feature development speed up 20-30%, junior developers completing integration tasks 70% faster. Pharma giant Novo Nordisk uses it to write clinical research documents: reports that took ten-plus weeks now draft in ten minutes (vendor official case). Ride-hailing platform Lyft connected Claude to customer service, average resolution time down 87%; customer service software company Intercom's agent Fin after switching to Claude, resolution rate from 23% to 51%, deep customization up to 86% — these two deployments' complete process from pilot to all-hands rollout is written in Chapter 4. Meanwhile, it cooperated with consulting giant Accenture to train thirty thousand Claude-certified consultants, enterprise customer count in two years from under a thousand to over 300,000.

Deeper differentiation lies in "knowledge transfer" official commitment: embedding's explicit goal is making FIS "able to independently build and expand its own agents in the future." Writing "teaching the customer" into the contract, short-term looks like weakening one's own irreplaceability, but long-term is the most powerful response to "vendor lock-in" doubts — Gartner analyst Coqueiro predicts 70% of enterprises will abandon such solutions by 2028 due to supplier costs and skill hollowing (media relay, see section 5.1), Anthropic's approach is defusing this time bomb in advance.

In May 2026, Anthropic was reported to be forming an enterprise AI services joint venture with Blackstone and others, reportedly about $1.5 billion, focusing on embedding Claude into mid-sized enterprises' operations — competing head-on with OpenAI's Deployment Company on the same day. Two model giants completing "deployment as strategy" organizationalization on the same day — this matter itself illustrates FDE's coordinates better than any analysis.

#### Variation 2: Sierra and Decagon — Startups' "Delivery as Product"

Sierra (founded 2023 by former Salesforce co-CEO Bret Taylor and former Google VP Clay Bavor, valued at $4.5B at October 2024 funding, reportedly continued climbing since) made the FDE model into the business model itself: customers don't pay for software, they pay for "resolved conversations"; implementation hosted by Sierra's Forward Deployed team, customers only contribute brand voice and operating rules. Effect: Sonos, Casper, WeightWatchers, ADT and other brand customers flocking, publicly reported fastest go-live case four weeks, annual contract threshold about $150K minimum (third-party estimate, see section 6.3). Charging by results makes Sierra's pricing naturally anchored to customer value — Chapter 6's "charging by results" most radical real-world sample.

Sierra's internal naming for this position is also worth noting: not FDE, but "Agent Engineer." Head Natalie Meurer (former Palantir five years, handled law enforcement, defense, and infrastructure customers) explained: the name should describe "the shape of technical work," not just "obsession with customers" — voice agent building requires a special "taste" (what sounds human, what sounds right), a narrower and deeper craft than general FDE. Ticketing platform Vivid Seats' cooperation is her team's brightest combat report: four weeks online, resolution rate up 40%, CSAT up 35% — and conversation data feeding back into product's mechanism, making "ten thousand people asking about the same feature in a month" immediately schedulable.

Decagon (co-founder Ashwin Sreenivas from Palantir, total funding $231M) walked another path: directly productizing delivery experience into Agent Operating Procedures — letting customer operations personnel define multi-step workflows in natural language, AI executing deterministically. Customer list: Notion, Duolingo, Eventbrite, Rippling. Reportedly, Chime's resolution rate reached 70%, Duolingo's problem deflection rate 80%, ClassPass's customer service cost down 95%. Decagon's FDE more plays "the person who teaches customer teams to use this system" — delivery's goal is making customer non-technical personnel have self-service capability, this is Chapter 7's "productization four questions" "can it be used by people who can't code" best practice.

#### Variation 3: Harvey — Breaking Into Places Ordinary Software Can't Enter

The legal industry is enterprise software's "Bermuda": top law firms' strict confidentiality discipline, data not leaving the domain, partners each doing their own thing — self-service SaaS rarely wins here. Harvey (founded 2022, after March 2026 funding round valued at $11B) broke in with the FDE model.

This company's pedigree is special: two founders, one a litigation lawyer from law firm background, one a scientist from DeepMind background; seed round $5 million from OpenAI's startup fund.

Reviewing its approach, almost every step finds correspondence in this book's methodology. First major customer locked onto global elite firm Linklaters (February 2023, 3,500 lawyers, 43 offices), then PwC (4,000+ legal professionals), Clyde & Co, Macfarlane followed. Inside Linklaters, counterpart David Wakeling (Market Innovation lead) became deployment's in-firm axis; rhythm-wise entering from a single business group, driven by partner supporters, horizontal expansion only after six months of real combat. Customer research was the hardest link: partners pay but don't work, associates work but don't pay, knowledge management lawyers see both sides' blind spots — so FDE's interview system must simultaneously penetrate three groups — per Harvey deployment side's retrospective, deployment's hardest part isn't the model, it's the customer research loop. Cycles are also very long: single-firm deployment six to nine months, FDE responsible from document management system's data pipes all the way to partner-by-partner adoption demos.

Effect is vertical AI's rare surge: users exceeded 100,000 lawyers, 1,300 organizations, covering most of the US top 100 law firms; ARR from about $100M in August 2025 to about $190M in January 2026; valuation jumped four times in one year — $3B, $5B, $8B, $11B.

Harvey proved FDE model's boundaries: wherever "confidentiality systems, data not leaving domain, key user autonomy" three mountains coexist, productized delivery has no solution — only people entering can bring the system in. And such markets — law, healthcare, financial, government — happen to be the highest-profit enterprise service markets on Earth.

#### Variation 4: Databricks and Snowflake — Platform Vendors' Embedded Delivery

Variations don't only happen at model companies. Data platform vendors' customers mostly aren't AI-native companies, but traditional industries with mountains of data they don't know how to use — delivery here equally can only be done by engineers embedding in.

First American is a veteran US title insurance company, maintaining over 8 billion public registration document images, a large portion historical scans without even metadata. It needed to classify and extract data fields page by page from about 4 million title insurance policies traceable to the 1930s, but commercial LLMs' accuracy didn't meet standards. Databricks' engineers directly embedded into the customer team — customer-side VP of Data and AI Prabhu Narsina recalled: "They almost met with us daily, wrote code together, debugged together." Final route was fine-tuning open-source models on the platform, about 50 GPUs running training, fine-tuning cycle compressed from over two months on other platforms to two weeks. Project total account: cost down 70%, timeline shortened 75%, data extraction volume up 10x.

Managed service provider Ensono's cooperation with Snowflake turned "firefighting" into "fire prevention": its prediction engine since launch analyzed over 75 million events and 9 million alerts, early warninging before a ticket evolves into a service incident — major incidents reduced over 20%, fault repair time compressed up to 70%.

These two cases fill an easily overlooked part of the variation spectrum: FDE isn't model companies' patent. Companies with platforms in hand and willingness to send engineers into customer sites can all enter this arena — the difference is only whether field experience ultimately precipitates into platform capability, or dissipates in yet another person-based delivery.

### 8.4 Chinese Cases: Planting FDE on "Project-Based" Soil

China is the world's most special enterprise software market: hardest-working delivery engineers, most demanding customization needs, deepest "project-based curse" — big enterprises want customization, vendors lose money per deal, costs can't be amortized, becoming client outsourcing, professional hollowing. FDE model's fate on this soil is a question that must be answered separately: is it the curse's antidote, or the curse's new vest?

How twisted this game is, three practitioners' sighs say clearest. First from database company DolphinDB, an industry long article asked "Who Is Destroying China's Enterprise Software Industry," answer being six mountains: freeloading, open source, outsourcing, bidding, digital subsidiaries (large groups' self-established digital tech subsidiaries), distorted market structure — China's top engineering talent long consumed in "highly customized, strong-relationship, price-war" non-standard delivery. Second from a veteran on podcast *Hard Land Hacker*: "Customization is the natural enemy of SaaS; this curse can only dissolve naturally when the market matures." Third from former DingTalk president Bu Qiong: many companies get stuck at 100-200 million revenue — hard to acquire, hard to deliver, hard to maintain, high customization costs, scale economy nowhere to start.

36Kr summarized these three sighs: "Software productization amortizes project-based R&D expenses, SaaS amortizes sales expenses — only project-based companies suffer most, project costs void upon leaving, can't be amortized out." These three sighs are the Chinese question the FDE model must answer.

#### Big Tech Path: Volcano Engine and Huawei

ByteDance's Volcano Engine is China's internet big tech's most explicit FDE flag-flyer: 2026 specifically formed FDE team, deeply co-creating with industry benchmark customers. Volcano Engine president Tan Dai's public interview wording echoes this book's definition almost word for word: "FDE isn't sales, nor pre-sales — they must have strong technical landing capability, especially AI code landing capability." He also revealed team members deliberately configured with diverse industry backgrounds (like having people from bioengineering background interface with biopharma industry), currently covering automotive, medical, education, financial, semiconductors and other key industries. In July 2026, Volcano Engine also signed strategic cooperation with consulting giant EY, both planning to build a thousand-person FDE team, "exploring AI full-stack delivery new models."

Big tech's weight is clearest in the heaviest industries. In February 2025, Shanghai Ruijin Hospital released clinical-grade pathology LLM RuiPath, co-built with Huawei: 16 GPU cards, two months, completing million-level pathology slide training, data preparation cycle shortened 80%. Pathology is one of China's most resource-scarce medical fields — huge doctor shortage, low primary hospital initial diagnosis concordance rate — this model covers cancer types affecting about 90% of China's annual cancer incidence population. Dean Ning Guang's statement at the launch can be read as the premise for such joint deployments: "We only use technology that withstands verification."

Big tech doing FDE's innate advantage is thick platform foundation (Volcano Ark provides model, toolchain, and cloud infrastructure's integrated foundation); innate challenge is big tech's sales system inertia and "delivery is cost center" financial inertia — whether FDE teams can obtain Palantir-style "field as R&D" organizational status determines whether it's real FDE, or a pre-sales support department with a new name.

#### Pioneer Path: Writing "FDE ≠ On-Site Outsourcing" Into the Website

More noteworthy is a batch of local startups. They lack big tech's foundation, yet use the clearest language to distinguish FDE from China's old species. Qimeng Technology, focused on real estate and facilities management, wrote China's currently most concise definitional differentiation of FDE on its website:

> 1. FDE delivers by phase and accepts by results; on-site outsourcing settles by work hours; 2. FDE brings a product foundation to do engineering; on-site outsourcing writes and modifies from scratch; 3. FDE leaves when done, capability precipitates in the system and your team; on-site outsourcing stays longer and longer, system stops when people leave.

Three sentences correspond to this book's three core propositions: charging by results (Chapter 6), platform foundation (Chapter 7), knowledge transfer (Chapter 5). It also built a "dissuasion mechanism" — not taking scenarios not yet validated, not take data exportable with one spreadsheet, not take those just wanting to understand AI, "we'd rather you start later than start at the wrong time." This is Chapter 2's "refusing the expensive PoC graveyard" conscious practice in the Chinese market.

Another service provider, Qiantuo Technology, moved the FDE model into the finance industry, the most compliance-sensitive sector, and precipitated a clear three-phase methodology: scenario diagnosis 1-2 weeks (identify 3-5 highest-value core scenarios, quantify ROI) → embedded delivery 8-16 weeks (full-stack delivery from model selection to production integration) → production deployment and continuous evolution (used daily by business departments, continuously iterating with business), while emphasizing "data not leaving the domain" — this is localized adaptation to Chinese financial institutions' regulatory environment.

In June 2026, a domestic investment institution practitioner published a long article online with a provocative title: "Silicon Valley's Hottest Position FDE, We've Been Doing It Quietly for Three Years." The article recorded their real feel applying this approach in Chinese enterprise services: Forward Deployed Engineers "after signing, drill into one customer, capability unlimited, truly embedding AI into his business"; measurement standard "not how much code written or how many documents delivered, but whether anyone's actually using the system and whether the customer's business improved"; and that summary completely consistent with this book — "go-live isn't done, he has to stay until the system becomes the customer's daily routine and the customer's own people can take over." This article was widely circulated in domestic practitioner circles, because it first clearly explained in Chinese a comparison table: product engineers responsible for roadmap, pre-sales responsible for signing, implementation responsible for acceptance, customer success responsible for renewal — while FDE is responsible for "whether the customer's transformation and per-capita efficiency truly rose."

#### Control Group: Set-Top Boxes and Paper Contracts

Who FDE should and shouldn't invest in, Baidao Data CEO Wu Guangyu gave two vastly different customers at an entrepreneur roundtable.

One is a set-top box customer, needs extremely clear — "how to use AI in set-top boxes." FDE soaked with them, finally made an agent that watches shows with you and chats gossip, very high ROI. Another is a going-global customer, boss opened with wanting to invest $1 million in AI, but at contract signing always printed the contract and circled changes with a pen, not even using Word's track changes. Wu Guangyu's judgment: "Customers without this kind of digital foundation, FDE investment definitely has no output. We directly told him, first buy 100 Gemini accounts for all staff to use, then talk when you have concrete ideas."

His conclusion echoes Chapter 2's rejection mechanism: FDE's premise is customers having clear need points. Vague, boundary-less requirements shouldn't be invested in lightly; can be split into phase one, two, three, first do the clear parts, after delivering results, subsequent requirements naturally transform into long-term service contracts.

#### The Other Side: Vacuum Layers and Dirty Work

But China's FDE practice isn't all like the above. Frontline news is much rougher.

*Growth Hacker AI Weekly* recorded frontline practitioner Shen Yue's observation: in many domestic projects, FDE is more like vendor outsourcing labor, doing dirty work of filling holes and cleaning up messes. She personally experienced a ten-million-level state-owned enterprise project — the big boss signed the contract then disappeared, no one truly responsible in the project, FDE put in a vacuum layer — upward no decision-maker, downward no executors, finally could only rely on studying "reporting logic" to fight for acceptance. Another Guangdong private home improvement company, second-generation factory owner got straight to the point: help her cut 6,000 people to 3,000. But AI can replace tasks, not positions, the project advanced difficultly amid repeated scolding.

Shen Yue's summary: China FDE's difficulty lies in demand-side layers, weak enterprise digital foundation, bosses lacking patience — and frontline sales' over-promising to sell products, ultimately all repaid by FDE. She also has a quote I used as Chapter 4's epigraph: "No matter how technology evolves, organizational internal human nature and power dynamics remain a more complex problem than technology."

#### Another Voice: Is FDE a Good Business?

Skepticism doesn't only come from the execution layer. At the same roundtable, Kuse.ai founder Wu Xiankun questioned the FDE model itself: "FDE is hard to become a good business model." His reasoning is direct: done shallowly, model companies do it themselves; done deeply, it's essentially still outsourcing, delivery costs high and hard to scale. "Serving state-owned enterprises, you can't refuse out-of-scope requirements, where's your leverage? Will you suspect in the middle of the night that you've become cheap outsourcing — this is a question everyone doing FDE must face."

His solution is quite radical: AI Roll-up (rolling M&A). Since customers worry about data leaks and teams feel outsourcing violates original intent, then buy the company, everyone becomes shareholders, interests aligned, turn the whole company upside down and rebuild; after rebuilding, use the same methodology to continue acquiring the next. His logic: if AI transformation really has that much value, then you should own the business yourself, not sell work hours.

This challenge may not have an answer, but it forms an echo with the Gartner prediction cited in Chapter 5 — 70% of enterprises may abandon FDE-led solutions by 2028: for the FDE model, the hardest gate is its own cost structure. This book doesn't plan to give a standard answer, but it's a question everyone wanting to enter should think through first.

#### Three Special Propsitions of Chinese FDE

Synthesizing these practices and industry observations, for FDE to work in China, it must answer three questions American peers don't need to answer.

**First, pricing.** US market can accept subscription, per-volume billing, even outcome share; while Chinese customers' muscle memory is "buyout plus project-based acceptance." A feasible transitional form is "mixed system": phased acceptance payment, accommodating Chinese customers' procurement habits; value metrics written into acceptance clauses, injecting outcome genes into transactions; then sign an annual maintenance and evolution contract, gradually cultivating renewal awareness. Copying per-resolution charging wholesale would die at the procurement department in most industries.

**Second, platform foundation.** FDE's economics depend on "platform foundation plus on-site customization," while many Chinese software companies' problem is exactly "having field, no platform" — every deal is a person-based business writing code from zero. For these companies, more important than learning FDE's form is filling FDE's foundation: first precipitate highest-frequency customization into reusable components, then talk about Forward Deployment. Without Chapter 7's replication lever, FDE in China will only become "on-site outsourcing with a nice name" — this is exactly why local pioneers wrote "bringing product foundation" into their definition.

**Third, talent.** Chinese engineer culture — can endure hardship, fast response, full-stack generalist, accustomed to solving everything at customer sites — is precisely closest to FDE's requirements, this is the "opportunity"; but the "constraint" is, the past twenty years, such talent has been trapped in per-person-day outsourcing systems, market price signals long undervaluing them. FDE concept's popularization in China may bring a profound side effect: repricing China's hundreds of thousands of delivery engineers. When they learn their peers across the ocean hold $385K median total compensation, this industry's value coordinates will loosen.

Evidence of pricing loosening was already listed in 2026. Demand side, the job market's prices opened up tiers: big tech and AI companies' FDE positions, monthly listed range roughly 20,000-80,000 RMB, high-level annual packages from 400,000 RMB, price gap with traditional implementation engineers pulled to several times (specific market and layering see section 1.8). Supply side, government is moving to supplement people: after Shanghai's first FDE training class in late 2025, February 2026 opened a transformation class for industry engineers, focusing on smart manufacturing, financial, healthcare three industries, first cohort registration exceeded 200 people, three sessions planned for the year, and listed in the municipal professional technical talent knowledge renewal project.

There's also a deeper anchor hidden in traditional software's financial reports. 2025 annual reports, Yonyou per-capita revenue about 480,000 RMB, Kingdee about 620,000 RMB; same year, Palantir's per-capita revenue about $1 million — ten-times-level efficiency gap. This is both the "project-based curse" financial form, and FDE model's biggest imagination space in China: whoever can pull delivery engineers' per-capita output from "person-day" pricing to "results" pricing simultaneously rewrites these tens of thousands people's market prices and this business's financial structure.

Veteran enterprise software companies are also corroborating the talent-side judgment. SAP Greater China president Yuan Xin discussed on the *LateTalk* podcast that Forward Deployed Engineers and traditional ERP consultants' roles are converging, and what's most scarce right now is "composite talent with both product engineering capability and deep business understanding." She also reminded: AI landing's biggest challenge is organizational inertia not technology — basic data architecture's historical debts won't automatically disappear because AI arrived.

#### Judgment

FDE won't cure all of China's enterprise software's chronic ills, but it offers a rare "legitimization" opportunity: redefining "close to customer" from a marker of low-end outsourcing into a marker of high-end capability. China has plenty of engineers willing to go to the field, but lacks three other things: platforms that make field work compound, methodology and pricing structures. Whoever fills these three first has a chance to run out in this world's largest and most complex enterprise services market.

### 8.5 An AI Startup Team's 180 Days: Complete FDE Combat Retrospective

The final case comes from a Chinese AI startup team I tracked and researched (anonymized at team's request, hereinafter "Company N"). It doesn't have Palantir's platform or OpenAI's halo, but its 180-day journey completely demonstrates how this book's methodology operates on a resource-limited team. To protect commercial information, numbers are blurred, but proportional relationships and decision logic remain true. And precisely because of it, this case's reading differs from the previous groups: previous facts can be checked item-by-item against Appendix C; this group please read as a complete "process demonstration" — its value is stringing the entire book's approach in chronological order, factual judgments defer to previous cases.

#### Days 1-30: Choosing the Battlefield, Not Grabbing Contracts

Company N does enterprise knowledge base AI, with three potential customer leads: a top securities firm (big budget, grand requirements), a regional chain retail group (medium budget, specific pain points), a Grade-A tertiary hospital (big influence, sensitive data). Sales instinct is pouncing on the securities firm. But the team followed Chapters 2 and 3's methods, doing triple verification and entry due diligence: the securities firm's problem is "universal requirements" (first meeting wanting to cover the whole company), and no clear business owner; the hospital's pain points are real, but data-not-leaving-domain constraints make delivery cycle uncontrollable; the retail group's CFO personally oversees the project, pain points specific ("3,000 stores' operational supervision reports, regional managers simply can't keep up"), data foundation messy but accessible.

The team chose the retail group — lighthouse value not highest, but triple verification all passed. This is section 3.8's discipline: scheduling ranked by strategic value and learning value, not contract amount.

The securities firm let go deserves a footnote. "Rejection" isn't the only solution to this problem. For big customers with extremely high lighthouse value but vague requirements, there's a third approach: don't do delivery, first sell a paid diagnosis — 2-3 weeks, fixed fee, producing a scenario prioritization report and a data readiness checklist, equivalent to making section 2.3's "graceful exit" into a formal product. If the other party truly has transformation determination, the diagnosis process will boil grand requirements into a clear first scenario, then signing MVD follows naturally; if the other party just wants to write "AI" in their annual report, the diagnosis fee is the touchstone — customers unwilling to even pay for diagnosis shouldn't be done in the first place. Company N didn't walk this path at the time. Reviewing through this book's framework, this was probably the only "correct but regrettable" decision in 180 days: rejection protected capacity, but also gave a potential top lighthouse to peers daring to sell diagnosis.

#### Days 31-75: Entry, Shadow Work, and a "Cut Big Solution"

Two engineers, one industry consultant entered. First two weeks didn't write a line of product code, doing shadow work: following regional managers on store visits, watching them chase store data in WeChat groups, watching them make weekly reports in spreadsheets. Key discovery came from a "workaround": regional managers don't look at reports in the company data system at all — the data source they truly trust is a form store managers fill in daily by hand — because "system data is three days late and always wrong."

This discovery overturned the initial big solution (intelligent data analysis platform), the team narrowed MVD to a small incision: **only make a "store anomaly daily report"** — every morning at 8, aggregating yesterday's 3,000 stores' anomaly signals (sales anomalies, inventory anomalies, complaint surges) into a daily report readable in three minutes, pushed to regional managers' WeChat. Real data, single pain point, six-week hard deadline.

#### Days 76-120: The Secret War of Activation

System going live is only the beginning. Activation period encountered two textbook obstacles. First is trust calibration: week one, AI misjudged two stores' promotion peaks as "anomaly surges," managers complained in the group. The team didn't argue, within 48 hours connected "promotion calendar" into judgment logic, and — key move — publicly thanked the manager who reported the error in the group. Second is influencer management: a veteran regional director (uncrowned king type) initially watched coldly from the sidelines, the team invited him to participate in evaluation criteria revision, his three pieces of experience were written into system rules. Two weeks later, he became the system's most devoted evangelist.

Day 90, the daily report's natural open rate stabilized above 85%. Day 120, the retail group's CIO proactively demonstrated this system at the quarterly business meeting — internal supporter, armed into a salesperson.

#### Days 121-180: The First Brick of Replication

Renewal negotiation had no suspense, but the team did two more important things. First, precipitated assets repeatedly used in this delivery: retail industry's data integration components, "anomaly signal" evaluation framework, store scenario's due diligence checklist — the first scenario playbook took shape. Second, used the retail group's case (customer agreed to joint publication) to open the second customer — a fast-moving consumer brand's channel management department, scenario isomorphic. The second project's delivery cycle shortened 40% compared to the first: the replication flywheel turned its first circle.

180 days, a small team, no financing news, no disruptive technology. But it verified the book's plainest conclusion: this methodology doesn't require platforms or halos, only requires honestly completing every step.

With five groups of cases told, two questions remain: what boundaries should such a force observe (epilogue); and which metrics should entrants watch (Appendix A).

---

## Epilogue: The Professional Ethics of FDE

Every book about methodology must end with one question: when you've mastered this method, where are the boundaries. And this book's topic is heavier than most methodology. Because what FDE hold in their hands isn't ordinary technology — it's the deepest secrets of customer organizations, and increasingly large power to make decisions replacing humans.

FDE's work nature determines what it will see. To do delivery well, you must look at the customer's most real operating data — including the ugly parts; you must map the organization's power structure — including who's incompetent, who's fallen from grace; you must touch core business processes — including those workarounds wandering in gray zones. The customer opens all this to you based on a simple agreement: you're here to help. This trust is the FDE model's foundation, and destroying it only requires one transgression.

I believe FDE's professional ethics have at least bottom lines, written here to share with all peers.

**First, data sovereignty belongs to the customer.** Data seen at customer sites, not a single byte should appear where it shouldn't — not entering AI training data (unless contract explicitly authorized), not entering case material (unless customer gives written consent), not entering your next job's talking points. Least privilege principle isn't just a technical spec, it's professional conduct: don't look if you don't have to, desensitize if you can.

**Second, honestly report results, including bad news.** In result-based charging models, the biggest moral risk is whitewashing results — packaging "system went live" as "value achieved," packaging correlation as causation. Chapter 6's value measurement system can be both the most honest tool and the most sophisticated lying machine, the difference only in human hearts. FDE's foundation is "daring to be tested" — then when tested results are bad, present them with the same mindset.

**Third, don't manufacture dependence, don't sell fear.** This industry has two hidden practices: one is deliberately making systems black boxes, making customers never able to leave you; the other is exaggerating "die if you don't use AI" panic to close deals. Gartner predicts 70% of enterprises will abandon Forward Deployed-led solutions by 2028 due to costs and skill hollowing — this prediction is a warning to the entire industry.

And the healthy FDE model, delivery's end marker is customers running on their own: knowledge transferred to customers, capability precipitated into customer teams.

**Fourth, take "the replaced people" seriously.** FDE-delivered systems in many scenarios do replace some people's work. This book talked extensively about "change management" techniques, but beyond technique is ethics: don't celebrate efficiency in front of the replaced, don't write people as "cost items" without giving paths in solutions, don't play dumb about "whose fate you're changing." Don't use "technology is neutral" as an excuse — the choices deployers make daily are themselves positions.

**Fifth, say no to "things customers ask for but shouldn't be done."** You'll encounter requirements wandering on compliance's edge: "help us make employee behavior monitoring a bit more detailed," "this data is compliance-wise a bit fuzzy, but connect it first." The "French waiter" metaphor has its deepest meaning here — true professionalism isn't satisfying all customer requirements, but daring to guide customers toward directions truly beneficial to them and harmless to the world. The backbone to say no comes from having other customers in your accounts; so morality is always also related to business models.

**Sixth, remember you represent "technology" itself.** For many customers, you're the first face of AI they encounter. Every exaggeration of yours is overdrawing the entire industry's credit in their hearts; every fulfillment is depositing for the entire industry.

The guardrails you design are also making decisions for ordinary people — Anthropic's engineering team publicly retrospected a number: when the system pops up for approval on everything, users approve about 93% of requests, the more they see the less carefully they look, "human-in-the-loop" thus becomes a dead letter in fatigue; so the people designing guardrails can't assume the person overseeing is always alert. When AI increasingly deeply enters society's operations, deployers are the last translation between technology and human daily life — translation distortion's cost is paid by everyone.

These six bottom lines, flipped over, are also your litmus paper for choosing employers. In 2026's job market, positions with the FDE title skyrocketed annually, yet only about 10% of engineers willing to do this work — the supply-demand gap is packed with bandwagoners. Under the same title, frontier lab positions are "software engineering plus customer sites," while bandwagon companies' positions may just be on-site outsourcing with a new name: one engineer discovered after joining that the company only wanted him to do project coordination, not planning to let him write a line of code, and resigned after four weeks.

Before entering the industry, ask one more question — whether this position writes production code, whether field experience feeds back to product — is far more important than salary negotiation.

Palantir itself is controversial: its history serving intelligence and military institutions makes many people wary of everything about it — including the FDE model. I extensively cite its methodology in this book, which doesn't equal endorsing all its customer choices. Precisely on the contrary, exactly because the fields it serves are so sensitive, those disciplines in its engineer culture about permissions, audits, and need-to-know are especially worth learning.

Nabeel Qureshi, who spent nearly eight years as FDE at Palantir, classified projects he handled by moral attribute: morally neutral, clearly doing good (pandemic response, combating child exploitation), and gray zones (military, immigration, policing). Facing gray zones, his answer isn't pursuing moral purity, nor turning away and exiting, but "staying in the room" — keeping one's vote at the decision table. I cite this classification because it's closer to deployers' real situation than "resist" or "obey": most moral dilemmas happen precisely in gray zones, and leaving gives the room to less discerning people — not necessarily a more moral answer.

FDE is a young profession, its professional code hasn't been written by anyone. Hope this book is its first boundary marker.

## Acknowledgments

Thanks to Bob McGrew, Barry, Ted Mabrey, Nabeel Qureshi and other former Palantir employees for their public recollections and writings — you turned a "secret company's" methodology into public knowledge; thanks to podcast hosts of YC Lightcone, Latent Space and others, your questioning preserved much first-hand experience; thanks to a16z, MIT NANDA Lab, The New Stack, CIO.com for research and reporting; thanks to China's FDE pioneers who wrote their thinking on their official websites — the Chinese-language world's discussion needn't start from zero because of you.

Thanks to everyone willing to read to this point. May the roads you build have travelers; may the roads remain after you've walked them.

---

## Appendix A: Common Metrics FDE Should Track

This appendix provides FDE work's full-chain metrics system, organized in four layers: delivery layer, customer layer, commercial layer, organization layer. Metrics are valuable for precision not quantity — each customer project watching 3-5 core metrics beats a wall-covering dashboard.

### 0. High-Frequency Jargon Quick Reference

One plain sentence per term. When stuck while reading the main text, come back here.

- **FDE (Forward Deployed Engineer):** Engineer embedded at customer sites, responsible for results.
- **Ontology:** Modeling enterprise data, logic, and actions into a semantic layer models can understand.
- **Bootcamp:** Customers bring real data, a usable prototype in one to five days, executives decide on the spot.
- **Echo / Delta:** Palantir's two-person combination — the former reads the customer, the latter builds.
- **PoC Graveyard:** Open-ended, metric-less, judge-less pilots that die in the doing.
- **MVD (Minimum Viable Deployment):** Using minimum engineering investment to verify value actually occurs once in the real environment.
- **Shadow Work:** Sitting beside a real user, watching them through their real day.
- **Lighthouse Customer:** Customer who can send signals to the entire industry, endorsement value greater than contract amount.
- **Requirement Locust:** Ample budget,旺盛 demand, but drains the team without producing compound interest.
- **NRR (Net Revenue Retention):** Whether the same batch of old customers pays more or less this year than last, 100% passing.
- **RPO (Remaining Performance Obligations):** Signed but not yet recognized revenue contract value.
- **ARR / ACV:** Annual Recurring Revenue / Annual Contract Value.
- **Rule of 40:** Revenue growth plus adjusted operating margin, software industry health indicator, 40 passing.
- **Charging by Results:** Customers don't pay for software, they pay for "problems solved."
- **Per-person-day pricing:** Charging by engineer headcount times days — outsourcing's old pricing method.
- **SLA (Service Level Agreement):** Commitments on availability, latency, error rates.
- **Health Score:** Customer checkup score synthesized from usage, value, relationship, commercial four signal types.
- **QBR (Quarterly Business Review):** Quarterly meeting where vendor and customer align value.
- **RAG (Retrieval-Augmented Generation):** Letting models check materials before answering.
- **Evaluation System:** System building quantifiable rulers for fuzzy business quality, simultaneously the billing foundation.
- **MCP (Model Context Protocol):** Open standard letting models connect external tools, led by Anthropic.
- **Customization Decrease Rate:** The Nth customer's customization volume should be significantly less than the 1st's; if not decreasing, it's outsourcing.

### 1. Delivery Layer Metrics (Is the project done right)

**TTV (Time to Value):** Time from entry to customer's first measurable value. FDE model's lifeline metric. Reference standard: MVD validation should be measured in weeks (2-6 weeks), full deployment in months (1-4 months). TTV continuously lengthening is the first signal of methodology or platform foundation problems.

**PoC Conversion Rate:** Proportion of validation projects entering paid deployment. Palantir's Bootcamp took this number from early 5-10% to company-disclosed about 75% (another standard says some sessions higher) — it simultaneously measures "customer screening quality" and "delivery quality." Too low conversion means entry screening dereliction; too high (near 100%) requires checking whether you're only taking unchallenging deals.

**Evaluation Pass Rate:** Proportion of AI output passing business evaluation sets, and its time series trend in production. Quality drift's alarm.

**Resolution Rate and Deflection Rate's Caliber Discipline:** Resolution rate (proportion of conversations closed without human intervention) and deflection rate (deflection, proportion of users stopped by self-service, no longer entering human channels) are customer service deployments' core value metrics, and also the metrics with messiest calibers across vendors. Taking ServiceNow's official standard, a deflection requires two conditions simultaneously: no ticket submitted within 24 hours after interaction, AND positive engagement signal (like user giving positive feedback on results). Before citing any vendor's resolution rate or deflection rate, first ask three things clearly: what's the denominator, how long's the judgment window, who judges — an unclear-caliber 86% is worse than a clear-caliber 51%.

**Deployment Frequency and Rollback Rate:** Hard metrics for iteration speed. Healthy deployment period should maintain high-frequency small steps (weekly or even daily), rollback rate low and stable.

**Defect Escape Rate:** Proportion of defects discovered only after go-live. Measures testing and evaluation system's completeness, not engineer level.

### 2. Customer Layer Metrics (How's the customer doing)

**Activation Rate:** Proportion of target user group forming stable usage habits. Note denominator is "target user group," not "system account count." Warning: deployments with long-term low activation rate are nominally alive, actually dead.

**Usage Depth:** What percentage of key functions are used by people (how many scenarios used), usage frequency distribution (check-in style use or workflow embedding), and emergence of self-service exploration behavior (users starting to discover new uses themselves — this is the most precious signal).

**Health Score:** Synthesized from usage, value, relationship, commercial four signal types (see section 5.6). Key discipline: full review weekly, automatically triggering intervention process when dropping below warning lines.

**Supporter Coverage Count:** Number and level distribution of active allies in the customer organization. Single point is high-risk, three points form a net.

**NPS Caution:** NPS (Net Promoter Score, asking "how likely you'd recommend us to others") has limited reference value in enterprise scenarios — small samples, politicized. More reliable alternative is "early inquiry of renewal intention": two quarters before expiration, directly ask supporters "if renewing today, would you renew."

### 3. Commercial Layer Metrics (Is the business worthwhile)

**NRR (Net Revenue Retention):** Annual change in existing customer revenue (including churn, downgrade, expansion). FDE business model's final judge. Passing line 100%, excellent line 120%. Companies with NRR above 120% have endogenous growth engines.

**Delivery Gross Margin:** (Single customer revenue minus delivery direct costs (labor, travel, cloud resources)) / single customer revenue. FDE model's passing line floats with platformization degree: pure labor delivery period may only be 20-40%, after platform reuse rises should climb toward 60%+. Whether gross margin rises fast says more about whether the model works than absolute level — FDE that doesn't rise is a consulting company.

**Customization Decrease Rate:** McGrew's touchstone — the Nth customer's customization workload should be significantly less than the 1st's. Three consecutive customers without decrease, immediately review product feedback mechanism.

**Sales Cycle:** Time from first contact to signing. Palantir used Bootcamp to compress it from 9-12 months to weeks. It's a composite reading of acquisition efficiency and trust asset thickness.

**CAC Payback Period:** Time for Customer Acquisition Cost (CAC, including free validation investment) to be recovered through contract gross margin. FDE model's early period is universally ugly; the key is seeing it shorten with case accumulation.

**LTV/CAC:** Customer Lifetime Value (LTV) to CAC ratio. Enterprise business's healthy line is generally above 3; FDE model due to front-loaded acquisition cost may be below 2 early, must be read together with NRR to be meaningful.

### 4. Organization Layer Metrics (Can the team go the distance)

**Field-to-Product Feedback Rate:** Output count precipitated from field into components or platform capability per unit time (component entry count, playbook update count, platformization proposal count). This metric measures whether the FDE model's "soul organ" is still beating.

**Delivery Asset Reuse Rate:** Proportion of new projects reusing existing components, templates, checklists. Reuse rate is the three-level replication lever (Chapter 7)'s composite reading, target should rise quarter by quarter.

**FDE Per-Capita Capacity:** Annual revenue supported by each Forward Deployed Engineer. It's the scaling total account: pure labor mode's ceiling is obvious, after platformization should continuously rise.

**Team Endurance Metrics:** Travel intensity (monthly travel days), on-call load, turnover rate and burnout warning signals. Reddit's FDE practitioners' biggest complaint is travel and endurance — team burned dry, all previous metrics are fireworks.

### Usage Suggestions

1. Each customer project locks 3-5 "core metric combinations": usually one value metric + one usage metric + one relationship metric.
2. Baseline data collected on project launch's first day — miss it and it's gone forever.
3. Metrics co-built with customers, mutually recognized, otherwise they have no效力 at the renewal negotiation table.
4. Review the metrics system itself every half year: delete what no one looks at, add what's repeatedly asked.

---

## Appendix B: FDE People and Team Directory

This appendix lists people, teams, and knowledge sources that can't be bypassed for understanding the FDE model. The complete source list referenced during this book's writing is in the research notes published with the manuscript.

### 1. Key People

**Shyam Sankar** — Palantir President and CTO, early employee. Widely considered inventor of FDE strategy: the person who redefined "on-site customization" from cost as "product discovery." His public statements are first-hand material for understanding Palantir's philosophy.

**Bob McGrew** — PayPal early engineer, Palantir early executive, former OpenAI Chief Research Officer (led ChatGPT, GPT-4, o1 development). FDE model's best interpreter. "Gravel roads and highways" and "doing things that don't scale at scale" both come from him. Must-read: YC Lightcone podcast *The FDE Playbook for AI Startups* (September 2025).

**Stephen Cohen** — Palantir co-founder. Inventor of the demo loop: protagonist of "this is terrible" and "so what would you want it to be different."

**Alex Karp** — Palantir CEO. Proposer of the "French waiter" behavioral model: opposing obsequious order-taking engineering culture.

**Barry** — Former Palantir Forward Deployed Engineer, author of *Understanding Forward Deployed Engineering*. FDE model's most important "insider warning": the real account of costs, chaos, and burnout.

**Ted Mabrey** — Palantir senior employee and writer, firsthand recollector of the "Sankar Bomb" email (Sankar's all-hands email announcing strategic shift). He broke "everything speaks through results" into two questions: "Does it actually work? Does it actually matter?"

**Nabeel Qureshi** — Spent nearly eight years as Forward Deployed Engineer at Palantir, author of *Reflections on Palantir* (2024). Stationed at Toulouse Airbus site for a year; "fuck generalizability," hiring's "bat signal" reverse screening, "data problems 95% are integration, cleaning, association," and facing gray-zone projects' "staying in the room" moral three-classification all come from his public writings.

**Vinoo Ganesh** — Designer of Palantir's rotational training program (Project Frontline), author of *The Definitive Guide to FDE* (2026). "You can't build a real FDE organization through hiring, only through cultivation" — over 250 engineers entered real deployment through rotation, alumni scattered in OpenAI, xAI, Anduril. The book's Chapter 7 six-month self-cultivation checklist and Chapter 4's "2.3 million data entries crashing memory" incident retrospective both come from his first-hand writings.

**Colin Jarvis** — OpenAI Forward Deployed Engineering team lead, the person who built OpenAI's FDE organization from zero.

**Brad Lightcap** — OpenAI COO, leader of "The Deployment Company."

**Natalie Meurer** — Sierra Agent Engineering lead (former Palantir five years). Namer of "Agent Engineer." Must-read: Latent Space podcast interview (July 2026).

**Bret Taylor / Clay Bavor** — Sierra founders (former Salesforce co-CEO and former Google VP respectively). People who made the FDE model into the business model itself (charging by results).

**Jesse Zhang / Ashwin Sreenivas** — Decagon founders (the latter from Palantir). Designers of Agent Operating Procedures, the model of "productizing delivery experience."

**David Wakeling** — Former Linklaters Market Innovation lead, in-firm supporter of Harvey's first lighthouse deployment. Best sample of customer-side supporter perspective.

### 2. Iconic Teams

**Palantir FDE Organization** — The mode's inventor and completed form. "Echo-Delta-Platform" triangle, Bootcamp machine.

**OpenAI Forward Deployed Engineering Team** — Formed 2024, globally distributed, operator of John Deere and BBVA; upgraded to "The Deployment Company" in 2026.

**Anthropic Applied AI Team** — FDE organization under the name "Applied AI Engineer," co-builder of FIS financial crime agents; formed enterprise AI services joint venture with Blackstone and others in 2026.

**Sierra Agent Engineering Team** — The extreme form of charging by results + hosted delivery (founded 2023, valued $4.5B October 2024, reportedly continued climbing since).

**Harvey Deployment Team** — Vertical industry (legal) FDE textbook (founded 2022, valued $11B March 2026, user coverage 100,000+ lawyers).

**Cognition Forward Deployed Team** — "Embedded in partner's body" ecosystem bundling model: from 2026 an embedded Forward Deployed Engineer team stationed at global IT services giant Cognizant, responsible for project screening, engineer mentoring, and effectiveness measurement, leveraging partner's decades of customer relationships to roll product into healthcare, financial, and insurance large enterprises.

**Scale AI / Databricks / Salesforce / Google Cloud / Mistral / Cohere** — Each has FDE or isomorphic positions, different names (Solutions Architect, Customer Engineer etc.), same skeleton.

**Volcano Engine Doubao LLM FDE Team** — China's internet big tech's most explicit FDE organization (formed 2026, covering automotive, medical, education, financial, semiconductors; building thousand-person team with EY).

**Chinese Local FDE Pioneers: Qimeng Technology, Qiantuo Technology** — Local service providers with real estate facilities management and finance as positions, publicly outputting the definitional thinking that "FDE ≠ on-site outsourcing."

### 3. Knowledge Sources (Ranked by Importance)

1. YC Lightcone podcast: *The FDE Playbook for AI Startups with Bob McGrew* (September 2025) — 51-minute retrospective by the mode's first narrator.
2. a16z: *Trading Margin for Moat* — benchmark for business model analysis.
3. Barry: *Understanding Forward Deployed Engineering* — insider's cool-headed warning.
4. MIT NANDA Lab: *The GenAI Divide: State of AI in Business 2025* — source of the "95% failure rate," the data foundation for FDE's reason to exist.
5. The New Stack: *Why OpenAI and Anthropic Are Both Racing to Build FDE Teams* (May 2026).
6. CIO.com: *Anthropic's Financial Agents Expose the New Bottleneck of Forward Deployed Engineers* (May 2026) — buyer perspective and Gartner warning.
7. Latent Space podcast: *Forward Deployed Engineers and the Future of Software Engineering* (July 2026) — Sierra perspective.
8. Palantir official blog: *A Day in the Life of a Palantir Forward Deployed Engineer* (2020) — official self-account, Chinese translation circulating.
9. OpenFDE community (open-fde.com) — practitioners' open-source community, position and company map.
10. 36Kr *China's To B Software: Escaping the Loss-Making Growth Trap*, Chen George WeChat public account FDE series articles — must-read comparison for Chinese context.

### 4. Compensation and Job Reference

- GetPerspective: *2026 Forward Deployed Engineer Compensation Report* (1,200 samples) — top lab mid-level FDE median annual total compensation about $385K, senior about $610K, principal over $1.2M.
- fdenest.com / fde.academy / sundeepteki.org — three dedicated sites for interview preparation and career paths.
- Levels.fyi — real-time compensation data for Palantir and other positions.
- Job postings themselves are the best textbook: OpenAI, Anthropic, Decagon, Harvey, Scale AI's FDE job postings are worth studying word by word.

---

*Translation note: This is a fan translation for learning purposes. The original Chinese text is by Fan Bing (XDash), published at fde4.ai and github.com/xdash/FDE-the-Guidance-Book-of-Forward-Deployed-Engineer. All rights belong to the original author.*
