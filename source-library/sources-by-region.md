# Source Library
*Tracked sources by region and type. Updated as source performance is observed over time.*
*Note: source quality assessment accumulates here — which outlets were ahead of the curve, which were noise.*

---

## Wire Services / Global

| Source | RSS / URL | Type | Notes |
|---|---|---|---|
| AP News | `https://rsshub.app/apnews/topics/ap-top-news` | Wire | Fast, factual baseline |
| Reuters | `https://feeds.reuters.com/reuters/topNews` | Wire | Strong on energy, Gulf |
| AFP | Via Google News | Wire | Strong on Levant |

---

## Global Early Warning — The "Beginning to Matter" Layer
*These sources operate across all regions simultaneously. Scan these before regional sources in every session. They surface structural deterioration before it reaches mainstream coverage — exactly the pre-signal the Triad Model is designed to catch.*

| Source | RSS / URL | Type | Notes |
|---|---|---|---|
| ACLED | `https://acleddata.com/feed` | Data | Conflict event data globally — best for detecting violence clustering and acceleration before it becomes headline news. Filter by region. Updated weekly. |
| FEWS NET | `https://fews.net/fews-data/333` | Data | Famine and food security early warning. Covers 30+ countries. Food stress precedes political instability by 3-6 months — one of the best leading indicators available. |
| CFR Global Conflict Tracker | `https://www.cfr.org/global-conflict-tracker/rss` | Research | Tracks ~30 active conflicts with status updates. Best for flagging conflicts moving from stable to deteriorating. |
| Political Violence at a Glance | `https://politicalviolenceataglance.org/feed` | Research | Academic-grade analysis of political violence globally. Strong on early pattern recognition before Western media catches up. |
| ICG Crisis Watch | `https://www.crisisgroup.org/crisiswatch/rss` | Research | Monthly bulletin tracking 70+ conflict situations globally. Color-coded deterioration/improvement signals. One of the most reliable early warning products available open source. |
| UNHCR Operational Data | `https://reporting.unhcr.org/rss` | Data | Refugee and displacement flows. Displacement acceleration is a reliable leading indicator of conflict escalation or state failure. |
| UN OCHA ReliefWeb | `https://reliefweb.int/updates/rss.xml` | Data | Humanitarian situation reports globally. Strong on sub-Saharan Africa and South Asia where mainstream coverage is thin. |
| V-Dem | `https://www.v-dem.net` | Data | Democratic backsliding indicators. Early structural signal for regime fragility and political instability. Updated annually. |

*Usage note: In daily sessions, a 60-second scan of ICG Crisis Watch and ACLED for any new deterioration flags outside the primary regional focus is the minimum global early warning check. In Wednesday SITREPs, FEWS NET and UNHCR displacement data should be checked for any significant threshold crossings in the prior week.*

---

## Hard Indicator / Verification Tools
*These sources produce physical or sensor-derived data independent of narrative reporting. They are not news sources. Use them for cross-verification, not for signal detection.*

**Verification protocol:** A strike claim from any Telegram or news source gains elevated confidence when a FIRMS thermal anomaly appears in the same grid square within the same time window. An ADS-B pattern change over the Gulf combined with a MarineTraffic vessel movement and a Tzeva Adom alert sequence constitutes a hard indicator cluster. Two independent hard indicators plus one narrative source = reportable with high confidence. One hard indicator alone = notable but not confirmable. Narrative source alone = treat as claim pending verification.

| Source | URL | Type | Notes |
|---|---|---|---|
| NASA FIRMS | `https://firms.modaps.eosdis.nasa.gov` | Satellite | Thermal anomalies — confirm airstrikes, fires, missile impacts within hours. Free, API key easy to obtain. |
| ADS-B Exchange | `https://globe.adsbexchange.com` | Aircraft tracking | Military/unfiltered — does not honor government suppression requests. Use for ISR orbit detection and airspace closure confirmation over Gulf. |
| Tzeva Adom | `https://www.tzevaadom.co.il` | Alert system | Real-time Israeli missile and rocket alerts — primary hard indicator for Levant escalation. Updates every few seconds during active exchanges. |
| MarineTraffic | `https://www.marinetraffic.com` | Vessel tracking | Real-time vessel tracking — Hormuz and global chokepoints. Cross-reference with FIRMS and ADS-B for incident verification. |

---

## Think Tanks / Analytical

| Source | URL | Type | Notes |
|---|---|---|---|
| International Crisis Group | `https://www.crisisgroup.org/rss` | Research | Deep regional analysis — all active conflict zones |
| ACLED | `https://acleddata.com` | Data | Conflict event data by region |
| IISS | `https://www.iiss.org/rss` | Research | Military and security focus |
| Chatham House | `https://www.chathamhouse.org/rss.xml` | Research | Strong on energy and Russia |
| CFR Daily Brief | `https://www.cfr.org/rss/daily-brief` | Research | Fast daily analytical summary |
| Soufan Center | `https://thesoufancenter.org/feed` | Research | Terrorism and proxy networks |
| PIIE | `https://www.piie.com/rss/realtime` | Research | Economic dimensions |
| Geopolitical Futures | `https://geopoliticalfutures.com/feed` | Research | Friedman structural framework |
| RUSI | `https://rusi.org/rss` | Research | Military and security — strong on Russia and Europe |
| Bellingcat | `https://www.bellingcat.com/feed` | Research | Open source investigation — strong on verification of military claims |
| Stimson Center | `https://www.stimson.org/feed` | Research | South Asia, nuclear issues, non-traditional security |
| TTM Intelligence Division | `https://iran-sitrep.netlify.app/` | Internal | Daily updates specifically on the Iran conflict — cross-reference with current session output |

---

## Middle East — English Language

| Source | RSS / URL | Type | Notes |
|---|---|---|---|
| Al Jazeera English | `https://www.aljazeera.com/xml/rss/all.xml` | Broadcast | Strong Gulf and Levant coverage |
| Haaretz | `https://www.haaretz.com/cmlink/1.628765` | Newspaper | Best Israeli domestic politics |
| Middle East Eye | `https://www.middleeasteye.net/rss` | Digital | Strong on Gulf and Iran |
| Iran International | `https://iranintl.com/en/rss` | Broadcast | Best English-language Iran coverage |
| The New Arab | `https://www.newarab.com/rss.xml` | Digital | Arab perspective |
| Jerusalem Post | `https://www.jpost.com/rss/rssfeedsfrontpage.aspx` | Newspaper | Israeli security focus |
| Times of Israel | `https://www.timesofisrael.com/feed` | Digital | Fast on Israeli security breaking news |
| Daily Star Lebanon | `https://www.dailystar.com.lb/RSS.aspx` | Newspaper | Lebanon ground-level |
| Dawn (Pakistan) | `https://www.dawn.com/feeds/home` | Newspaper | Pakistan-Iran-Gulf dynamics |

---

## Middle East — Arabic Language

| Source | RSS / URL | Type | Notes |
|---|---|---|---|
| Al Jazeera Arabic | `https://www.aljazeera.net/xml/rss/all.xml` | Broadcast | Primary Arabic source |
| Al Arabiya | `https://www.alarabiya.net/ar/rss.xml` | Broadcast | Saudi-aligned perspective |
| Al Monitor | `https://www.al-monitor.com/rss` | Digital | Strong on Iran domestic |

---

## Energy / Commodity

| Source | URL | Type | Notes |
|---|---|---|---|
| IEA | `https://www.iea.org/news` | Official | Energy supply and reserve data |
| OPEC | `https://www.opec.org/opec_web/en/press_room/rss.htm` | Official | Supply decisions |
| Kpler | `https://www.kpler.com` | Data | Oil flow tracking |
| S&P Global Commodity | `https://www.spglobal.com/commodityinsights` | Data | Energy market intelligence |

---

## Great Power Inputs

| Source | RSS / URL | Region | Notes |
|---|---|---|---|
| TASS | `https://tass.com/rss/v2.xml` | Russia | State narrative — read for signal in framing, not content |
| Meduza | `https://meduza.io/en/rss/all` | Russia | Independent Russian journalism — actual ground truth vs TASS state narrative |
| Xinhua | `http://www.xinhuanet.com/english/rss/worldrss.xml` | China | State narrative — read for signal in framing |
| Global Times | `https://www.globaltimes.cn/rss/outbrain.xml` | China | Nationalist framing of China-US dynamics |
| CGTN | `https://www.cgtn.com/subscribe/feeds/english/rss.xml` | China | Chinese international broadcast |
| AMTI (CSIS) | `https://amti.csis.org/feed` | China / Indo-Pacific | Asia Maritime Transparency Initiative — South China Sea tracking |
| PressTV | `https://www.presstv.ir/feed` | Iran | Iranian state narrative — read for official framing, flag as propagandistic |
| Tasnim News | `https://www.tasnimnews.com/en/rss` | Iran | IRGC-aligned — read for military signaling, flag as propagandistic |
| CNBC Energy | `https://www.cnbc.com/id/10000664/device/rss/rss.html` | Global | Energy market reaction |

---

## Security Council / UN

| Source | URL | Notes |
|---|---|---|
| Security Council Report | `https://www.securitycouncilreport.org/monthly-forecast/` | Monthly forecasts by conflict |
| OCHA | `https://www.unocha.org/rss.xml` | Humanitarian situation data |
| UN News Middle East | `https://news.un.org/feed/subscribe/en/news/region/middle-east/feed/rss.xml` | Official UN coverage — Middle East |
| UN News Global | `https://news.un.org/feed/subscribe/en/news/feed/rss.xml` | Official UN coverage — all regions |

---

## Regional Expansion — Stubs
*Not yet active. Populate when coverage expands to these regions. Sources pre-vetted and ready.*

### Sub-Saharan Africa
| Source | RSS / URL | Type | Notes |
|---|---|---|---|
| AllAfrica | `https://allafrica.com/tools/headlines/rdf/latest/headlines.rdf` | Aggregator | Broadest Africa coverage available |
| ISS Africa | `https://issafrica.org/rss` | Research | Institute for Security Studies — conflict and governance |
| The Africa Report | `https://www.theafricareport.com/feed` | Digital | Strong on political economy |
| Daily Maverick | `https://www.dailymaverick.co.za/feed` | Newspaper | South Africa, regional politics |
| Premium Times | `https://www.premiumtimesng.com/feed` | Newspaper | West Africa — Nigeria |
| The East African | `https://www.theeastafrican.co.ke/feed` | Newspaper | East Africa |

### Indo-Pacific / South and Southeast Asia
| Source | RSS / URL | Type | Notes |
|---|---|---|---|
| The Diplomat | `https://thediplomat.com/feed` | Digital | Best general Indo-Pacific analytical coverage |
| Lowy Institute | `https://www.lowyinstitute.org/rss.xml` | Research | Australia-based, strong Indo-Pacific |
| Nikkei Asia | `https://asia.nikkei.com/rss/feed/nar` | Newspaper | Japan, regional economics |
| South China Morning Post | `https://www.scmp.com/rss/91/feed` | Newspaper | China and Hong Kong |
| The Hindu | `https://www.thehindu.com/news/feeder/default.rss` | Newspaper | India — best for South Asia regional dynamics |

### Eastern Europe / Former Soviet Space
| Source | RSS / URL | Type | Notes |
|---|---|---|---|
| Eurasianet | `https://eurasianet.org/rss` | Digital | Central Asia and Caucasus |
| RFE/RL | `https://www.rferl.org/api/zpiqmiesrrm` | Broadcast | Eastern Europe, Central Asia, Iran in Farsi |
| CACI Analyst | `https://cacianalyst.org/feed` | Research | Central Asia-Caucasus specialist depth |
| Kyiv Independent | `https://kyivindependent.com/feed` | Newspaper | Ukraine — ground truth on Russia-Ukraine |

### Latin America
| Source | RSS / URL | Type | Notes |
|---|---|---|---|
| InSight Crime | `https://insightcrime.org/feed` | Research | Organized crime and instability — best early warning for LatAm |
| NACLA | `https://nacla.org/rss.xml` | Research | Political economy of Latin America |
| Folha de S.Paulo | `https://feeds.folha.uol.com.br/mundo/rss091.xml` | Newspaper | Brazil — largest economy, regional signal |
| El País América | `https://feeds.elpais.com/mrss-s/pages/ep/site/elpais.com/section/america/portada` | Newspaper | Spanish-language regional coverage |

---

## Source Performance Notes
*Updated as source quality is observed over longitudinal tracking*

**As of Issue 001:**
- No performance data yet — baseline established
- Track: which sources surface signals before Western mainstream; which sources reflect official positions vs ground truth; which analytical outlets proved accurate on Iran succession and IRGC dynamics

**Performance tracking format (add entries here as patterns emerge):**
- Source name: observation, issue number where observed
- Example: "Iran International: surfaced Mojtaba health reporting 48 hours before wire services — Issue 002"

---

## Google News RSS by Country
*Use for country-specific coverage in any language. Swap language and country codes as needed.*

Format: `https://news.google.com/rss?hl=[language]&gl=[country]&ceid=[country]:[language]`

**Middle East:**
- Iran (Persian): `https://news.google.com/rss?hl=fa&gl=IR&ceid=IR:fa`
- Israel (Hebrew): `https://news.google.com/rss?hl=iw&gl=IL&ceid=IL:iw`
- Saudi Arabia (Arabic): `https://news.google.com/rss?hl=ar&gl=SA&ceid=SA:ar`
- Lebanon (Arabic): `https://news.google.com/rss?hl=ar&gl=LB&ceid=LB:ar`
- Pakistan (Urdu): `https://news.google.com/rss?hl=ur&gl=PK&ceid=PK:ur`

**Great Powers:**
- Russia (Russian): `https://news.google.com/rss?hl=ru&gl=RU&ceid=RU:ru`
- China (Chinese): `https://news.google.com/rss?hl=zh-CN&gl=CN&ceid=CN:zh-Hans`
- USA (English): `https://news.google.com/rss?hl=en&gl=US&ceid=US:en`

**Regional Expansion (ready when needed):**
- India (Hindi): `https://news.google.com/rss?hl=hi&gl=IN&ceid=IN:hi`
- Brazil (Portuguese): `https://news.google.com/rss?hl=pt-BR&gl=BR&ceid=BR:pt-419`
- Turkey (Turkish): `https://news.google.com/rss?hl=tr&gl=TR&ceid=TR:tr`
- Nigeria (English): `https://news.google.com/rss?hl=en&gl=NG&ceid=NG:en`
- South Africa (English): `https://news.google.com/rss?hl=en&gl=ZA&ceid=ZA:en`
- Indonesia (Indonesian): `https://news.google.com/rss?hl=id&gl=ID&ceid=ID:id`
- Japan (Japanese): `https://news.google.com/rss?hl=ja&gl=JP&ceid=JP:ja`
