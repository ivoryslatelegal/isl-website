# Ivory Slate Legal — Website (V12)

This folder is a complete, ready-to-host website: `index.html` (homepage), a dedicated DPDP Act compliance page at `dpdp-act-data-protection-compliance/index.html`, a `dpdp.html` redirect stub for anyone with the old link, a `docket/` section (index page plus one folder per post, plus a `docket/assets/` folder with per-post title-card images), a `team/` page with the firm's roster and photos, `robots.txt`, `sitemap.xml`, and a `CNAME` file, a root-level `favicon.ico`, and an `assets` folder with the logos (PNG plus WebP), favicons, and team photos (`assets/team/`). No build step, no dependencies - just static files.

## What's new in V12
A new **Our Team** page (`/team/`), linked from the main nav and footer on every page.

1. **Nine team members featured**, grouped by seniority - Partners, Senior Associates, Associates, Paralegals - with photo, name, title, and a short bio for each. Gauri Jasana and Samarth Acharya (the firm's Managing Partners) are intentionally not featured, per the standing decision to keep them off the public-facing site for now; this page instead introduces the other partner and the associate/paralegal team as the firm's public face in the meantime.
2. **All seven practice areas assigned a named head.** Each Partner and Senior Associate heads one or two of the firm's seven practice areas (Litigation & Dispute Resolution, Regulatory & Compliance, Mergers & Acquisitions, White Collar Crime & Investigations, Banking & Finance, Corporate & Commercial, Intellectual Property & Trademarks), with Associates and Paralegals mapped in support underneath. Bios were checked and revised with you over several rounds, and the specific services named in each bio (e.g. "MSME Act Section 18 claims," "trademark search & registration") are pulled directly from the existing Practice Areas section for consistency.
3. **Interactive photo cards**, matching the site's existing motion language: a mouse-tracking 3D tilt and spotlight glow on each photo, a bio reveal on hover (falls back to a bio line shown by default on mobile, where hover doesn't apply), scroll-triggered fade-in, and a lift/border-glow on hover - built with the same easing curves and teal/cream palette as the rest of the site.
4. **Photos processed and delivered as a single set** in `assets/team/`, cropped to a consistent 3:4 portrait ratio and compressed for web use.
5. Since this adds a new page/section (not a bug fix), the version number moved to a new whole number per the versioning convention agreed earlier, rather than a decimal bump.

## What's new in V11.4
A quick follow-up correction on the post-page layout, after review of the delivered V11.3 build:

1. **"Back to The Docket" link moved back to the left**, above the headline - left-aligned, arrow pointing left. (V11.2/V11.3 had it right-aligned; on reflection the left position reads more naturally as "back".)
2. **Header image narrowed to 700px**, flush with the article text column, instead of the wider 960px used in V11.2/V11.3.

## What's new in V11.3
A visual-bug and brand-accuracy pass on the V11.2 Docket round, caught from a screenshot review before you uploaded:

1. **Featured post's image on the Docket index no longer crops.** It was being stretched to fill the row height set by the text next to it, cutting off the sides of the image and part of the title. It now keeps its correct 1200:630 shape and centers in the row.
2. **Header image on post pages widened.** It was capped at the same 700px width as the article text, while the teal hero band above it ran full-width - leaving it looking small and stranded. It's now 960px wide, so it reads as a proper visual continuing the hero. The article text itself stays at 700px for readability, and stays un-boxed (we talked this through - a boxed article body would've been a bigger, unnecessary departure from how the rest of the site reads).
3. **Title-card images rebuilt to match the actual brand collateral.** The line motif in the first version was an invented pattern that didn't match the firm's real brand assets. Rebuilt using the exact clustered-parallel-contour-line motif from the brand reference image, banked to the right edge the same way - the same motif already used in the homepage hero.

## What's new in V11.2
A Docket polish round, all four items you asked for:

1. **Post cards rearranged into a "featured + grid" layout.** The most recent post shows large at the top (image left, title/description right), with older posts below it in a uniform two-column grid. This was chosen over a fully asymmetric/bento grid specifically because it holds up as more posts get added one at a time through the self-serve workflow - there's always exactly one "featured" slot, and everything else just drops cleanly into the grid, no manual rebalancing needed.
2. **"Back to The Docket" link moved to the right.** It now sits flush right above each post's headline, instead of being stranded on the left where it looked accidental - the arrow still points left/back, since that's what it does.
3. **Share buttons added to every post** - LinkedIn, X, WhatsApp, and Copy Link, styled as small round teal buttons matching the brand. Instagram was deliberately left out: Instagram has no web "share this link" button at all (it only supports sharing via its own mobile app to Stories), so a same-looking button for it would have been non-functional. WhatsApp was added instead, since it's a real, working, and widely used sharing channel for this audience.
4. **Every post now has its own branded title-card image** - teal background, the site's topographic line motif, the post's practice-area tag and title set in Fira Sans, plus the firm name and date. These live in `docket/assets/` and are used both as a header image on the post itself, and as the `og:image`/Twitter-card image, so a link shared to LinkedIn, WhatsApp, or anywhere else now renders with a distinct, on-brand image, title, and description - not the generic firm logo it fell back to before.

## What's new in V11.1
A quick follow-up round right after V11 launched, no other changes:

1. **Knowledge-bank section renamed from "Insights" to "The Docket"** (`/insights/` is now `/docket/`), per your feedback that "Insights" was too generic - picked from a shortlist of more distinctive, legal-literate options. Every nav link, page title, meta tag, canonical URL, JSON-LD reference, and the `sitemap.xml` entries were updated to match.
2. **A "Home" link added to the top nav on every Docket page** (the index and all three posts), matching the pattern already used on the DPDP compliance page - so a visitor landing directly on a post from a search result or shared link has an obvious way back to the homepage, not just the logo click.

## What's new in V11
1. **Tagline replaced.** "Strong opinions. Stronger paperwork." (flagged as cringe) is now "Clarity in counsel, precision in execution."
2. **Top nav decluttered.** The redundant "Contact" link (identical destination to the "Get in Touch" button) has been removed from the main nav; footer nav is unchanged.
3. **Practice Areas ring rebuilt from six items to seven genuine practice areas**, replacing two items that weren't actually practice areas (Data Protection and Drafting & Documentation were service/compliance topics, not fields of practice). The ring now reads: Litigation & Dispute Resolution, Corporate & Commercial, Banking & Finance, Mergers & Acquisitions, White Collar Crime & Investigations, Regulatory & Compliance (which now carries DPDP Act advisory as one of its listed services, with the same "Explore DPDP Compliance" link the old Data Protection node had), and Intellectual Property & Trademarks. The ring geometry was recomputed for seven nodes (was six).
4. **New knowledge-bank section launched** (originally named "Insights," renamed to "The Docket" in V11.1 - see above), linked from the main nav on every page. Launched with three seed posts (DPDP Act enforcement timeline, MSME Act Section 18 recovery claims, five vendor-contract clauses founders skip), each Rule-36-safe (general awareness only, no case specifics), with its own OG tags and Article structured data so links render well when shared or crossposted to LinkedIn/Substack. See `claude/isl-insights-workflow-guide.md` in the project for how to add future posts.

## What's new in V10
A Bar Council of India compliance addition, no other changes:

1. **A disclaimer gate now appears on first visit**, on both the homepage and the DPDP compliance page (so a visitor arriving directly at either URL - not just through the homepage - sees it). It states that under BCI rules advocates and law firms may not advertise or solicit work, that the visitor is accessing the site of their own accord, that nothing on the site is legal advice or creates an advocate-client relationship, and that the Firm is not liable for reliance on the site's content - closely modeled on the pattern used by AZB & Partners, Khaitan & Co, and other established Indian firms, researched directly from their live sites before writing this. Content style follows Khaitan's shorter, plain-paragraph format (three paragraphs) rather than a longer bulleted list, per your preference.
2. **Requires an explicit checkbox + click to proceed** - "I have read and understood the above and I wish to proceed," with the "Proceed to Website" button disabled until the box is checked. This is the same gated-popup pattern used by AZB, Khaitan, and other large firms (rather than a passive footer-only disclaimer link), which is the stronger compliance posture under Rule 36.
3. **Remembered permanently once accepted**, via the browser's local storage - a visitor who accepts won't see it again on a later visit from the same browser, only if they clear their browser data.
4. **No copy or layout changes anywhere else** - the rest of the site is identical to V9.

## What's new in V9
A technical SEO pass, no visible design change (except faster-loading logos):

1. **`robots.txt` added**, telling search engines every page can be crawled and pointing them to the sitemap.
2. **`sitemap.xml` added**, listing the homepage and the DPDP compliance page so search engines can discover both without depending purely on internal links.
3. **`CNAME` file added** to the repo root, so GitHub Pages remembers the custom domain (`ivoryslatelegal.com`) even if the repository is ever re-created or re-imported - previously this was only set through the GitHub Pages settings UI, which works but doesn't travel with the repo itself.
4. **Structured data (JSON-LD) added to both pages.** The homepage now carries `LegalService` schema (firm name, phone, email, practice areas, and the three service cities - no street address, matching the site's service-area positioning) and the DPDP page carries `Service` schema referencing that same firm as provider. This is what lets Google show richer results (and understand the firm/service relationship) rather than just a plain blue link.
5. **Logo images converted to WebP with PNG fallback**, cutting their file size by about 95% (from ~330KB down to ~18KB each) using a `<picture>` element - modern browsers get the small WebP file, and any browser that doesn't support it automatically falls back to the original PNG. This improves page-load speed, which is itself a ranking factor.
6. **No copy or layout changes.** Everything visible is identical to V8.

## What's new in V8
An SEO and polish round, no new sections:

1. **Practice Areas is now side-by-side on desktop.** The radial orbit selector sits on the left with its detail panel now next to it on the right, instead of below it — no more scrolling up to pick an area and back down to read about it. Below 900px width the panel drops beneath the ring (a clean stacked layout); below 640px the ring itself flattens into the same tappable button-row fallback as before, unchanged from V7.4.
2. **Browser tab title updated for SEO.** Was "Ivory Slate Legal - Advocates & Legal Consultants, Jaipur" — now **"Ivory Slate Legal | Advocates & Legal Consultants"**, dropping the single-city framing now that the firm spans three cities. Drafted as three options and confirmed with you before writing.
3. **Google's search-result icon addressed.** The generic house icon Google was showing isn't caused by anything wrong in the site's code — the favicon markup and files were already correctly built (multiple icon sizes, valid `.ico` and PNGs). It's most likely Google's own search-result icon cache lagging behind, common for a site that hasn't been (re)crawled recently. As a defensive fix, a copy of the favicon now also sits at the site's root (`/favicon.ico`), since some crawlers check that conventional location regardless of declared `<link>` tags. Once the site is live on the real domain, requesting reindexing via Google Search Console should refresh the icon shown in search results.
4. **Google's search-result description rewritten.** Replaced the old single-city, generic description with one naming the firm's actual practice range and all three cities, drafted as three options and confirmed with you before writing.
5. **Contact section no longer lists a single static office address.** The old Jaipur street address is gone; the location line now simply reads **"Jaipur · Gurugram · Bangalore"**, reflecting the firm's multi-city presence without committing to one office as "the" address.

## What's new in V7.4
The homepage's Practice Areas section has a completely new presentation, per your request for something "outside the box":

1. **Radial orbit selector, replacing the 3x2 grid.** The six practice areas are now arranged as icons in a circle around a center hub (a nod to the rotating orbit graphic already used in the "How We Work" section), with a slow ambient rotation on the outer dashed ring. Click any icon and its full description + bullet list smoothly appears in a detail panel below, with a highlighted spoke connecting it back to the hub. Only one area's full text is showing at a time, but all six are present in the page's HTML (not loaded dynamically), so search engines still index everything.
2. **Data Protection leads the ring** at the top (12 o'clock) and is the practice area shown by default, since it's your actively-marketed differentiator with its own dedicated page. The other five follow clockwise: Litigation & Disputes, Corporate & Commercial, Regulatory Compliance, Drafting & Docs, IP & Trademarks - renumbered 01-06 in that order.
3. **Mobile fallback.** Below 900px width, the ring becomes a simple wrapped row of tappable icon buttons above the same detail panel - the circular layout doesn't hold up on narrow screens, so it drops to a flat, still-interactive layout automatically.
4. All the practice-area copy (descriptions + bullet lists) is unchanged from V7.1/V7.2/V7.3 - this was a presentation change only, drafted as three concept options and confirmed with you before building, per the standing "ask before you write" process for this project.

## What's new in V7.3
Another quick SEO fix, no visible design change:

1. **DPDP page moved to a keyword-rich, extension-free URL.** It used to live at `ivoryslatelegal.com/dpdp.html` - now it's `ivoryslatelegal.com/dpdp-act-data-protection-compliance/`, covering both "DPDP Act" and "data protection compliance" search terms with no file extension in the URL (the modern, cleaner convention). This is done by putting the page's HTML in a folder named `dpdp-act-data-protection-compliance` as `index.html` - your host serves that folder's `index.html` automatically when someone visits the folder's URL, no server configuration needed.
2. **Old `dpdp.html` kept as a redirect.** Anyone who already bookmarked or linked to `ivoryslatelegal.com/dpdp.html` is instantly forwarded to the new URL (both a `<meta refresh>` and a JS redirect, plus a canonical tag), so no existing link breaks and no SEO value is lost in the move.
3. **All internal links updated** - the homepage's "DPDP Compliance" nav links, the practice-card link, and the homepage CTA banner all now point straight to the new URL (not through the redirect).

## What's new in V7.2
Quick SEO fix, no visible design change:

1. **`index.html` links replaced with root-relative links.** Every link on `dpdp.html` that pointed back to the homepage via the literal filename (`index.html`, `index.html#contact`, `index.html#practice`, `index.html#about`) now points to `/` or `/#contact` etc. instead. This avoids `ivoryslatelegal.com` and `ivoryslatelegal.com/index.html` being treated as two separate, duplicate pages by search engines - all authority now consolidates on the bare domain.

## What's new in V7.1
Follow-up round after reviewing V7:

1. **Tagline changed again.** "Counsel that argues your case, not its own importance" read as unprofessional - replaced with **"Strong opinions. Stronger paperwork."**
2. **Est.-panel replacement removed entirely.** The quote-style line ("No associate hands off your matter...") attributed to "The Founding Partners" had the same problem - it's gone, and the hero is back to just the headline, subhead, and CTAs, full width.
3. **Practice-area cards expanded**, both for substance and for search visibility: each of the six cards now carries a fuller description plus a 4-item bullet list naming the specific services and legal terms clients search for (MSME Act Section 18, DPDP Act compliance, trademark registration, etc.) rather than one generic line.
4. **Watermark icons resized.** The background icon in each practice card is now much larger (150px, up from 76px) and far more transparent (8% opacity, down from 15%), moved into the corner as a true watermark so it never competes with the longer text.

## What's new in V7
Homepage feedback from the partners, addressed point by point:

1. **Cities removed from the hero.** The homepage no longer opens with "Jaipur, Gurugram, Bangalore." City names now appear only once, in the address line next to the contact form.
2. **"Est. 2026" replaced**, then removed entirely in V7.1 (see above).
3. **Stat rail redesigned, content and layout both.** The four identical boxes are gone. The rail now leads with a wider, color-blocked panel making the firm's actual differentiator ("Every matter, a partner's own") the headline, with three supporting numbers beside it — Founding Partners, Years Combined Litigation, and Practice Areas (updated from "2 Practice Divisions" to "6 Practice Areas, One Roof" to reflect the expanded practice list in point 5).
4. **Font switched to Fira Sans, sitewide.** Replaces the Cormorant Garamond / Jost pairing on both `index.html` and `dpdp.html`. Space Mono (DPDP page's countdown/mono accents) is untouched.
5. **Homepage diversified beyond DPDP.** Researched several established Indian law firm sites (full-service and IP-boutique) for range. Changes made:
   - Added a sixth practice-area card, **Intellectual Property & Trademarks**, replacing the vaguer "General Advisory." (Descriptions and bullets for all six expanded further in V7.1 - see above.)
   - The "New Practice Wing" DPDP showcase — previously a large two-column block with three of its own stats — is now a single slim banner line. The dedicated DPDP page, its nav link, and its practice-grid card remain; the homepage no longer restates the pitch three separate times.
   - Softened two About-section lines that named DPDP specifically, so they now speak to the firm's range (litigation, corporate advisory, regulatory compliance, IP) with data protection as one growth area, not the throughline.
6. **New tagline**, replaced again in V7.1 (see above).

Everything from V5.1/V6 carries forward unchanged: real contact details, the live Formspree-wired form, no em-dashes, and the DPDP page's cursor-chasing dots and data-flow pipe animations (only its font changed in V7).

## Go live for free — GitHub Pages + your GoDaddy domain

**1. Put the site on GitHub Pages**
1. Create a free GitHub account at github.com if you don't have one.
2. Create a new repository (e.g. `isl-website`), public.
3. Upload the site's files (GitHub's web "Add file → Upload files" works fine, no command line needed) — see "Uploading correctly" below for how to do this without ending up with duplicated or misplaced files.
4. In the repo, go to Settings → Pages. Under "Source," choose the `main` branch and save.
5. GitHub gives you a URL like `https://<yourusername>.github.io/isl-website/` — confirm both pages load there.

**2. Point ivoryslatelegal.com at it**
1. In that same GitHub Pages settings screen, add your custom domain: `ivoryslatelegal.com`, and check "Enforce HTTPS" once it's available.
2. GitHub will show you DNS records to add — typically four `A` records pointing at GitHub's IP addresses, plus a `CNAME` record for `www`.
3. Log into GoDaddy → My Products → DNS for ivoryslatelegal.com, and add those records (edit the existing `A`/`CNAME` records if GoDaddy already has placeholders).
4. DNS changes can take anywhere from a few minutes to 24 hours to propagate. Once it does, ivoryslatelegal.com will load this site directly, with free SSL.

This costs nothing beyond the domain you already own and the Formspree free tier. Cloudflare Pages or Netlify are equally free alternatives to GitHub Pages if you'd rather use one of those — the DNS step with GoDaddy is the same idea either way (they'll give you their own records to add).

## Making future edits
This site is plain HTML files — any text, color, or copy change can be made by editing `index.html` or `dpdp.html` directly (with a text editor, or by asking Claude), then re-uploading to your GitHub repo. GitHub Pages auto-updates within a minute or two of a new upload.

## A note on the self-assessment tools and the Readiness Certification
Under Bar Council of India Rule 36 restrictions on advocate advertising, active lead-generation tools and solicitation mechanisms are a grey area for a law firm website. The free Pulse Check / Deep-Dive tools were deliberately built to collect nothing — no form, no email capture, no data leaves the visitor's browser — to keep them squarely informational. The contact form (wired to Formspree) and the paid Readiness Certification's "Request a Readiness Audit" link are the site's only actual lead-capture points, both housed in the Contact section. The sitewide disclaimer noted as deferred in earlier versions of this README is no longer outstanding — it was built in V10 as a gated entry popup on both the homepage and the DPDP page (see "What's new in V10" above).

## Earlier versions (V1–V6)
The detailed changelog above goes back to V7; before that:
- **V1** — first brand-accurate mockup: teal/cream/ivory palette, topographic line motif, asymmetric layout, scroll-reveal and hover interactions.
- **V2** — added a pointer-repel effect on the background line motif.
- **V3** — added a proper favicon; enlarged and cropped the nav/footer logo; removed redundant wordmark text next to it.
- **V4** — anonymized the "Partners" section to "Leadership" (no names, per the founders' other job commitments); added the dedicated DPDP Act compliance page with its countdown, penalty-exposure cards, and free self-assessment tools.
- **V5** — multi-city positioning (Jaipur, Gurugram, Bangalore); fixed a sitewide icon-rendering bug affecting several card icons; layout fixes to the stat rail and About section; added the paid ISL DPDP Readiness Certification.
- **V5.1** — filled in the real office address, phone number, and a live Formspree-wired contact form; removed all em-dashes from site copy.
- **V6** — added SMIL data-flow "pipe" animations and cursor-attraction dots to the DPDP page.

## Uploading correctly (avoiding duplicate/misplaced files)
This site has files nested inside subfolders — `dpdp-act-data-protection-compliance/`, and as of V11, `docket/` and its three post subfolders. GitHub's web upload only preserves folder structure if you drag a **folder** onto the upload area; if you drag loose files that happen to share a name (several pages are all called `index.html`), GitHub can't tell them apart and will rename the collisions to `index (1).html`, `index (2).html`, etc. at the repo root instead of placing them in the right subfolder.

To avoid this, upload folder-by-folder rather than "select everything and drop it in one go":
1. Drag the `assets` folder in on its own.
2. Drag the `dpdp-act-data-protection-compliance` folder in on its own.
3. Drag the `docket` folder in on its own (this one has its own subfolders inside it — make sure you're dragging the `docket` folder itself, not its contents).
4. Drag the remaining top-level files together: `index.html`, `dpdp.html`, `CNAME`, `robots.txt`, `sitemap.xml`, `README.md`, `favicon.ico`.

After each upload, check the repo's file list shows folders (with a folder icon) rather than a flat pile of numbered duplicates before moving to the next step.
