# Abu Dhabi Family Brief sources (verified 2026-10-25, ~07:00 CET)
X handles were checked through the X API on 2026-10-25. Each account exists, is public and matches its official description. "Last post" is the latest post seen in a search since mid-September. "n/c" means activity was not checked. "Quiet" means no posts were found since Sep 15. Follower counts are as of the check. The X read budget is shared with the other briefs, so batch lookups and prefer one combined `from:a OR from:b` search per run.

## X: government, emergency and services
| Handle | Name | Followers | Last post | Why |
|---|---|---|---|---|
| @ADMediaOffice | Abu Dhabi Media Office (verified) | 322,239 | Oct 24 | Official Abu Dhabi government news, in English and Arabic |
| @UAEmediaoffice | UAE Government Media Office (verified) | 451,801 | n/c | Federal announcements, holidays, laws |
| @WAMNEWS_ENG | WAM English | 68,039 | n/c | State news agency |
| @NCEMAUAE | NCEMA (verified) | 248,125 | Quiet | National emergency authority; posts only when there is an incident |
| @ncmuae | National Centre of Meteorology (verified) | 192,251 | Oct 25 | Fog, rain and dust alerts (mostly Arabic, some English) |
| @ADPoliceHQ | Abu Dhabi Police (verified) | 297,462 | n/c | Traffic, safety, scams |
| @ad_mobility | AD Mobility, ex-ITC (verified) | 66,410 | Oct 23 | Road closures, Darb tolls, parking, buses |
| @Etihad_Rail | Etihad Rail (verified) | 166,893 | Oct 24 | Passenger rail news |
| @MOHRE_UAE | Ministry of Human Resources (verified) | 312,340 | Oct 24 | Labour law, gratuity, work permits |

## X: schools, housing, health
| Handle | Name | Followers | Last post | Why |
|---|---|---|---|---|
| @ADEK_tweet | ADEK (verified) | 104,541 | Oct 23 | School policy, fees, admissions, inspections |
| @adrec_ae | Abu Dhabi Real Estate Centre | 435 | Oct 22 | Rent cap, Tawtheeq, broker rules (small but official) |
| @DoHSocial | Department of Health Abu Dhabi (verified) | 77,411 | Oct 24 | Health rules, insurance, campaigns |
| @SEHAHealth | SEHA | 80,552 | n/c | Public hospitals, including Corniche Hospital (maternity) |
| @bayut / @propertyfinder | Property portals | 5,147 / 5,950 | n/c | Rent reports (use their websites for data) |

## X: advisories and embassies
| Handle | Name | Followers | Last post | Why |
|---|---|---|---|---|
| @USAinUAE | US Mission to UAE (verified) | 43,224 | Oct 24 | US advisories and security alerts for the UAE |
| @TravelGov | US State Dept Consular Affairs (verified) | 761,256 | Oct 24 | Advisory level changes |
| @FCDOtravelGovUK | FCDO Travel Advice (verified) | 146,826 | Oct 24 | UK travel advice updates |
| @Utrikesdep | Utrikesdepartementet | 65,223 | n/c | Swedish UD; the avrådan itself lives on regeringen.se |
| @SwedeninUAE | Embassy of Sweden in the UAE | 4,906 | Quiet | Swedish embassy (low activity) |
| @ukinuae | British Embassy UAE (verified) | 26,529 | Quiet | UK embassy (low activity) |

## X: news
| Handle | Name | Followers | Last post | Why |
|---|---|---|---|---|
| @TheNationalNews | The National (verified) | 1.11M | Oct 25 (web) | Main English daily in Abu Dhabi |
| @gulf_news | Gulf News | 1.58M | n/c | UAE daily (note: @GulfNews is suspended) |
| @khaleejtimes | Khaleej Times | 1.24M | n/c | UAE daily, strong on visas and expat rules |
| @AletihadEn | Aletihad English (verified) | 1,828 | Oct 23 | Abu Dhabi state daily, English |
| @ArabianBusiness | Arabian Business | 83,091 | n/c | Business, cost of living, visas |
| @agbinews | AGBI | 924 | n/c | Gulf business (use RSS) |

## X: life, travel and culture
| Handle | Name | Followers | Last post | Why |
|---|---|---|---|---|
| @TimeOutAbuDhabi | Time Out Abu Dhabi | 107,425 | Quiet | Use the RSS feed instead |
| @VisitAbuDhabi | Experience Abu Dhabi (verified) | 399,798 | n/c | Events and attractions |
| @dctabudhabi | DCT Abu Dhabi (verified) | 35,278 | n/c | Culture and tourism announcements |
| @yasisland | Yas Island (verified) | 43,354 | n/c | Yas events and parks |
| @LouvreAbuDhabi | Louvre Abu Dhabi (verified) | 63,191 | n/c | Saadiyat culture |
| @etihad / @EtihadHelp | Etihad Airways (verified) | 843,116 / 78,698 | n/c | Flight changes and disruption |
| @ADGlobalMarket | ADGM | 15,523 | n/c | ADGM (Al Reem and Al Maryah fall under ADGM rules) |

Rejected: @itcabudhabi (an empty placeholder with 0 posts; ITC is now @ad_mobility), @adek_ae (an unrelated personal account), @icpuae (empty, 0 posts), @USEmbassyUAE (suspended), @GulfNews (suspended) and @AbuDhabiGov (suspended).
Not found: ADEK_UAE, ADEKabudhabi, ADEK_AD, TAMMAbuDhabi, TAMM_AbuDhabi, TAMMgov, AbuDhabiDCT, whichschooladv, WhichSchoolAdvi, NCMS_media, uae_ncm, ADRECgov, AbuDhabiPolice, UAE_ICP, ADGMgov, ADRESOffice. No verified TAMM or ICP account was found, so use their websites.

## Web and RSS (checked 2026-10-25)
Working feeds:
- The National UAE: https://www.thenationalnews.com/arc/outboundfeeds/rss/category/news/uae/?outputType=xml
- The National, all sections: https://www.thenationalnews.com/arc/outboundfeeds/rss/?outputType=xml
- Gulf News: https://gulfnews.com/feed
- Time Out Abu Dhabi: https://www.timeoutabudhabi.com/feed (article pages block curl and fetch, so use the headlines and teasers)
- AGBI: https://www.agbi.com/feed/
- Arabian Business: https://www.arabianbusiness.com/feed (article pages are JS-walled)
- US Embassy UAE: https://ae.usembassy.gov/feed/ (alerts and the advisory)
- UK FCDO: https://www.gov.uk/foreign-travel-advice/united-arab-emirates.atom and https://www.gov.uk/api/content/foreign-travel-advice/united-arab-emirates (`public_updated_at`)

Pages to check:
- Sweden UD avrådan: https://www.regeringen.se/ud-avrader/forenade-arabemiraten---avradan/
- Swedish embassy reseinformation: https://www.swedenabroad.se/sv/om-utlandet-f%C3%B6r-svenska-medborgare/f%C3%B6renade-arabemiraten/reseinformation/ (curl gets 403; use WebFetch)
- ADEK news: https://adek.gov.ae/en/Media-Centre/News
- ADREC news: https://adrec.gov.ae/en/news
- Abu Dhabi Residents Office (Golden Visa): https://www.added.gov.ae/en/live/long-term-residency
- ICP Golden Residency: https://icp.gov.ae/en/services/uae-golden-residency/
- Abu Dhabi Media Office: https://www.mediaoffice.abudhabi/en/ (its RSS returns 404)
- TAMM: https://www.tamm.abudhabi/
- DoH: https://www.doh.gov.ae/en/news
- u.ae public holidays: https://u.ae/en/information-and-services/public-holidays-and-religious-affairs/public-holidays
- WAM fuel prices (monthly, around the last day of the month): https://www.wam.ae/en
- Savills Abu Dhabi residential (quarterly): https://www.savills.ae/research_articles/
- Regeringen pressmeddelanden (Swedish tax rules for people living abroad): https://www.regeringen.se/pressmeddelanden/ and Skatteverket: https://www.skatteverket.se/privat/internationellt/bosattutomlands/

Failing: Khaleej Times RSS (404, so use WebSearch or WebFetch for articles), WAM /en/rss (no items), the WhichSchoolAdvisor feed (no items; use the site through search), Abu Dhabi Media Office RSS (404).

Secondary, use with a flag: VisaHQ news and UECN (fast on visa circulars but they rewrite, so confirm with ADRO/ICP), Bayut and Property Finder reports (portal data), and thegulfpulse.com (market summaries).
