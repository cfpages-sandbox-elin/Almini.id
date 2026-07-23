# Topical Authority — almini.id

## Role and boundary

`almini.id` should become an Indonesian reference for aluminium as a material and as a building-product system: terminology, alloys and tempers, product forms, specification, fabrication, finishes, durability, structural limits, façades, openings, canopies, interiors, building physics, installation, maintenance, K3, and recycling. It serves homeowners and buyers as well as architects, engineers, façade consultants, fabricators, installers, facility teams, and procurement staff. Indonesia-specific conditions include heat, high rainfall and humidity, marine exposure, workmanship variability, retrofit constraints, and traceable procurement.

“Almini” is the owner-confirmed project term for aluminium and is also observed as Indonesian market vernacular for aluminium products. It is not presented as the formal material designation: technical pages use **aluminium**, state alloy/temper/product form where relevant, and treat “almini” as a search and vocabulary bridge.

The knowledge layer is educational. `/jasa/` and its child routes own quotation, capability, service area, warranty, and portfolio intent. `/produk/` and its child routes own stock, dimensions actually supplied, commercial availability, and product enquiries. Articles may support those routes contextually but must not combine neutral guidance with an undisclosed sales pitch. Structural sizing, façade engineering, fire classification, live electrical work, welding-procedure approval, work-at-height planning, regulated inspection, and acceptance of safety-critical work remain competent-professional tasks.

Other owned domains may independently cover façades, ACP, glass, welding, cutting, safety, fire, lighting, steel, partitions, or recycling. That is cross-domain opportunity, not cannibalization. The anti-cannibalization controls here apply only within `almini.id`.

## Evidence audited

Audit date: 2026-07-23. Repository evidence was inspected on clean `main`, tracking `origin/main`.

| Evidence | Observed count/finding | Planning implication |
|---|---:|---|
| Tracked repository files | 9,290 | Static WordPress export with substantial bundled theme/plugin assets rather than a source-driven article collection |
| Sitemap families | 19 XML files | `sitemap.xml` and `sitemap_index.xml` each reference 15 post sitemaps plus one page sitemap; `sitemap-complete.xml` is a separate generated inventory |
| Canonical sitemap rows | 2,987 rows in post plus page sitemaps; 2,979 exact unique | Eight exact URL duplicates occur across post sitemap files and should be removed |
| Generated complete sitemap | 3,071 exact unique URLs | Includes archives and technical template routes that should not be treated as editorial coverage |
| Geography-template pages | 2,964 local root HTML files | Six service/product stems multiplied across 494 place labels each; no location-swapped briefs are added |
| Geography families | 494 each for ACP/curtain wall, canopies, kitchen sets, frames/doors/partitions, general aluminium products, and shower boxes | Consolidate around national intent owners unless real local evidence supports a distinct page |
| Service and product routes | 17 sitemap pages | `/jasa/` plus eight service children; `/produk/` plus seven product children |
| Informational articles | 0 substantive standalone articles observed | `/berita/` contains a listing and 24 pagination pages, not an evidence-rich article corpus |
| Archive/pagination routes | 80 in `sitemap-complete.xml` | 30 category, 26 author, and 24 news listing/pagination URLs are navigation utilities, not authority depth |
| Static/technical sitemap routes | 9 additional routes beyond home, commercial pages, and archives | Contact/about/portfolio may remain; form, Elementor template, and author routes require indexation review |
| Duplicate place-name suffixes | 30 root files ending `-2.html` | Five ambiguous place labels appear twice in every geography family and need city/regency disambiguation before any retention decision |
| Crawl controls | `robots.txt` exists; no `_redirects`, `_headers`, or local 404 page | Canonical/redirect behavior must be designed and verified at deployment, not inferred from the export |
| Canonicals sampled | Relative self-canonicals on home and geography pages | Self-canonicals do not resolve thin template families or duplicate place intent |
| Terminology evidence | Portfolio registry explicitly confirms `almini.id` means aluminium; independent Indonesian commerce and recycling usage also maps “almini” to aluminium | Use the colloquial term as discovery vocabulary, but use formal material terminology in technical specifications |

The sitemap counts come from parsing URL entries rather than counting image locations. The eight exact duplicates in post sitemaps are `kitchen-set-aluminium-pegunungan-bintang.html`, `produk-aluminium-luwu-timur.html`, `kusen-pintu-partisi-aluminium-humbang-hasundutan.html`, `shower-box-yogyakarta.html`, `shower-box-buleleng.html`, `acp-curtain-wall-luwu-utara.html`, `kusen-pintu-partisi-aluminium-raja-ampat.html`, and `acp-curtain-wall-madiun.html`.

Terminology verification is deliberately narrow: examples of “almini” used for aluminium appear in an [Indonesian community-recycling paper](https://ejurnal.uwp.ac.id/lppm/index.php/semanggi/article/download/2/55/446) and Indonesian product listings, while the project owner explicitly defines the domain that way. Drafts must not state that “almini” is a formal alloy name, grade, or universally accepted spelling.

## Existing coverage and risks

| Existing URL/pattern | Observed role/problem | Decision | Destination/owner | Verification needed |
|---|---|---|---|---|
| `/` | Broad national supplier/service homepage | keep | Homepage and ALM-01-A01 knowledge hub | Clarify navigation between neutral education and commercial offers |
| `/jasa/` and eight child routes | Legitimate commercial taxonomy for ACP, curtain wall, canopies, kitchens, frames, partitions, openings, and showers | keep | Existing commercial routes | Verify current capability, service scope, proof, warranty, and response codes |
| `/produk/` and seven child routes | Commercial taxonomy for ACP, accessories, hollow, honeycomb, plate, profiles, and spandrel | keep | Existing product routes | Verify stocked forms, actual specifications, manufacturer evidence, and availability |
| `{acp-curtain-wall,kanopi-aluminium,kitchen-set-aluminium,kusen-pintu-partisi-aluminium,produk-aluminium,shower-box}-{place}.html` | 2,964 location-swapped pages with national template intent | manual review | Corresponding national service/product hub; retain a local route only when real local proof changes substance | GSC queries/clicks, backlinks, leads, unique photos/projects, staffed service area, logistics, legal locality, and redirect target |
| Thirty `*-2.html` geography pages | Ambiguous duplicate location labels across six template families | merge | Explicit city/regency owner or national hub | Map each label to the intended administrative area and compare equity before redirect |
| `/berita/` plus `/berita/page/2/` through `/page/25/` | Empty/thin listing footprint without substantive article routes | noindex | Future `/artikel/` hub or a rebuilt `/berita/` hub | Confirm live pagination, canonical tags, internal links, and whether any indexed history exists |
| `/category/**` | Six category families with pagination, largely mirroring template posts | noindex | Navigation only | Confirm no unique category demand or useful backlinks before changing indexation |
| `/author/admin/**` and `/author/lixusicava6312/` | Thin author archives; unexpected second author identifier | noindex | Real editorial author/profile route if created | Security/editorial review of author identity, live exposure, and links |
| `/form/simple-contact-form/` and `/elementor-hf/**` | Technical/form/template routes included by generated sitemap | remove | None; exclude from sitemaps | Verify whether live routes return indexable HTML and whether forms rely on them |
| `/merk/` | Brand listing/commercial support route | expand | Existing commercial brand route | Require actual brand relationships, current manufacturer documentation, and neutral disclosure |
| `sitemap-complete.xml` versus Rank Math sitemap index | Parallel manifests with different inclusion policies | canonicalize | One canonical sitemap index | Confirm deployed sitemap submitted to search engines and remove archives/technical URLs |
| Sitemap generation workflows | Workflow can inventory every HTML file and turn static/technical pages into sitemap URLs | manual review | Controlled route allowlist | Test workflow output in a branch before any production run |
| Relative canonicals plus absent redirect map | `.html`, extensionless, and trailing-slash behavior may diverge | manual review | One URL convention | Crawl live responses, canonical tags, internal links, and GSC-selected canonicals |

Primary risks are mass doorway-like geography, sitemap inflation, same-template commercial intent, weak technical evidence, conflation of aluminium grades, unsafe structural/fire/electrical advice, and publication volume replacing quality. This catalog is a planning system, not authorization to generate 78 pages automatically.

## Coverage matrix

| Completeness lens | Topic owner(s) | Coverage decision |
|---|---|---|
| Definition, Indonesian vocabulary, history, mechanisms, basic properties | ALM-01 | “Almini” is a vocabulary bridge; formal technical terms govern specification |
| Taxonomy, alloys, tempers, forms, dimensions, tolerances, certificates | ALM-01, ALM-02 | Separate material identity from purchasable product form and verification |
| Need, survey, requirements, comparison, budget, procurement | ALM-02, ALM-05–ALM-09 | Decision tables avoid invented prices and universal product rankings |
| Cutting, machining, forming, joining, welding, fabrication QC | ALM-03 | Procedures require manufacturer/WPS/equipment limits and competent review |
| Anodizing, coating, appearance, corrosion, galvanic and electrical contact | ALM-04 | Treat finish, environment, dissimilar-metal contact, and current-carrying joints as distinct decisions |
| Structural use, load path, stiffness, connections, anchorage, retrofit | ALM-05 | Engineering gate applies whenever failure can injure people or damage the building |
| ACP, curtain wall, honeycomb, spandrel, drainage, movement, façade fire | ALM-06 | System evidence outranks generic material claims |
| Frames, doors, windows, partitions, glazing, hardware | ALM-07 | Commercial routes retain quotation intent; articles own selection and diagnosis |
| Canopies, roofs, gutters, outdoor and coastal exposure | ALM-08 | Climate changes substance; city-name swapping does not |
| Kitchens, shower boxes, cabinetry, wet interiors, hygiene | ALM-09 | Separate cabinet/system decisions from glazing and waterproofing responsibilities |
| Thermal, condensation, acoustic, expansion, fire and high-temperature behavior | ALM-10 | Exact performance claims require assembly test/classification evidence |
| Installation, commissioning, handover, inspection, maintenance, defects, repair, replacement | ALM-11 | Lifecycle path links diagnosis to prevention and repair-versus-replace decisions |
| Workshop/site K3, hot work, chemicals, heights, lifting, electrical tools, emergencies | ALM-12 | Controls hierarchy and stop conditions; no article substitutes for site authorization |
| Recycling, scrap, recycled content, disassembly, embodied impact, circular procurement | ALM-13 | Environmental claims require declared boundaries and traceable data |
| Stakeholder paths | ALM-02, ALM-05–ALM-13 | Buyer, architect, engineer, fabricator, installer, facility team, and recycler each receive a coherent path |
| Building/site types and scale | ALM-05–ALM-10 | Residential, commercial, high-rise, occupied retrofit, wet area, and exposed outdoor uses are separated |
| New build versus retrofit | ALM-05, ALM-07, ALM-11 | Existing substrate, access, unknown materials, and occupied-site risk are explicit |
| DIY versus professional | ALM-03–ALM-12 | Low-risk inspection/cleaning may be described; structural, façade, fire, live electrical, welding, and work-at-height tasks have professional gates |
| Standards and regulation | ALM-02–ALM-13 | Verify current BSN/SNI, project code, authority, contract, test report, and manufacturer instructions before naming clauses |
| Failure modes and myths | ALM-04–ALM-12 | Correct “aluminium never corrodes,” “light means weak,” “ACP is one product,” and appearance-only acceptance |
| Calculation, checklist, visual reference, case study | ALM-01–ALM-13 | Calculators declare assumptions; case studies require real records and consent |
| News/trends | N/A | No maintainable news desk exists; durable changes belong in evergreen pages with review dates |

## Topical map

| Topic ID | Parent topic | Reader outcome | Required subtopics/questions | Evidence/formats | Boundary | Article target |
|---|---|---|---|---|---|---:|
| ALM-01 | Aluminium fundamentals, alloys, tempers, and properties | Use correct terminology and understand which material identity controls performance | Almini/aluminium/alumunium terms; element versus alloy; alloy families; wrought versus cast; temper; density; stiffness; strength; conductivity; oxide layer; recyclability; units and certificates | Terminology map, property diagrams, alloy/temper decision table, primary standards, metallurgist review | Does not select a purchasable section or supplier; ALM-02 owns form/specification and `/produk/` owns commercial availability | 6 |
| ALM-02 | Product forms, specification, measurement, and procurement | Convert a requirement into a verifiable aluminium purchase specification | Extrusions/profiles; plate/sheet; hollow/tube; ACP; honeycomb; spandrel; accessories; dimensions; thickness; tolerances; certificates; sampling; supplier comparison; substitutions; storage | Annotated product anatomy, measurement checklist, certificate guide, quote matrix, manufacturer data | Does not teach fabrication or promise stock/price; ALM-03 owns processing and `/produk/` owns availability | 6 |
| ALM-03 | Fabrication, forming, machining, joining, and workshop quality | Choose and control a fabrication route without normalizing unsafe shortcuts | Sawing; routing; drilling; CNC; burrs; bend radius; springback; fixtures; welding; mechanical fastening; adhesives; sealants; dimensional inspection; traceability; rework | Process map, tool/manufacturer limits, WPS gate, inspection plan, original workshop photos, qualified review | No universal machine settings, structural joint approval, or DIY production welding; ALM-05 owns structural adequacy and ALM-12 owns K3 | 6 |
| ALM-04 | Finishes, corrosion, dissimilar metals, and electrical contact | Preserve appearance and function by controlling surface and interface risks | Natural oxide; pitting/crevice/galvanic corrosion; marine/polluted exposure; drainage; anodizing; powder coating; liquid coating; pretreatment; finish defects; copper/steel contact; current-carrying terminals; cleaning | Corrosion diagrams, exposure/finish matrix, coating data, electrical manufacturer instructions, field photos, specialist review | Does not authorize live electrical work or guarantee finish life; ALM-12 owns electrical K3 and ALM-11 owns maintenance/repair | 6 |
| ALM-05 | Structural use, design responsibility, connections, and retrofit | Recognize when aluminium can be structural and what evidence engineering must provide | Load paths; strength versus stiffness; buckling; deflection; alloy/temper after fabrication; connection behavior; anchors; fatigue; thermal movement; robustness; temporary works; retrofit substrate; inspection and acceptance | Engineer-reviewed diagrams, calculation assumptions, project standards, test/certificate matrix, ITP | No member sizing, anchor schedule, load rating, or approval for a live project; a competent engineer owns project decisions | 6 |
| ALM-06 | Façades, ACP, curtain walls, honeycomb, and spandrel systems | Select and evaluate aluminium façade assemblies as systems rather than isolated panels | Rainscreen versus curtain wall; ACP/solid/honeycomb/spandrel distinctions; brackets/rails; glazing; drainage; pressure equalization; wind; water; movement; sealants; fire evidence; mockups; installation QC; failures | System sections, decision table, project calculations, accredited test reports, manufacturer manuals, façade/fire expert review | `/jasa/acp/` and `/jasa/curtain-wall/` own quotations; ALM-10 owns general fire/thermal principles and ALM-05 owns structural approval | 6 |
| ALM-07 | Frames, doors, windows, partitions, glazing, and hardware | Specify openings and partitions that operate, drain, seal, and remain maintainable | System selection; profile chambers; glass interface; gaskets; sealants; fasteners; hardware; air/water; drainage; tolerances; retrofit survey; operation; condensation; leaks; rattles; replacement | Annotated sections, survey checklist, performance/test matrix, original defect photos, installation expert review | Existing `/jasa/kusen/`, `/jasa/pintu-jendela/`, and `/jasa/partisi-kaca/` own sales; ALM-09 owns cabinets/showers | 6 |
| ALM-08 | Canopies, roofs, gutters, and exposed outdoor aluminium | Choose and maintain an outdoor system for rain, wind, heat, drainage, and corrosion exposure | Covering versus frame; spans/load paths; slope; gutters/downpipes; ponding; wind uplift; thermal movement; sealants; anchors; coast; lightning/electrical interfaces; cleaning; storm inspection | Section diagrams, rainfall/drainage inputs, engineer review, corrosion matrix, inspection checklist | `/jasa/kanopi/` owns quotation; no universal span, slope, anchor, or drainage capacity is provided | 6 |
| ALM-09 | Kitchens, shower boxes, cabinetry, and wet interiors | Select interior aluminium systems around water, hygiene, glazing, hardware, and serviceability | Cabinet carcass/fronts; countertops/interfaces; food-area cleaning; wet-area corrosion; shower glass; water containment; sealants; ventilation; hardware; sharp edges; accessibility; repair | Detail drawings, cleaning matrix, waterproofing responsibility map, original photos, glazing/interior expert review | `/jasa/kitchen-set/` and `/jasa/shower-box/` own commercial intent; waterproofing and structural glass design require their respective specialists | 6 |
| ALM-10 | Thermal, moisture, acoustic, fire, and high-temperature behavior | Interpret assembly performance claims without treating aluminium alone as the whole building system | Conductivity; thermal bridges; condensation; expansion; solar heat; acoustic paths; melting/softening concepts; combustibility versus fire resistance; coatings/cores/sealants; smoke/toxicity evidence; test scope and classification | Building-physics diagrams, psychrometric explanation, accredited assembly reports, fire engineer review, evidence hierarchy | No fire rating or acoustic/thermal value is inferred from appearance or base metal alone; ALM-06 owns façade-specific evidence | 6 |
| ALM-11 | Installation, handover, maintenance, diagnosis, repair, and replacement | Manage the installed asset from delivery through end-of-life decisions | Receiving/storage; substrate survey; tolerances; protection; hold points; sealants/fasteners; commissioning; as-builts; warranties; cleaning; inspection; leaks; corrosion; loose joints; distortion; repair versus replace | ITP, handover checklist, symptom decision tree, field measurement, manufacturer maintenance data, expert review | Does not provide DIY structural/façade repair or override warranty terms; ALM-05 owns structural approval and ALM-12 owns hazardous access | 6 |
| ALM-12 | K3 for aluminium workshops and site installation | Recognize hazards, apply the controls hierarchy, and know when work must stop | Sharp edges; chips/dust; noise; rotating tools; manual handling; lifting; welding fumes/arc; hot work; coatings/solvents; electrical tools; heights; dropped objects; housekeeping; fire; emergency response | Current Indonesian K3 sources, SDS, task-risk checklist, permit workflow, competent K3 and trade review | Not a substitute for risk assessment, permit, training, supervision, rescue plan, electrical authorization, or medical advice | 6 |
| ALM-13 | Recycling, circular design, and environmental evidence | Make credible lifecycle and recovery decisions from procurement through scrap | Primary versus recycled input; embodied-impact boundaries; production scrap; alloy segregation; coating/adhesive contamination; recycled-content evidence; design for disassembly; reuse; transport; recycler chain; environmental claims | Lifecycle-boundary diagram, mass-balance worksheet, supplier declarations, recycler evidence, comparative assessment | Does not claim infinite recycling, guaranteed carbon savings, or regulatory compliance without traceable project-specific evidence | 6 |

Total planned articles: **78**.

## Related-domain opportunities

| Domain/topic context | Useful collaboration | Independence rule |
|---|---|---|
| `fasad.co.id`, ACP, glass, and curtain-wall properties | Share terminology for envelope layers, drainage, sealants, test evidence, and defect photography | `almini.id` retains aluminium-material and aluminium-system treatment; no topic is suppressed because another domain covers façades |
| Welding, cutting, fabrication, and workshop properties | Cross-reference process capability, measurement, joining, and K3 where a reader needs deeper trade guidance | Links must be contextual; ALM-03 remains the aluminium-specific fabrication owner |
| `safety.co.id` and `firesafety.co.id` | Provide deeper controls, emergency planning, and fire-system context | ALM-10 and ALM-12 retain aluminium-specific evidence boundaries and stop conditions |
| Glass, partitions, roofs, lighting, steel, and electrical-adjacent sites | Explain material interfaces, galvanic isolation, glazing, anchorage, or lightning/electrical coordination | Same owner across domains does not make independent editorial coverage cannibalization |
| Recycling and materials properties | Share evidence vocabulary for recycled content, scrap segregation, and end-of-life | Avoid sitewide reciprocal networks or mechanically repeated cross-domain links |

## Consolidation plan

1. Freeze generation of new place-swapped pages while live response, GSC, backlink, lead, and locality evidence is collected.
2. Select one national intent owner for each of the six geography families: the relevant `/jasa/` or `/produk/` hub, not a new article.
3. Retain a local page only when it contains a real service area, staffed fulfilment route, unique project/logistics evidence, local constraint, and measurable value. Location names alone are insufficient.
4. Merge ambiguous `-2` place routes after mapping city versus regency intent; preserve the stronger URL where evidence exists and redirect the other.
5. Remove exact duplicate entries across post sitemaps and converge on one allowlisted sitemap index that excludes author, archive pagination, form, and Elementor template routes.
6. Rebuild `/berita/` as an article hub or create `/artikel/`, then noindex thin pagination until enough real editorial assets justify crawlable archives.
7. Preserve commercial service/product URLs. Expand them with auditable scope, materials, process, proof, exclusions, and warranty rather than turning knowledge articles into sales pages.
8. Publish the first bounded cluster only after templates support author/reviewer, sources, review dates, disclosure, breadcrumbs, related links, and schema appropriate to the real content.

No redirect or deletion should be executed from this plan alone. Historical value, live behavior, canonical selection, and deployment constraints must be checked first.

## Internal-link architecture

- `/artikel/aluminium-dan-almini/` is the central beginner hub and links to all thirteen parent hubs.
- Every article links upward to its parent topic hub; each hub links to all six child assets and to only the adjacent hubs required for the reader’s next decision.
- ALM-01 vocabulary and property pages lead to ALM-02 specification, ALM-04 durability, ALM-05 structural limits, and ALM-13 lifecycle evidence.
- ALM-02 purchase/specification pages lead to ALM-03 fabrication, application hubs ALM-06–ALM-09, and relevant `/produk/` routes only when actual commercial data supports the link.
- Application comparison pages link to material/finish evidence, engineering gates, installation control, diagnosis, and the matching `/jasa/` route; commercial links are not copied sitewide.
- Diagnostic pages in ALM-04, ALM-06–ALM-11 link to prevention, safe isolation, inspection, repair-versus-replace, and professional escalation.
- Fire, structural, electrical-contact, welding, chemical, lifting, and height-related pages link visibly to their evidence limitations and ALM-12 stop conditions.
- ALM-13 links backward to alloy identification, finish compatibility, disassembly, maintenance, and procurement evidence so recycling is not isolated as a marketing appendix.
- Archives, author pages, and pagination do not substitute for hub links; no planned article is orphaned.

## Evidence and editorial standards

1. Use a claim hierarchy: current Indonesian law/regulator and BSN/SNI records where applicable; adopted project code/specification; accredited test/classification; engineering calculation; mill/test certificate; manufacturer technical data and installation instructions; qualified expert review; then clearly labelled field observation.
2. Verify the current edition, applicability, authority, contractual adoption, test specimen, orientation, support condition, joints, fixings, finish, and limitations before quoting any standard number, classification, load, fire rating, or acceptance criterion.
3. **Structural gate:** no span, load, member, anchor, connection, deflection, buckling, fatigue, or retrofit conclusion without project inputs and competent engineering approval. Do not infer safety from alloy strength alone.
4. **Alloy/temper gate:** never use “aluminium” as a complete specification. State form, alloy, temper, dimensions/tolerances, finish, certificate requirement, and any property changes caused by heat or fabrication.
5. **Corrosion/electrical-contact gate:** distinguish atmospheric, crevice, pitting, and galvanic mechanisms. Current-carrying aluminium-to-copper/terminal advice must follow equipment manufacturer instructions and authorized electrical design; never recommend improvised joint compounds or live work.
6. **Fire gate:** distinguish noncombustible base metal, strength loss with temperature, melting, coating/core/sealant behavior, smoke/toxicity, and assembly fire resistance. Only the tested/classified assembly within its scope may carry a rating.
7. **Façade gate:** require system drawings, wind/water/thermal movement inputs, drainage, interfaces, mockup/test evidence where applicable, installation ITP, and qualified façade/structural/fire review.
8. **Fabrication gate:** no universal cutting, bending, welding, adhesive, cure, or torque recipe. Use machine/tool limits, alloy/temper, WPS or approved procedure, consumable data, environmental conditions, inspection, and traceability.
9. **Finish gate:** require substrate/alloy, pretreatment, coating/anodizing system, exposure, thickness/class where applicable, color/gloss/tolerance, cut-edge/joint details, maintenance, and supplier evidence.
10. **K3 gate:** procedural content includes prerequisites, hazards, controls hierarchy, PPE limits, stop conditions, competence/permit requirements, emergency response, and verification. SDS and site risk assessment control chemical work.
11. **Recycling gate:** declare system boundary, data period/geography, primary versus recycled content, allocation method, recovery losses, contamination, transport, and evidence owner. Avoid “100% recyclable” as a proxy for actual recovery.
12. Prices, case studies, test results, warranties, project photographs, and firsthand experience must not be invented. A case study requires real records, permission, constraints, method, result, and limitations.
13. Every article carries author, qualified reviewer where needed, sources, publication/review dates, assumptions, disclosure of commercial interest, and a scheduled evidence review.

## First bounded publication cluster

Publish these **12 P0 assets** as one connected evidence cluster:

1. ALM-01-A01 — aluminium/almini terminology and central navigation.
2. ALM-01-A02 — alloy and temper decision foundation.
3. ALM-02-A01 — product-form identification.
4. ALM-02-A03 — material specification checklist.
5. ALM-03-A01 — controlled fabrication workflow.
6. ALM-04-A01 — corrosion mechanism and prevention.
7. ALM-05-A01 — structural-use engineering gate.
8. ALM-06-A01 — façade panel/system comparison.
9. ALM-07-A01 — opening-system selection.
10. ALM-10-A04 — aluminium and fire evidence.
11. ALM-11-A01 — installed-system symptom triage.
12. ALM-12-A01 — workshop/site K3 control hierarchy.

The cluster moves from vocabulary and material identity to purchase, processing, high-cost applications, failure prevention, and safety. Each page links upward to its hub and laterally only to the next decision or stop condition.

Monitor: valid indexation and selected canonicals; impressions and clicks grouped by intent rather than page count; engagement with diagrams/checklists and navigation to the next task; qualified product/service enquiries with source page; evidence-review completion; and query/page overlap in GSC. Review at 30, 60, and 90 days. Ranking alone is not success, and evidence of cannibalization pauses expansion until boundaries are corrected.

## Definition of done

- All 13 parent topics have exactly six distinct catalog briefs and no location-swap exceptions.
- IDs, titles, slugs, intents, evidence formats, priorities, waves, and related IDs pass the skill validator.
- Planned slugs do not collide with existing repository routes or with each other.
- Repeated stems are resolved in the same-domain anti-cannibalization register.
- Existing commercial, geography, archive, author, form, template, and sitemap routes have an explicit evidence-dependent decision.
- Structural, alloy/temper, corrosion, electrical-contact, fire, façade, fabrication, finish, K3, and recycling gates are present in briefs and editorial review.
- The first wave is limited to 12 connected assets and is reviewed before later waves.
- Every published page has sources, ownership, reviewer where required, disclosure, review date, hub link, contextual related links, and no invented claims.
- Consolidation is implemented only after live response, GSC, backlink, lead, and deployment verification.
