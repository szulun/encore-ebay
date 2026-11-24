# Prompt Log: eBay Fashion Strategy and the Encore Prototype

**Author:** Szu Lun Huang
**Course assignment:** Extra credit, “Make eBay the #1 fashion marketplace” (due November 30, 2026)
**AI tool:** Claude (Anthropic), used in claude.ai between November 23 and 24, 2026
**Language note:** The working session was conducted in Traditional Chinese. The prompts below are translated into English, lightly condensed, and kept in their original order. Quotes from interviewees were translated too, except Respondent E, who answered in English.

This log has three parts:

1. The prompts I used to develop the strategy, the prototype and the deck.
2. The prompt the prototype itself sends to Claude to appraise a piece of clothing.
3. Where I made the key decisions, as opposed to the AI.

---

## Part 1. Session prompts, in order

### Phase 1: Understanding the assignment and finding the problem

**1. Kickoff**
> *[Uploaded a screenshot of the assignment brief]* Let’s discuss first.

**AI output:** A breakdown of the grading weights (Innovation 20, “#1” strategy 15, Customers 15, Competition 15, Roadmap 15, Metrics 10, Deck 10) and the argument that defining “#1” is the decision everything else depends on. Proposed candidate definitions (pre-loved fashion, trusted luxury, hard-to-find items).

**2. My view of eBay**
> I’m thinking about what eBay’s problem is. To me it’s just a transaction platform. I don’t feel it’s especially suited to luxury or fashion items. If eBay wants to do this, it might need a sub-brand, because eBay feels like an auction platform.

**AI output:** Reframed my point as a jobs-to-be-done problem: eBay is built for *searching* (you know what you want), while fashion is *browsing* (you want inspiration and identity). Laid out three options: a fully separate brand, a new storefront on a shared backend, or a fashion section inside eBay.

**3. Choosing the model**
> Option 2, “new storefront, shared backend”: a separate brand and app designed for browsing, reusing eBay’s inventory, sellers, payments and authentication. That’s my favorite too.

**AI output:** Stress-tested the model: the riskiest assumption (eBay’s messy listings won’t look browsable), cannibalization, and how visible “by eBay” should be.

**4. Target customer**
> *(Follow-up)* What age is Gen Z?

**AI output:** Born 1997 to 2012 (Pew Research Center), so 14 to 29 in 2026; because eBay requires users to be 18+, the real target is 18 to 29.

### Phase 2: Finding the innovation

**5. My own behavior as a starting point**
> I use Poshmark. I don’t think it’s good or bad. I just want to compare: where is the same item cheaper? Maybe we could have a pricing suggestion feature that checks what other sites sell the same thing for, and gives our users a suggested price.

**AI output:** Turned this into two sides of one engine: a suggested price for sellers and a “good price” label for buyers. Flagged that showing competitor prices would send buyers away, and that eBay’s decades of *sold* prices are a data advantage rivals don’t have.

**6. Interview questions**
> Please translate these into English: What comes to mind when you think of eBay? Would you buy clothes on eBay? How do you usually buy secondhand clothes?

### Phase 3: Building the prototype

**7. Start building**
> Let’s do what we can first. *(After confirming the seller-side flow)*

**AI output:** A working web prototype (“Encore by eBay”): upload a photo → Claude identifies the item → writes the listing → suggests three prices (quick sale, recommended, max value) with estimated days to sell.

**8. Interview insight**
> *(Sharing a friend’s answers)* “eBay makes me think of secondhand goods. I wouldn’t buy clothes there because I never have. I go to Goodwill.” … I think Goodwill wins because you can see the item, and the treasure hunt.

**AI output:** Two needs: *seeing it* (trust) and *the hunt* (fun). Real competitors include offline thrift stores, not just apps.

**9. The buyer side**
> This is the page where the user uploads, right? What about the display after upload?

**AI output:** Added a buyer-facing preview of the listing, including a “good price” label.

**10. Visual direction**
> For users, the page itself matters. It has to be beautiful, or I won’t want to browse. *(Shared screenshots of Mercari Japan, Poshmark and The RealReal)* These are sites I like to browse. I want a vintage feeling: retro and premium. *(Shared vintage reference images)* This kind of feeling, gold. What do you think?

**AI output:** Analysis of why The RealReal feels premium (consistent studio photos, serif type, white space, editors’ picks) and the insight: “The RealReal’s look, at eBay’s scale,” achieved with AI instead of a warehouse. Proposed “ornate outside, clean inside”: gold, aged paper and vintage badges for framing, clean product grids.

**11. Three pages**
> The prototype should have an upload page, a home page and a “my page.” I want them to look really good.

**AI output:** Rebuilt the prototype as three pages: Shop (curated edits, good-price stamps, editors’ picks), Sell (AI appraisal with a kraft-paper price tag) and My closet (earnings, an AI price-drop nudge, saved items).

**12. Photo quality**
> Like you said, we need to teach users how to take better photos. So should the AI detect problems, or generate photos for them?

**AI output:** Recommended detection and coaching, not generation. Design principle: **“AI edits the background, never the clothes,”** because the biggest fear in buying secondhand online is that the item won’t match the photo.

**13. Polish**
> Don’t you think the text is a bit hard to read? *(Then supplied product photos and asked to swap them in.)*

**AI output:** Fixed thin display type and low-contrast gold; replaced the line drawings with real photos.

### Phase 4: The deck, research and reframing

**14. Deck draft**
> For the slides, please make a Chinese version first so I can review it.

**AI output:** A 19 to 20 slide draft mapped to the grading rubric, with speaker notes.

**15. More interviews and a research-design check**
> *(Shared answers from three more friends, including:)* “eBay is a magical store that sells everything. I wouldn’t buy clothes there, there are lots of other clothing sites like 24S.” … Maybe the people I asked don’t buy secondhand at all.

**AI output:** Identified sampling bias and split respondents into resale shoppers and non-resale shoppers; suggested a screener question (“In the past year, have you bought secondhand clothes? Where?”).

**16. Real numbers**
> You haven’t filled in the numbers, have you? Please search and fill in reasonable figures.

**AI output:** Market data from ThredUp’s 2026 Resale Report and eBay’s 2026 Recommerce Report, targets labeled as assumptions with the math in speaker notes. **Key discovery: eBay completed its acquisition of Depop in July 2026.**

**17. Back to the brief**
> OK, but this goes back to the question: what is the teacher actually asking?

**AI output:** Flagged that the deck had drifted into pitching a new startup instead of answering “make *eBay* #1.” Reframed: eBay is the hero; Encore is one of three cards (Depop, Encore, eBay) on a shared backbone, and AI listing improves eBay’s experience today.

**18. Is Encore still needed?**
> eBay used to sell everything, and now it wants to do fashion. But it acquired Depop, so I’m not sure we still need Encore. The positioning has to be very clear, and why it should exist. eBay really isn’t fashion, and I don’t think Depop is fashion either.

**AI output:** Agreed and turned it into Encore’s reason to exist: neither eBay nor Depop stands for taste. A positioning map (price vs. taste and curation) shows an empty space for “affordable, tasteful pre-loved” between Depop and The RealReal.

**19. Personal insight**
> I don’t buy luxury on eBay because I didn’t know it did luxury authentication. I only found out later.

**AI output:** “eBay’s best asset is hidden.” Encore should make authentication visible, not just reuse it.

**20. Connecting the portfolio in the prototype**
> Please summarize. So should our prototype also include eBay and Depop?

**AI output:** Instead of copying eBay’s and Depop’s interfaces, show the portfolio inside Encore: AI recommends which marketplaces to list on, an “Authenticated by eBay” badge on luxury pieces, and one closet showing where each item is listed.

**21. Why Depop works**
> Why did Depop succeed? Was it because of Instagram ads reaching its target customers?

**AI output:** Mainly a social, feed-based product and word of mouth, with ads as an accelerator. Surfaced reports that users and sellers “graduate” from Depop, which became the deck’s growth path: Depop (about 18–22) → Encore (about 23–30) → eBay (about 30+).

### Phase 5: Shipping

**22. Export and demo mode**
> *(Class Claude licenses close November 28.)* Do I need to add the demo link and prompt log? Please build the demo mode, compile a prompt log in English, and translate the slides into English. I’ll put the demo on GitHub Pages.

**AI output:** A demo mode for the public link (sample appraisals, clearly labeled), this prompt log, and the English deck.

---

## Part 2. The prompt inside the prototype

When a seller uploads a photo, the prototype sends this prompt to Claude along with the image, and asks for JSON that drives the interface. In the public demo, the three sample appraisals were prepared in advance in the same format.

```
You are the listing and pricing assistant for Encore, a curated resale fashion app by eBay for Gen Z and young millennial shoppers who love vintage and quality pieces.

The attached photo shows one fashion item a seller wants to resell.
Seller notes: [seller’s optional notes]

Do three things:
1. Identify the item: brand (write "Unbranded" or "Unknown" if you can't tell), category, item name, main color, material if visible, style or era, and size if visible or stated.
2. Write a listing a style-conscious buyer would click on: a title under 80 characters with item, one key detail and era if relevant (the brand is shown separately, so leave it out of the title); a 2-3 sentence description in a warm, honest voice that mentions condition; and 3-5 lowercase style tags (for example vintage, 90s, minimalist, workwear, quiet luxury, y2k).
3. Suggest a resale price in USD for the US secondhand market (eBay, Poshmark, Depop, Vinted, The RealReal), based on typical prices for comparable pre-owned items in similar condition. Give three price points (quick sale, recommended, max value) and the estimated number of days to sell at each. Quick sale must be lowest and max value highest. If you know it, give the item's approximate original retail price.

4. Recommend where to list it within the eBay family of marketplaces: "encore" (curated pre-loved fashion: quality, designer, vintage or timeless pieces in good condition), "depop" (Gen Z community: streetwear, Y2K, trend-led or affordable casual pieces), "ebay" (the widest reach, luxury buyers who want authentication, and long-tail searches). Recommend one to three of them, and write a one-sentence reason for each of the three, addressed to the seller. Also say whether this is a designer or luxury piece that should go through eBay authentication.

Be honest about uncertainty. If you can't see the brand, size or condition, lower your confidence and list what the seller should confirm before listing.

Reply with only a JSON object in exactly this shape:
{
  "item": {"brand": string, "category": string, "name": string, "color": string, "material": string, "style": string, "size": string},
  "confidence": "high" | "medium" | "low",
  "title": string,
  "description": string,
  "tags": [string],
  "condition": "New with tags" | "Like new" | "Good" | "Fair",
  "confirm": [string],
  "price": {"quick": number, "recommended": number, "max": number, "days_quick": number, "days_recommended": number, "days_max": number, "retail": number | null},
  "why": [string, string, string],
  "comparables": [{"label": string, "price": number}],
  "channels": {"recommended": ["encore" | "depop" | "ebay"], "reasons": {"encore": string, "depop": string, "ebay": string}},
  "authenticate": boolean
}
"size" is "Unknown" if not visible or stated. "confirm" holds 1-3 short questions for the seller. "why" holds three short reasons for the recommended price. "comparables" holds 3 typical comparable pre-owned listings with their usual selling price.
```

---

## Part 3. Who decided what

The AI drafted, researched, structured and built. These calls were mine:

- **The core problem:** eBay feels like an auction or transaction platform, not a place for fashion; it needs a separate brand experience.
- **The innovation’s starting point:** my own habit of comparing prices across sites became the pricing engine.
- **The visual direction:** vintage, retro and premium, with gold, based on sites I actually browse.
- **Three pages** (Shop, Sell, My closet) and teaching users to take better photos.
- **Catching sampling bias** in my own interviews.
- **Returning to the brief** and asking what the teacher is really asking, which led to reframing around eBay.
- **Challenging whether Encore should exist** after learning eBay owns Depop, which produced the positioning map.
- **The hidden-asset insight** from my own experience: I didn’t know eBay authenticates luxury.

## Sources used in the deck

- ThredUp, 2026 Resale Report (US secondhand apparel market size and growth; share of incremental spend from new shoppers)
- eBay, 2026 Recommerce Report (frequency of secondhand purchases by 18–29-year-olds)
- Fortune, October 29, 2026 (eBay’s acquisition of Depop; Depop active buyers; eBay and Depop US fashion sales)
- Retail Gazette, July 2026 (completion of eBay’s Depop acquisition)
- Reporting on Depop’s social, feed-based design and creators “graduating” from the platform
