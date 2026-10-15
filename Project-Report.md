---
title: Project Report – Building the OC Local Resources Knowledge Base
type: project-report
region: Orange County, CA
report_date: 2026-10-05
tags: [project-report, methodology, orange-county]
---

# Project Report: Building the OC Local Resources Knowledge Base

**Report date:** October 5, 2026
**Work period:** October 3–5, 2026
**Repository:** https://github.com/xunman0/OC-Local-Resources

## Summary
This project built a plain-language knowledge base of free food, diaper, and community resources in Orange County, California. It is written in Markdown for Obsidian and organized so an AI assistant can give accurate, specific answers to the general public.

In three days, the work turned four source lists and dozens of web checks into **443 resource entries** across 47 files. Every entry names its source. Conflicts between sources are shown, not hidden. About **65 entries** were checked against the organization's own website or corrected.

| Section | Files | Entries |
|---|---|---|
| Food pantries by city (`03-Pantries-by-City`) | 33 city files + index | 294 sites |
| Diaper resources (`08-Diaper-Banks`) | 1 | 30 sites |
| Community resources (`10-Community-Resources`) | 12 category files + index | 119 organizations |
| **Total** | **47** | **443** |

## Goals
1. Help Orange County residents find free food, diapers, and other help quickly and accurately.
2. Make the content easy for an AI assistant to search and quote correctly.
3. Be honest about uncertainty: show sources and dates, flag conflicts, and tell people to call before going.
4. Keep the content easy to update as source lists change.

## Sources Used

| Source | Date | Used for |
|---|---|---|
| Second Harvest Food Bank of Orange County partner list (PDF, 21 pages) | As of 09/14/2026 | Main food pantry data: 289 sites in 33 cities |
| City of Westminster FRC "Local Food Pantries" flyer (PDF, 3 pages) | File created 10/29/2025 | Phone numbers and requirements for 16 sites; 3 new sites |
| CAP OC Diaper Bank partner list (capoc.org) | Read 10/03/2026 | 29 diaper partners |
| Community resources spreadsheet (recreation of the RCOC community resources list) | 2026 | 106 community organizations |
| Legal Resources list (Orange County and surrounding area) | 2026 | 15 legal and immigration organizations |
| Organization websites (checked in the browser) | 10/03–10/05/2026 | Verifying hours, addresses, phones, and status |
| Information confirmed by the project owner | 10/03–10/05/2026 | Hours, contacts, and closures for specific sites |

## How the Knowledge Base Is Organized

| Folder | Contents |
|---|---|
| `00-Overview` | Scope, glossary, writing rules, sources, AI guidance, and this report |
| `03-Pantries-by-City` | One file per city. Sites grouped as community pantries, school sites, Senior Grocery, Park-it Markets, and kids meal sites |
| `08-Diaper-Banks` | Diaper distributions, mostly through CAP OC partners |
| `10-Community-Resources` | 12 topics: legal aid, immigration, disability, benefits, healthcare, mental health and crisis, housing, children and education, family resource centers, seniors, transportation, general help |
| `99-Sources-and-Verification` | Internal only (not published): verification tracker and source flag logs |

### What every entry includes
- Name, address, phone, email, and website where available
- Days and hours written in plain language (for example, "1st & 3rd Saturdays of the month")
- **Who can use it**, including notes like "may be for residents only" or "children enrolled in the program"
- **Before you go**, telling people to call ahead and who to call
- Source and date

### Design choices for AI retrieval
- **One topic per file** and one heading per site, so search tools find small, complete pieces.
- **YAML frontmatter** on every file (title, type, city, ZIP codes, sources, dates, tags).
- **Plain-language schedules** instead of shorthand like "2nd/4th".
- **Quick summaries** at the top of each city file: days open, weekend options, evening options.
- **"Call before you go" banners** on every file.
- **Cross-links** between related entries (for example, a family resource center that also hosts a food distribution).

## Work Completed

### Phase 1: Food pantries (October 3)
- Planned the folder structure, overview, and city file template.
- Extracted the 21-page Second Harvest PDF with a script. Built 33 city files with 289 sites and 534 distribution times.
- Logged about 20 likely errors in the source (AM/PM typos, ZIP mismatches, outdated closure dates).

### Phase 2: Second source merged (October 3)
- Merged the Westminster FRC flyer: phone numbers and requirements added to 13 matching sites; 3 new sites added.
- Matched sites listed under different names by address (for example, "Cantlay Food Distribution Center" = Catholic Charities).
- Logged 9 hours conflicts between the two sources.

### Phase 3: Diaper resources (October 3)
- Created the diaper folder from the 3 diaper mentions in the food lists.
- Expanded it to 30 sites using the CAP OC Diaper Bank partner list, read in the browser.

### Phase 4: Public readiness (October 3)
- Reviewed what was safe and appropriate to publish.
- Added "Who can use it" and "Before you go" notes to every site.
- Flagged 25 sites at apartment or housing communities as "may be for residents only."
- Kept internal working files out of the public repository.

### Phase 5: GitHub publishing (October 3)
- Published to a public GitHub repository.
- Added a README and a `.gitignore` that keeps internal files from being uploaded.
- Checked each upload against the local files.

### Phase 6: Food pantry verification (October 3–4)
- Built a verification tracker grouping open items by who to contact.
- Checked 18 sites on their own websites in the browser.
- The project owner confirmed or supplied details for 11 more items.
- Added official website links to 24 food sites and 6 diaper partners.

### Phase 7: Community resources (October 4–5)
- Converted the community spreadsheet and legal list into 12 topic files.
- Regrouped 20 source categories into 12 clearer topics. Combined duplicates and moved miscategorized entries.
- Three rounds of browser checks covered about 20 flagged items.
- Added 6 current FaCT family resource centers and removed 3 entries that had closed or were removed.

## Key Corrections Found
These are examples of errors in the source lists that could have sent someone to the wrong place or time:

| Site | Problem in source | Correction |
|---|---|---|
| Gilbert High – El Mercadito (Anaheim) | Address was Ball Junior High's | 1800 W. Ball Rd., Room 44 |
| Heart of the City (Los Alamitos) | 8:00–10:30 AM | 7:00–9:30 AM |
| Fullerton Community Center Senior Grocery | 1st & 3rd Thursdays, 10–11 AM | 1st, 2nd & 3rd Thursdays, 10:30 AM–12 PM |
| 3 kids meal and school sites | Times listed as AM instead of PM | Changed to PM |
| Mariners Church – Santa Ana | Flyer said Tuesday–Friday | Saturday 9–11 AM; flyer hours belonged to Mariners Irvine |
| Southlands Church (Brea) | "Every 4th Saturday" | Dates vary; check the church calendar |
| Medi-Cal Dental | Phone and website were HICAP's | 800-322-6384, smilecalifornia.org |
| Sensory Impaired Guidance Network | Listed under old name, P.O. box as address | Renamed; entry says to call for visit location |
| 3 sites | Wrong ZIP codes | Corrected |

Notable findings:
- **Serve The People's 4:00 AM start looked like a typo but is real.**
- **Hope Lutheran's "1st Friday" listing was incomplete, not wrong.** The pantry runs every Friday; the 1st Friday is when Second Harvest produce arrives.

## Decisions and Policies
These rules were set during the project and apply to all future updates:

1. **Second Harvest partner sites:** Direct people to Second Harvest Food Bank of Orange County (949-653-2900, info@feedoc.org) for the latest schedule. For **school sites**, contact Second Harvest instead of the school.
2. **CAP OC diaper partners:** Direct people to CAP OC (714-897-6670, info@capoc.org) for the latest partner list.
3. **Contacts:** Use main or office numbers only, never individual staff names or personal emails.
4. **Conflicting sources:** Show the newer source first, keep the other version below, and mark it as a conflict until it is resolved.
5. **Corrections:** Keep the original value visible ("corrected from …") so anyone can compare against the source.
6. **Closed organizations are removed**, not left with a warning. Removed: Church World Service Orange County (office closed), La Habra Family Resource Center (closed due to funding), and Anaheim Harbor Family Resource Center.
7. **Internal working files stay private** and out of the public repository.
8. **Crisis safety:** The crisis line entry includes 988, the Suicide & Crisis Lifeline.

## Verification Status
| Area | Checked or corrected | Still open |
|---|---|---|
| Food pantries | 25 sites with a verification section; 3 typo corrections; 24 website links | 3 phone calls; 22 possible residents-only sites; 7 corrections to report to Second Harvest |
| Diaper resources | 6 partners checked | Addresses for 14 partners; direct numbers for 5 WIC offices; diaper sizes and limits |
| Community resources | About 30 entries fixed; 6 FRCs added; 3 removed | Missing emails (minor) |

Most of the 294 food sites still rely on the Second Harvest list alone. That list is the most current source available, and each entry tells people to call before going.

## Open Items and Next Steps
1. **Email Second Harvest** with 1 question (which residents-only sites are open to the public) and 7 corrections to report.
2. **Call 3 sites:** Delhi Center (Monday or Thursday?), His Place (Friday and Sunday distributions?), and Abrazar (food times).
3. **Contact CAP OC** for missing diaper partner addresses, WIC numbers, and diaper limits.
4. **Build the missing folders** linked from every city file: `01-How-to-Get-Food-Now` and `05-Benefit-Programs`. Also planned: food banks, special populations, hot meals and mobile pantries, and referral lines.
5. **Fill coverage gaps** in cities with few or no listed sites.
6. **Set an update schedule.** Second Harvest updates its list regularly; dated items (like Fullerton's 2026 Senior Grocery dates and Southlands' calendar dates) will go stale.

## How to Maintain This Knowledge Base
- When a new source list arrives, add it as a new source, merge by address, and log conflicts in `99-Sources-and-Verification`.
- When verifying a site, record the date and source in the entry's ✅ section.
- Keep the "Call before you go" banners and "Before you go" lines on every entry.
- Re-check the repository after each upload to confirm it matches the local files.
