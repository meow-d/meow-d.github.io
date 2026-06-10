---
tags: computers
---

mermaid is most people's introduction to the "diagrams as code" concept, being the one that popularized that concept, gathering extremely widespread support along the way. imagine being supported by even github, you can write in mermaid and it'll show up as a chart; like that's an incredible achivement. even if it did not invent the concept, it wouldn't be wrong to say that mermaid is life-changing to a lot of people.

unfortunately, mermaid does not act that way. rather than staying proud and saying "we're the one and only mermaid", they active want to be a mere product, they want to appeal to people who do not care about mermaid.

the thing is, i like open source developers earning money, i like using mermaid with ai, and building a product around an open source project is entirely valid. plenty of companies use the open core model while staying completely focused on their core audience - [typst](https://typst.app/) comes to mind.

so i'm not sure why mermaid's attempts to make money became so aimless and confusing. there is much confusion between mermaid chart (the company), mermaid.js (the library), mermaid.live (mermaid live editor), and the new mermaid.ai. by the way, they are also getting rid of their js.org domain in favour of mermaid.ai, presumably unifying everything under the new mermaid.ai. except for some reason they didn't put up a redirect. mermaid.js.org has the documentation and a notice, mermaid.live has the live editor, mermaid.ai has both (plus its own new app) (plus another [documentation](https://mermaid.ai/docs/mermaid-oss/syntax/flowchart.html)).

the mermaid.ai homepage is this claude aesthetic ai startup page. i personally associate that design language with disingenuous startups, but that's entirely subjective. what *is* objective is how generic that home page is, how little it says about mermaid's true impact.

---

once you look into something like [plantuml](https://plantuml.com/), which has been around for far longer, you realize mermaid is a complete mess. the syntax and looks of every diagram is inconsistent, sometimes with questionable quicks.

my final straw is the realization that mermaid-cli requires puppeteer and chromium, where every command spawns a chromium instance. it is unfair to blame them, you can't just force yourself to solve a [technical challange](https://github.com/mermaid-js/mermaid/issues/3650#issuecomment-2298254704), but i would never have considered that problem would exist in a million years, it certainly doesn't on any competitor.

---

i don't want to be a doomer. so let's look at the positive side.

the new mermaid.ai app is good. you can edit diagrams visually and drag items around, so you get the best of both worlds. the ai integration is nice. but the 3 diagram limit is atrotious though; if they're giving away ai credits at all, can't they at least afford to store some files.

i'm also grateful that there is competition, showing us what could have been done better, and as a fallback, especially on some UML diagrams that mermaid lack.

there's even [D2](https://d2lang.com/), a "competitor" in a more literal sense because they are also an open core company selling [a similar platform](https://terrastruct.com/d2-studio/index.html), without the ai. they seem to be much more competent and consistent visually too. most importantly, it's a single 50MB binary because it's written in golang. god bless golang.

