# Changelog: NEPSE_dividend_panel_COMPLETED.csv

Every cell that was **empty** in `NEPSE_dividend_panel_FY2015-2025.csv` and is filled in `NEPSE_dividend_panel_COMPLETED.csv`. No cell that already had a value was changed. This list is generated from a cell-by-cell diff of the two files.

**Total cells filled: 325** (164 reported, 161 derived, 0 estimated).

## Classification

- **Reported**: the value is stated directly in the cited source.
- **Derived**: calculated from reported values. The formula is given in Notes. "Computed in-file" means both inputs are in the same row of the CSV.
- **Estimated**: none. No value was guessed or estimated. Where a source gave only an approximate figure (e.g. "about Rs 72.9 million"), the cell was left blank.

## Caveats

- Sources were found through web search. This environment could not open the source pages directly, so every value should be checked against the cited page before publication.
- Most new values for recent years come from **unaudited Q4 quarterly reports**, not audited annual reports.
- "Per-share proxy" ROE = EPS / net worth per share. This uses year-end equity, which is close to, but not identical to, NP / Equity.
- Prices derived as P/E x EPS carry the rounding of the reported P/E.
- SHL has a Rs 10 face value. Its cash DPS converts the reported dividend % to NPR (% / 100 x 10). Its DPS_Stock stays in %, as in the existing SHL rows.

## Other columns changed

- **Status**: recomputed for every row from the five core fields (SP, TotalAssets, EPS, DPS_Cash, ROE).
- **SourceRef**: new source text was appended after the existing text, which is unchanged. Two rows also carry cross-check notes with no cells changed: NTC 2019/20 (possible one-year offset in the existing EPS/NP) and CHCL 2022/23 (implausible quarter-end price of 209.4, not used).

## Cells filled by column

| Column | Cells |
|---|---|
| FirmAge_Years | 66 |
| YearIncorporated | 55 |
| DY_pct | 36 |
| DPS_Cash_NPR | 36 |
| DPS_Stock_NPR | 36 |
| EPS_NPR | 25 |
| ROE_pct | 21 |
| SP_NPR | 19 |
| PE_times | 18 |
| NetProfitAfterTax_NPR | 9 |
| FS_lnTA | 4 |

## All filled cells

| Company | FY | Column | Value | Type | Source | Notes |
|---|---|---|---|---|---|---|
| CHCL | 2018/19 | DY_pct | 0.9597 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| CHCL | 2019/20 | SP_NPR | 397.98 | Derived | https://www.sharesansar.com/newsdetail/chilime-hydropower-company-profit-remains-stagnant-in-q4-earns-rs-7480-crore-with-eps-of-rs-1310 | Qtr-end P/E x EPS (both reported in the same source); price not directly stated (30.38 x unaudited EPS 13.10) |
| CHCL | 2019/20 | DY_pct | 2.5127 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| CHCL | 2019/20 | PE_times | 30.47 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| CHCL | 2021/22 | DY_pct | 1.8382 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| CHCL | 2024/25 | NetProfitAfterTax_NPR | 679590000 | Reported | https://www.sharesansar.com/announcementdetail/chilime-hydropower-company-limited-has-posted-a-net-profit-of-rs-67959-million-and-published-its-4th-quarter-company-analysis-of-the-fiscal-year-208182-2025-08-12 | Unaudited Q4 |
| BPCL | 2022/23 | SP_NPR | 330.5 | Reported | https://www.sharesansar.com/newsdetail/butwal-power-bpcl-publicizes-q4-report-with-marginal-decline-in-net-profits-eps-at-rs-784-2023-08-11 ; https://www.investopaper.com/news/butwal-power-company-fourth-quarterly-report/ | Ashad-end price; 2 sources agree |
| BPCL | 2022/23 | DY_pct | 1.5129 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| BPCL | 2022/23 | PE_times | 36.93 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| BPCL | 2024/25 | DPS_Cash_NPR | 6 | Reported | https://www.sharesansar.com/newsdetail/butwal-power-company-proposes-6-cash-dividend-for-fy-208182-2025-12-19 | Board proposal, 6% cash; AGM Poush 28, 2082 |
| BPCL | 2024/25 | DPS_Stock_NPR | 0 | Reported | https://www.sharesansar.com/newsdetail/butwal-power-company-proposes-6-cash-dividend-for-fy-208182-2025-12-19 | Board proposal, 6% cash; AGM Poush 28, 2082 |
| BPCL | 2024/25 | DY_pct | 0.6268 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| NHPC | 2014/15 | YearIncorporated | 1996 | Reported | EMIS company profile https://www.emis.com/php/company-profile/NP/National_Hydro_Power_Company_Ltd_en_14787800.html | Incorporated 1996-09-12; single commercial-database source |
| NHPC | 2014/15 | FirmAge_Years | 19 | Derived | Computed in-file | FY end year - YearIncorporated |
| NHPC | 2015/16 | YearIncorporated | 1996 | Reported | EMIS company profile https://www.emis.com/php/company-profile/NP/National_Hydro_Power_Company_Ltd_en_14787800.html | Incorporated 1996-09-12; single commercial-database source |
| NHPC | 2015/16 | FirmAge_Years | 20 | Derived | Computed in-file | FY end year - YearIncorporated |
| NHPC | 2015/16 | DPS_Cash_NPR | 0 | Reported | MeroLagani NHPC dividend/announcement table https://merolagani.com/CompanyDetail.aspx?symbol=NHPC ; https://merolagani.com/AnnouncementSummary.aspx?actType=Cash+Dividend | 0.00% cash and bonus listed for FY2072/73-2076/77 |
| NHPC | 2015/16 | DPS_Stock_NPR | 0 | Reported | MeroLagani NHPC dividend/announcement table https://merolagani.com/CompanyDetail.aspx?symbol=NHPC ; https://merolagani.com/AnnouncementSummary.aspx?actType=Cash+Dividend | 0.00% cash and bonus listed for FY2072/73-2076/77 |
| NHPC | 2016/17 | YearIncorporated | 1996 | Reported | EMIS company profile https://www.emis.com/php/company-profile/NP/National_Hydro_Power_Company_Ltd_en_14787800.html | Incorporated 1996-09-12; single commercial-database source |
| NHPC | 2016/17 | FirmAge_Years | 21 | Derived | Computed in-file | FY end year - YearIncorporated |
| NHPC | 2016/17 | DPS_Cash_NPR | 0 | Reported | MeroLagani NHPC dividend/announcement table https://merolagani.com/CompanyDetail.aspx?symbol=NHPC ; https://merolagani.com/AnnouncementSummary.aspx?actType=Cash+Dividend | 0.00% cash and bonus listed for FY2072/73-2076/77 |
| NHPC | 2016/17 | DPS_Stock_NPR | 0 | Reported | MeroLagani NHPC dividend/announcement table https://merolagani.com/CompanyDetail.aspx?symbol=NHPC ; https://merolagani.com/AnnouncementSummary.aspx?actType=Cash+Dividend | 0.00% cash and bonus listed for FY2072/73-2076/77 |
| NHPC | 2017/18 | YearIncorporated | 1996 | Reported | EMIS company profile https://www.emis.com/php/company-profile/NP/National_Hydro_Power_Company_Ltd_en_14787800.html | Incorporated 1996-09-12; single commercial-database source |
| NHPC | 2017/18 | FirmAge_Years | 22 | Derived | Computed in-file | FY end year - YearIncorporated |
| NHPC | 2017/18 | DPS_Cash_NPR | 0 | Reported | MeroLagani NHPC dividend/announcement table https://merolagani.com/CompanyDetail.aspx?symbol=NHPC ; https://merolagani.com/AnnouncementSummary.aspx?actType=Cash+Dividend | 0.00% cash and bonus listed for FY2072/73-2076/77 |
| NHPC | 2017/18 | DPS_Stock_NPR | 0 | Reported | MeroLagani NHPC dividend/announcement table https://merolagani.com/CompanyDetail.aspx?symbol=NHPC ; https://merolagani.com/AnnouncementSummary.aspx?actType=Cash+Dividend | 0.00% cash and bonus listed for FY2072/73-2076/77 |
| NHPC | 2018/19 | YearIncorporated | 1996 | Reported | EMIS company profile https://www.emis.com/php/company-profile/NP/National_Hydro_Power_Company_Ltd_en_14787800.html | Incorporated 1996-09-12; single commercial-database source |
| NHPC | 2018/19 | FirmAge_Years | 23 | Derived | Computed in-file | FY end year - YearIncorporated |
| NHPC | 2018/19 | DPS_Cash_NPR | 0 | Reported | MeroLagani NHPC dividend/announcement table https://merolagani.com/CompanyDetail.aspx?symbol=NHPC ; https://merolagani.com/AnnouncementSummary.aspx?actType=Cash+Dividend | 0.00% cash and bonus listed for FY2072/73-2076/77 |
| NHPC | 2018/19 | DPS_Stock_NPR | 0 | Reported | MeroLagani NHPC dividend/announcement table https://merolagani.com/CompanyDetail.aspx?symbol=NHPC ; https://merolagani.com/AnnouncementSummary.aspx?actType=Cash+Dividend | 0.00% cash and bonus listed for FY2072/73-2076/77 |
| NHPC | 2019/20 | SP_NPR | 53 | Reported | https://www.sharesansar.com/newsdetail/national-hydro-power-company-limited-reports-slight-increase-in-revenue-eps-at-rs-076-2020-09-28 | Unaudited Q4 FY2076/77 |
| NHPC | 2019/20 | YearIncorporated | 1996 | Reported | EMIS company profile https://www.emis.com/php/company-profile/NP/National_Hydro_Power_Company_Ltd_en_14787800.html | Incorporated 1996-09-12; single commercial-database source |
| NHPC | 2019/20 | FirmAge_Years | 24 | Derived | Computed in-file | FY end year - YearIncorporated |
| NHPC | 2019/20 | EPS_NPR | 0.76 | Reported | https://www.sharesansar.com/newsdetail/national-hydro-power-company-limited-reports-slight-increase-in-revenue-eps-at-rs-076-2020-09-28 | Unaudited Q4 FY2076/77 |
| NHPC | 2019/20 | DPS_Cash_NPR | 0 | Reported | MeroLagani NHPC dividend/announcement table https://merolagani.com/CompanyDetail.aspx?symbol=NHPC ; https://merolagani.com/AnnouncementSummary.aspx?actType=Cash+Dividend | 0.00% cash and bonus listed for FY2072/73-2076/77 |
| NHPC | 2019/20 | DPS_Stock_NPR | 0 | Reported | MeroLagani NHPC dividend/announcement table https://merolagani.com/CompanyDetail.aspx?symbol=NHPC ; https://merolagani.com/AnnouncementSummary.aspx?actType=Cash+Dividend | 0.00% cash and bonus listed for FY2072/73-2076/77 |
| NHPC | 2019/20 | ROE_pct | 1.02 | Derived | https://www.sharesansar.com/newsdetail/national-hydro-power-company-limited-reports-slight-increase-in-revenue-eps-at-rs-076-2020-09-28 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| NHPC | 2019/20 | DY_pct | 0 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| NHPC | 2019/20 | PE_times | 69.74 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| NHPC | 2020/21 | YearIncorporated | 1996 | Reported | EMIS company profile https://www.emis.com/php/company-profile/NP/National_Hydro_Power_Company_Ltd_en_14787800.html | Incorporated 1996-09-12; single commercial-database source |
| NHPC | 2020/21 | FirmAge_Years | 25 | Derived | Computed in-file | FY end year - YearIncorporated |
| NHPC | 2020/21 | NetProfitAfterTax_NPR | -22180000 | Reported | https://www.sharesansar.com/announcementdetail/national-hydro-power-company-limited-has-posted-a-net-loss-of-rs-2218-million-and-published-its-4th-quarter-company-analysis-of-the-fiscal-year-207778-2021-08-22 | Net loss Rs 22.18 million, unaudited Q4 |
| NHPC | 2021/22 | YearIncorporated | 1996 | Reported | EMIS company profile https://www.emis.com/php/company-profile/NP/National_Hydro_Power_Company_Ltd_en_14787800.html | Incorporated 1996-09-12; single commercial-database source |
| NHPC | 2021/22 | FirmAge_Years | 26 | Derived | Computed in-file | FY end year - YearIncorporated |
| NHPC | 2022/23 | YearIncorporated | 1996 | Reported | EMIS company profile https://www.emis.com/php/company-profile/NP/National_Hydro_Power_Company_Ltd_en_14787800.html | Incorporated 1996-09-12; single commercial-database source |
| NHPC | 2022/23 | FirmAge_Years | 27 | Derived | Computed in-file | FY end year - YearIncorporated |
| NHPC | 2022/23 | EPS_NPR | 0.29 | Reported | https://nepsetrading.com/stockanalysis/tearsheet/NHPC | Q4 annualized EPS, unaudited |
| NHPC | 2022/23 | ROE_pct | 0.29 | Derived | https://nepsetrading.com/stockanalysis/tearsheet/NHPC | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| NHPC | 2023/24 | YearIncorporated | 1996 | Reported | EMIS company profile https://www.emis.com/php/company-profile/NP/National_Hydro_Power_Company_Ltd_en_14787800.html | Incorporated 1996-09-12; single commercial-database source |
| NHPC | 2023/24 | FirmAge_Years | 28 | Derived | Computed in-file | FY end year - YearIncorporated |
| NHPC | 2023/24 | EPS_NPR | -1.01 | Reported | https://nepsetrading.com/stockanalysis/tearsheet/NHPC | Q4 annualized EPS, unaudited |
| NHPC | 2023/24 | ROE_pct | -1.01 | Derived | https://nepsetrading.com/stockanalysis/tearsheet/NHPC | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| NHPC | 2024/25 | YearIncorporated | 1996 | Reported | EMIS company profile https://www.emis.com/php/company-profile/NP/National_Hydro_Power_Company_Ltd_en_14787800.html | Incorporated 1996-09-12; single commercial-database source |
| NHPC | 2024/25 | FirmAge_Years | 29 | Derived | Computed in-file | FY end year - YearIncorporated |
| NHPC | 2024/25 | EPS_NPR | 0.13 | Reported | https://nepsetrading.com/stockanalysis/tearsheet/NHPC | Q4 annualized EPS, unaudited |
| NHPC | 2024/25 | ROE_pct | 0.13 | Derived | https://nepsetrading.com/stockanalysis/tearsheet/NHPC | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| AHPC | 2014/15 | YearIncorporated | 1998 | Reported | https://www.sharesansar.com/company/ahpc | Established 1998-03-12 (Falgun 28, 2054 BS) |
| AHPC | 2014/15 | FirmAge_Years | 17 | Derived | Computed in-file | FY end year - YearIncorporated |
| AHPC | 2015/16 | YearIncorporated | 1998 | Reported | https://www.sharesansar.com/company/ahpc | Established 1998-03-12 (Falgun 28, 2054 BS) |
| AHPC | 2015/16 | FirmAge_Years | 18 | Derived | Computed in-file | FY end year - YearIncorporated |
| AHPC | 2016/17 | YearIncorporated | 1998 | Reported | https://www.sharesansar.com/company/ahpc | Established 1998-03-12 (Falgun 28, 2054 BS) |
| AHPC | 2016/17 | FirmAge_Years | 19 | Derived | Computed in-file | FY end year - YearIncorporated |
| AHPC | 2017/18 | YearIncorporated | 1998 | Reported | https://www.sharesansar.com/company/ahpc | Established 1998-03-12 (Falgun 28, 2054 BS) |
| AHPC | 2017/18 | FirmAge_Years | 20 | Derived | Computed in-file | FY end year - YearIncorporated |
| AHPC | 2018/19 | YearIncorporated | 1998 | Reported | https://www.sharesansar.com/company/ahpc | Established 1998-03-12 (Falgun 28, 2054 BS) |
| AHPC | 2018/19 | FirmAge_Years | 21 | Derived | Computed in-file | FY end year - YearIncorporated |
| AHPC | 2019/20 | YearIncorporated | 1998 | Reported | https://www.sharesansar.com/company/ahpc | Established 1998-03-12 (Falgun 28, 2054 BS) |
| AHPC | 2019/20 | FirmAge_Years | 22 | Derived | Computed in-file | FY end year - YearIncorporated |
| AHPC | 2020/21 | YearIncorporated | 1998 | Reported | https://www.sharesansar.com/company/ahpc | Established 1998-03-12 (Falgun 28, 2054 BS) |
| AHPC | 2020/21 | FirmAge_Years | 23 | Derived | Computed in-file | FY end year - YearIncorporated |
| AHPC | 2021/22 | YearIncorporated | 1998 | Reported | https://www.sharesansar.com/company/ahpc | Established 1998-03-12 (Falgun 28, 2054 BS) |
| AHPC | 2021/22 | FirmAge_Years | 24 | Derived | Computed in-file | FY end year - YearIncorporated |
| AHPC | 2021/22 | EPS_NPR | 4.98 | Reported | https://www.sharesansar.com/newsdetail/ahpc-witnesses-decline-in-net-profits-attributed-to-flood-damage-in-company-managed-hydropower-projects-in-q4-2023-08-15 | Prior-year comparative column |
| AHPC | 2021/22 | ROE_pct | 4.57 | Derived | https://www.sharesansar.com/newsdetail/ahpc-witnesses-decline-in-net-profits-attributed-to-flood-damage-in-company-managed-hydropower-projects-in-q4-2023-08-15 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| AHPC | 2022/23 | SP_NPR | 255 | Reported | https://www.sharesansar.com/newsdetail/ahpc-witnesses-decline-in-net-profits-attributed-to-flood-damage-in-company-managed-hydropower-projects-in-q4-2023-08-15 | Unaudited Q4 FY2079/80 |
| AHPC | 2022/23 | YearIncorporated | 1998 | Reported | https://www.sharesansar.com/company/ahpc | Established 1998-03-12 (Falgun 28, 2054 BS) |
| AHPC | 2022/23 | FirmAge_Years | 25 | Derived | Computed in-file | FY end year - YearIncorporated |
| AHPC | 2022/23 | EPS_NPR | 3.13 | Reported | https://www.sharesansar.com/newsdetail/ahpc-witnesses-decline-in-net-profits-attributed-to-flood-damage-in-company-managed-hydropower-projects-in-q4-2023-08-15 | Unaudited Q4 FY2079/80 |
| AHPC | 2022/23 | ROE_pct | 3.03 | Derived | https://www.sharesansar.com/newsdetail/ahpc-witnesses-decline-in-net-profits-attributed-to-flood-damage-in-company-managed-hydropower-projects-in-q4-2023-08-15 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| AHPC | 2022/23 | PE_times | 81.47 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| AHPC | 2023/24 | YearIncorporated | 1998 | Reported | https://www.sharesansar.com/company/ahpc | Established 1998-03-12 (Falgun 28, 2054 BS) |
| AHPC | 2023/24 | FirmAge_Years | 26 | Derived | Computed in-file | FY end year - YearIncorporated |
| AHPC | 2023/24 | EPS_NPR | 0.01 | Reported | https://www.sharesansar.com/newsdetail/arun-valley-hydropower-ahpc-reports-massive-surge-in-q4-profit-revenue-soars-by-14929-eps-reaches-rs-1165-2025-08-15 | Prior-year comparative column |
| AHPC | 2023/24 | ROE_pct | 0.01 | Derived | https://www.sharesansar.com/newsdetail/arun-valley-hydropower-ahpc-reports-massive-surge-in-q4-profit-revenue-soars-by-14929-eps-reaches-rs-1165-2025-08-15 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| AHPC | 2024/25 | SP_NPR | 291.69 | Reported | https://www.sharesansar.com/newsdetail/arun-valley-hydropower-ahpc-reports-massive-surge-in-q4-profit-revenue-soars-by-14929-eps-reaches-rs-1165-2025-08-15 | Unaudited Q4 FY2081/82 |
| AHPC | 2024/25 | YearIncorporated | 1998 | Reported | https://www.sharesansar.com/company/ahpc | Established 1998-03-12 (Falgun 28, 2054 BS) |
| AHPC | 2024/25 | FirmAge_Years | 27 | Derived | Computed in-file | FY end year - YearIncorporated |
| AHPC | 2024/25 | EPS_NPR | 11.65 | Reported | https://www.sharesansar.com/newsdetail/arun-valley-hydropower-ahpc-reports-massive-surge-in-q4-profit-revenue-soars-by-14929-eps-reaches-rs-1165-2025-08-15 | Unaudited Q4 FY2081/82 |
| AHPC | 2024/25 | ROE_pct | 10.38 | Derived | https://www.sharesansar.com/newsdetail/arun-valley-hydropower-ahpc-reports-massive-surge-in-q4-profit-revenue-soars-by-14929-eps-reaches-rs-1165-2025-08-15 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| AHPC | 2024/25 | DY_pct | 0.0891 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| AHPC | 2024/25 | PE_times | 25.04 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| SHPC | 2014/15 | YearIncorporated | 2008 | Reported | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-limited-ipo-analysis ; https://www.sharesansar.com/company/SHPC | Incorporated 2008 as Mai Hydropower Pvt Ltd |
| SHPC | 2014/15 | FirmAge_Years | 7 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHPC | 2015/16 | YearIncorporated | 2008 | Reported | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-limited-ipo-analysis ; https://www.sharesansar.com/company/SHPC | Incorporated 2008 as Mai Hydropower Pvt Ltd |
| SHPC | 2015/16 | FirmAge_Years | 8 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHPC | 2016/17 | YearIncorporated | 2008 | Reported | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-limited-ipo-analysis ; https://www.sharesansar.com/company/SHPC | Incorporated 2008 as Mai Hydropower Pvt Ltd |
| SHPC | 2016/17 | FirmAge_Years | 9 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHPC | 2017/18 | YearIncorporated | 2008 | Reported | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-limited-ipo-analysis ; https://www.sharesansar.com/company/SHPC | Incorporated 2008 as Mai Hydropower Pvt Ltd |
| SHPC | 2017/18 | FirmAge_Years | 10 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHPC | 2018/19 | YearIncorporated | 2008 | Reported | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-limited-ipo-analysis ; https://www.sharesansar.com/company/SHPC | Incorporated 2008 as Mai Hydropower Pvt Ltd |
| SHPC | 2018/19 | FirmAge_Years | 11 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHPC | 2019/20 | YearIncorporated | 2008 | Reported | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-limited-ipo-analysis ; https://www.sharesansar.com/company/SHPC | Incorporated 2008 as Mai Hydropower Pvt Ltd |
| SHPC | 2019/20 | FirmAge_Years | 12 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHPC | 2020/21 | SP_NPR | 513.09 | Derived | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-reports-decline-in-revenue-by-small-margin-how-has-it-performed-overall-2021-08-12 | Qtr-end P/E x EPS (both reported in the same source); price not directly stated (35.41 x 14.49) |
| SHPC | 2020/21 | YearIncorporated | 2008 | Reported | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-limited-ipo-analysis ; https://www.sharesansar.com/company/SHPC | Incorporated 2008 as Mai Hydropower Pvt Ltd |
| SHPC | 2020/21 | FirmAge_Years | 13 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHPC | 2020/21 | EPS_NPR | 14.49 | Reported | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-reports-decline-in-revenue-by-small-margin-how-has-it-performed-overall-2021-08-12 | Unaudited Q4 FY2077/78 |
| SHPC | 2020/21 | ROE_pct | 11.66 | Derived | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-reports-decline-in-revenue-by-small-margin-how-has-it-performed-overall-2021-08-12 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| SHPC | 2020/21 | DY_pct | 0.1033 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHPC | 2020/21 | PE_times | 35.41 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| SHPC | 2021/22 | YearIncorporated | 2008 | Reported | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-limited-ipo-analysis ; https://www.sharesansar.com/company/SHPC | Incorporated 2008 as Mai Hydropower Pvt Ltd |
| SHPC | 2021/22 | FirmAge_Years | 14 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHPC | 2021/22 | EPS_NPR | 17.68 | Reported | https://www.sharesansar.com/newsdetail/shpc-discloses-q4-report-with-2544-percent-decline-in-net-profits-company-attributes-loses-to-unfavourable-hydrological-conditions-2023-08-11 | Prior-year comparative column |
| SHPC | 2021/22 | ROE_pct | 7.68 | Derived | https://www.sharesansar.com/newsdetail/shpc-discloses-q4-report-with-2544-percent-decline-in-net-profits-company-attributes-loses-to-unfavourable-hydrological-conditions-2023-08-11 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| SHPC | 2022/23 | SP_NPR | 355 | Reported | https://www.sharesansar.com/newsdetail/shpc-discloses-q4-report-with-2544-percent-decline-in-net-profits-company-attributes-loses-to-unfavourable-hydrological-conditions-2023-08-11 ; https://www.investopaper.com/news/sanima-mai-hydropower-fourth-quarterly-report/ | 2 sources agree; unaudited Q4 |
| SHPC | 2022/23 | YearIncorporated | 2008 | Reported | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-limited-ipo-analysis ; https://www.sharesansar.com/company/SHPC | Incorporated 2008 as Mai Hydropower Pvt Ltd |
| SHPC | 2022/23 | FirmAge_Years | 15 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHPC | 2022/23 | EPS_NPR | 13.18 | Reported | https://www.sharesansar.com/newsdetail/shpc-discloses-q4-report-with-2544-percent-decline-in-net-profits-company-attributes-loses-to-unfavourable-hydrological-conditions-2023-08-11 ; https://www.investopaper.com/news/sanima-mai-hydropower-fourth-quarterly-report/ | 2 sources agree; unaudited Q4 |
| SHPC | 2022/23 | ROE_pct | 7.33 | Derived | https://www.sharesansar.com/newsdetail/shpc-discloses-q4-report-with-2544-percent-decline-in-net-profits-company-attributes-loses-to-unfavourable-hydrological-conditions-2023-08-11 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| SHPC | 2022/23 | DY_pct | 0.1493 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHPC | 2022/23 | PE_times | 26.93 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| SHPC | 2023/24 | YearIncorporated | 2008 | Reported | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-limited-ipo-analysis ; https://www.sharesansar.com/company/SHPC | Incorporated 2008 as Mai Hydropower Pvt Ltd |
| SHPC | 2023/24 | FirmAge_Years | 16 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHPC | 2024/25 | SP_NPR | 627 | Reported | https://nepsetrading.com/announcements/sanima-mai-hydropower-q4-financial-report | Prior-year column of the FY2082/83 Q4 filing; column mapping inferred from the stated 8.42% YoY profit decline |
| SHPC | 2024/25 | YearIncorporated | 2008 | Reported | https://www.sharesansar.com/newsdetail/sanima-mai-hydropower-limited-ipo-analysis ; https://www.sharesansar.com/company/SHPC | Incorporated 2008 as Mai Hydropower Pvt Ltd |
| SHPC | 2024/25 | FirmAge_Years | 17 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHPC | 2024/25 | EPS_NPR | 8.57 | Reported | https://nepsetrading.com/announcements/sanima-mai-hydropower-q4-financial-report | Prior-year column of the FY2082/83 Q4 filing; column mapping inferred from the stated 8.42% YoY profit decline |
| SHPC | 2024/25 | DPS_Cash_NPR | 0 | Reported | https://sharehubnepal.com/news/132752-bajarko-chirfar-saanima-mai-hydropower-annual-general-meeting | Board decided no dividend for FY2081/82; single source |
| SHPC | 2024/25 | DPS_Stock_NPR | 0 | Reported | https://sharehubnepal.com/news/132752-bajarko-chirfar-saanima-mai-hydropower-annual-general-meeting | Board decided no dividend for FY2081/82; single source |
| SHPC | 2024/25 | ROE_pct | 4.95 | Derived | https://nepsetrading.com/announcements/sanima-mai-hydropower-q4-financial-report | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| SHPC | 2024/25 | DY_pct | 0 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHPC | 2024/25 | PE_times | 73.16 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| SHPC | 2024/25 | NetProfitAfterTax_NPR | 320420000 | Reported | https://nepsetrading.com/announcements/sanima-mai-hydropower-q4-financial-report | Prior-year column of the FY2082/83 Q4 filing; column mapping inferred from the stated 8.42% YoY profit decline |
| NTC | 2014/15 | DPS_Cash_NPR | 50 | Reported | https://www.investopaper.com/news/dividend-history-of-nepal-telecom-ntc/ | 50% cash |
| NTC | 2014/15 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-nepal-telecom-ntc/ | 50% cash |
| NTC | 2014/15 | DY_pct | 7.8616 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| NTC | 2015/16 | DPS_Cash_NPR | 51 | Reported | https://www.investopaper.com/news/dividend-history-of-nepal-telecom-ntc/ ; https://www.sharesansar.com/newsdetail/nepal-telecom-to-approve-51-cash-dividend-9th-agm-today | 51% cash |
| NTC | 2015/16 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-nepal-telecom-ntc/ ; https://www.sharesansar.com/newsdetail/nepal-telecom-to-approve-51-cash-dividend-9th-agm-today | 51% cash |
| NTC | 2015/16 | DY_pct | 7.402 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| NTC | 2016/17 | DPS_Cash_NPR | 55 | Reported | https://www.investopaper.com/news/dividend-history-of-nepal-telecom-ntc/ ; https://thehimalayantimes.com/business/nepal-telecom-distribute-cash-dividend/ | 55% cash, 10th AGM |
| NTC | 2016/17 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-nepal-telecom-ntc/ ; https://thehimalayantimes.com/business/nepal-telecom-distribute-cash-dividend/ | 55% cash, 10th AGM |
| NTC | 2016/17 | DY_pct | 8.1481 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| NTC | 2017/18 | DY_pct | 7.6283 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| NTC | 2018/19 | DY_pct | 6.4935 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| NTC | 2020/21 | DPS_Cash_NPR | 20 | Reported | https://www.investopaper.com/news/dividend-history-of-nepal-telecom-ntc/ ; https://merolagani.com/CompanyDetail.aspx?symbol=ntc | 20% cash + 20% bonus; the cash/bonus split comes from Investopaper only |
| NTC | 2020/21 | DPS_Stock_NPR | 20 | Reported | https://www.investopaper.com/news/dividend-history-of-nepal-telecom-ntc/ ; https://merolagani.com/CompanyDetail.aspx?symbol=ntc | 20% cash + 20% bonus; the cash/bonus split comes from Investopaper only |
| NTC | 2021/22 | SP_NPR | 878.9 | Reported | https://www.sharesansar.com/newsdetail/nepal-doorsanchar-company-limited-major-highlights-of-the-4th-quarter-net-profit-rises-by-1754-and-net-worth-at-massive-rs-52813-2022-08-15 | Quarter-end price, unaudited Q4 |
| NTC | 2021/22 | DPS_Cash_NPR | 40 | Reported | https://www.investopaper.com/news/dividend-history-of-nepal-telecom-ntc/ ; https://merolagani.com/CompanyDetail.aspx?symbol=ntc | 40% cash |
| NTC | 2021/22 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-nepal-telecom-ntc/ ; https://merolagani.com/CompanyDetail.aspx?symbol=ntc | 40% cash |
| NTC | 2021/22 | DY_pct | 4.5511 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| NTC | 2021/22 | PE_times | 18.68 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| NTC | 2022/23 | SP_NPR | 907.09 | Derived | https://www.sharesansar.com/newsdetail/ntc-unveils-q4-report-with-rs-780-arba-in-net-profits-eps-stands-at-rs-4336-2023-08-16 | Qtr-end P/E x EPS (both reported in the same source); price not directly stated (20.92 x 43.36) |
| NTC | 2022/23 | DPS_Cash_NPR | 40 | Reported | https://www.investopaper.com/news/dividend-history-of-nepal-telecom-ntc/ ; https://www.sharesansar.com/eventdetail/dividend-declaration-40-cash-dividend-ntc-2023-12-22 | 40% cash |
| NTC | 2022/23 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-nepal-telecom-ntc/ ; https://www.sharesansar.com/eventdetail/dividend-declaration-40-cash-dividend-ntc-2023-12-22 | 40% cash |
| NTC | 2022/23 | DY_pct | 4.4097 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| NTC | 2022/23 | PE_times | 20.54 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| NTC | 2023/24 | SP_NPR | 844.97 | Derived | https://www.sharesansar.com/newsdetail/nepal-telecoms-net-profit-drops-1644-in-q4-fy-208081-revenue-and-investments-decline-2024-08-15 | Qtr-end P/E x EPS (both reported in the same source); price not directly stated (22.98 x 36.77) |
| NTC | 2023/24 | DY_pct | 3.5504 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| NTC | 2023/24 | PE_times | 24.41 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| NTC | 2024/25 | DPS_Cash_NPR | 30 | Reported | https://www.investopaper.com/news/nepal-telecom-dividend/ ; https://myrepublica.nagariknetwork.com/amp/news/nepal-telecom-announces-30-pc-cash-dividend-for-shareholders-14-70.html | 30% cash, 18th AGM |
| NTC | 2024/25 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/nepal-telecom-dividend/ ; https://myrepublica.nagariknetwork.com/amp/news/nepal-telecom-announces-30-pc-cash-dividend-for-shareholders-14-70.html | 30% cash, 18th AGM |
| UNL | 2014/15 | YearIncorporated | 1992 | Reported | EMIS https://www.emis.com/php/company-profile/NP/Unilever_Nepal_Ltd_en_14785706.html ; Kathmandu Post https://kathmandupost.com/money/2017/09/04/unl-to-extend-dividend-of-rs1270-per-share | Incorporated 1992-07-24 as Nepal Lever Ltd |
| UNL | 2014/15 | FirmAge_Years | 23 | Derived | Computed in-file | FY end year - YearIncorporated |
| UNL | 2015/16 | YearIncorporated | 1992 | Reported | EMIS https://www.emis.com/php/company-profile/NP/Unilever_Nepal_Ltd_en_14785706.html ; Kathmandu Post https://kathmandupost.com/money/2017/09/04/unl-to-extend-dividend-of-rs1270-per-share | Incorporated 1992-07-24 as Nepal Lever Ltd |
| UNL | 2015/16 | FirmAge_Years | 24 | Derived | Computed in-file | FY end year - YearIncorporated |
| UNL | 2016/17 | YearIncorporated | 1992 | Reported | EMIS https://www.emis.com/php/company-profile/NP/Unilever_Nepal_Ltd_en_14785706.html ; Kathmandu Post https://kathmandupost.com/money/2017/09/04/unl-to-extend-dividend-of-rs1270-per-share | Incorporated 1992-07-24 as Nepal Lever Ltd |
| UNL | 2016/17 | FirmAge_Years | 25 | Derived | Computed in-file | FY end year - YearIncorporated |
| UNL | 2017/18 | YearIncorporated | 1992 | Reported | EMIS https://www.emis.com/php/company-profile/NP/Unilever_Nepal_Ltd_en_14785706.html ; Kathmandu Post https://kathmandupost.com/money/2017/09/04/unl-to-extend-dividend-of-rs1270-per-share | Incorporated 1992-07-24 as Nepal Lever Ltd |
| UNL | 2017/18 | FirmAge_Years | 26 | Derived | Computed in-file | FY end year - YearIncorporated |
| UNL | 2018/19 | FS_lnTA | 22.0732 | Derived | Computed in-file | ln(TotalAssets_NPR) |
| UNL | 2018/19 | YearIncorporated | 1992 | Reported | EMIS https://www.emis.com/php/company-profile/NP/Unilever_Nepal_Ltd_en_14785706.html ; Kathmandu Post https://kathmandupost.com/money/2017/09/04/unl-to-extend-dividend-of-rs1270-per-share | Incorporated 1992-07-24 as Nepal Lever Ltd |
| UNL | 2018/19 | FirmAge_Years | 27 | Derived | Computed in-file | FY end year - YearIncorporated |
| UNL | 2019/20 | FS_lnTA | 22.0379 | Derived | Computed in-file | ln(TotalAssets_NPR) |
| UNL | 2019/20 | YearIncorporated | 1992 | Reported | EMIS https://www.emis.com/php/company-profile/NP/Unilever_Nepal_Ltd_en_14785706.html ; Kathmandu Post https://kathmandupost.com/money/2017/09/04/unl-to-extend-dividend-of-rs1270-per-share | Incorporated 1992-07-24 as Nepal Lever Ltd |
| UNL | 2019/20 | FirmAge_Years | 28 | Derived | Computed in-file | FY end year - YearIncorporated |
| UNL | 2020/21 | YearIncorporated | 1992 | Reported | EMIS https://www.emis.com/php/company-profile/NP/Unilever_Nepal_Ltd_en_14785706.html ; Kathmandu Post https://kathmandupost.com/money/2017/09/04/unl-to-extend-dividend-of-rs1270-per-share | Incorporated 1992-07-24 as Nepal Lever Ltd |
| UNL | 2020/21 | FirmAge_Years | 29 | Derived | Computed in-file | FY end year - YearIncorporated |
| UNL | 2021/22 | YearIncorporated | 1992 | Reported | EMIS https://www.emis.com/php/company-profile/NP/Unilever_Nepal_Ltd_en_14785706.html ; Kathmandu Post https://kathmandupost.com/money/2017/09/04/unl-to-extend-dividend-of-rs1270-per-share | Incorporated 1992-07-24 as Nepal Lever Ltd |
| UNL | 2021/22 | FirmAge_Years | 30 | Derived | Computed in-file | FY end year - YearIncorporated |
| UNL | 2022/23 | YearIncorporated | 1992 | Reported | EMIS https://www.emis.com/php/company-profile/NP/Unilever_Nepal_Ltd_en_14785706.html ; Kathmandu Post https://kathmandupost.com/money/2017/09/04/unl-to-extend-dividend-of-rs1270-per-share | Incorporated 1992-07-24 as Nepal Lever Ltd |
| UNL | 2022/23 | FirmAge_Years | 31 | Derived | Computed in-file | FY end year - YearIncorporated |
| UNL | 2022/23 | DPS_Cash_NPR | 1580 | Reported | https://www.sharesansar.com/newsdetail/unilever-nepal-limited-proposes-massive-1580-cash-dividend-for-fiscal-year-207980-2023-10-16 ; https://www.investopaper.com/news/dividend-history-of-unilever-nepal-limited-unl/ |  |
| UNL | 2022/23 | DPS_Stock_NPR | 0 | Reported | https://www.sharesansar.com/newsdetail/unilever-nepal-limited-proposes-massive-1580-cash-dividend-for-fiscal-year-207980-2023-10-16 ; https://www.investopaper.com/news/dividend-history-of-unilever-nepal-limited-unl/ |  |
| UNL | 2023/24 | YearIncorporated | 1992 | Reported | EMIS https://www.emis.com/php/company-profile/NP/Unilever_Nepal_Ltd_en_14785706.html ; Kathmandu Post https://kathmandupost.com/money/2017/09/04/unl-to-extend-dividend-of-rs1270-per-share | Incorporated 1992-07-24 as Nepal Lever Ltd |
| UNL | 2023/24 | FirmAge_Years | 32 | Derived | Computed in-file | FY end year - YearIncorporated |
| UNL | 2023/24 | EPS_NPR | 2122.69 | Reported | https://www.sharesansar.com/newsdetail/unilever-nepal-limited-reports-stable-q4-performance-net-profit-edges-up-035-2025-08-14 | Prior-year comparative; NP reported as Rs 1,955,000 thousand |
| UNL | 2023/24 | DPS_Cash_NPR | 1714 | Reported | https://merolagani.com/CompanyDetail.aspx?symbol=UNL ; https://www.investopaper.com/news/dividend-history-of-unilever-nepal-limited-unl/ |  |
| UNL | 2023/24 | DPS_Stock_NPR | 0 | Reported | https://merolagani.com/CompanyDetail.aspx?symbol=UNL ; https://www.investopaper.com/news/dividend-history-of-unilever-nepal-limited-unl/ |  |
| UNL | 2023/24 | NetProfitAfterTax_NPR | 1955000000 | Reported | https://www.sharesansar.com/newsdetail/unilever-nepal-limited-reports-stable-q4-performance-net-profit-edges-up-035-2025-08-14 | Prior-year comparative; NP reported as Rs 1,955,000 thousand |
| UNL | 2024/25 | SP_NPR | 46340 | Reported | https://www.sharesansar.com/newsdetail/unilever-nepal-limited-reports-stable-q4-performance-net-profit-edges-up-035-2025-08-14 | Unaudited Q4; MeroLagani shows a differing EPS of 2143.54 for an undated Q4 |
| UNL | 2024/25 | YearIncorporated | 1992 | Reported | EMIS https://www.emis.com/php/company-profile/NP/Unilever_Nepal_Ltd_en_14785706.html ; Kathmandu Post https://kathmandupost.com/money/2017/09/04/unl-to-extend-dividend-of-rs1270-per-share | Incorporated 1992-07-24 as Nepal Lever Ltd |
| UNL | 2024/25 | FirmAge_Years | 33 | Derived | Computed in-file | FY end year - YearIncorporated |
| UNL | 2024/25 | EPS_NPR | 2130.18 | Reported | https://www.sharesansar.com/newsdetail/unilever-nepal-limited-reports-stable-q4-performance-net-profit-edges-up-035-2025-08-14 | Unaudited Q4; MeroLagani shows a differing EPS of 2143.54 for an undated Q4 |
| UNL | 2024/25 | DPS_Cash_NPR | 1842 | Reported | https://www.sharesansar.com/newsdetail/unilever-nepal-confirms-npr-1842-per-share-dividend-at-32nd-agm-2025-11-16 |  |
| UNL | 2024/25 | DPS_Stock_NPR | 0 | Reported | https://www.sharesansar.com/newsdetail/unilever-nepal-confirms-npr-1842-per-share-dividend-at-32nd-agm-2025-11-16 |  |
| UNL | 2024/25 | DY_pct | 3.975 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| UNL | 2024/25 | PE_times | 21.75 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| UNL | 2024/25 | NetProfitAfterTax_NPR | 1961900000 | Reported | https://www.sharesansar.com/newsdetail/unilever-nepal-limited-reports-stable-q4-performance-net-profit-edges-up-035-2025-08-14 | Unaudited Q4; MeroLagani shows a differing EPS of 2143.54 for an undated Q4 |
| BNT | 2014/15 | YearIncorporated | 1986 | Reported | Tribhuvan University thesis chapter, elibrary.tucl.edu.np (specific PDF not pinned down via search) | LOW CONFIDENCE: single non-official source |
| BNT | 2014/15 | FirmAge_Years | 29 | Derived | Computed in-file | FY end year - YearIncorporated |
| BNT | 2015/16 | YearIncorporated | 1986 | Reported | Tribhuvan University thesis chapter, elibrary.tucl.edu.np (specific PDF not pinned down via search) | LOW CONFIDENCE: single non-official source |
| BNT | 2015/16 | FirmAge_Years | 30 | Derived | Computed in-file | FY end year - YearIncorporated |
| BNT | 2015/16 | DPS_Cash_NPR | 25 | Reported | https://www.investopaper.com/news/dividend-history-of-bottlers-nepal-terai-limited-bnt/ |  |
| BNT | 2015/16 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-bottlers-nepal-terai-limited-bnt/ |  |
| BNT | 2016/17 | YearIncorporated | 1986 | Reported | Tribhuvan University thesis chapter, elibrary.tucl.edu.np (specific PDF not pinned down via search) | LOW CONFIDENCE: single non-official source |
| BNT | 2016/17 | FirmAge_Years | 31 | Derived | Computed in-file | FY end year - YearIncorporated |
| BNT | 2016/17 | EPS_NPR | 327 | Reported | https://www.sharesansar.com/newsdetail/which-one-is-best-between-bottlers-nepal-terai-balaju-eps-at-rs-327-rs-273-respectively-in-q4 | Q4 FY2073/74 |
| BNT | 2016/17 | ROE_pct | 31.93 | Derived | https://www.sharesansar.com/newsdetail/which-one-is-best-between-bottlers-nepal-terai-balaju-eps-at-rs-327-rs-273-respectively-in-q4 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| BNT | 2017/18 | YearIncorporated | 1986 | Reported | Tribhuvan University thesis chapter, elibrary.tucl.edu.np (specific PDF not pinned down via search) | LOW CONFIDENCE: single non-official source |
| BNT | 2017/18 | FirmAge_Years | 32 | Derived | Computed in-file | FY end year - YearIncorporated |
| BNT | 2018/19 | YearIncorporated | 1986 | Reported | Tribhuvan University thesis chapter, elibrary.tucl.edu.np (specific PDF not pinned down via search) | LOW CONFIDENCE: single non-official source |
| BNT | 2018/19 | FirmAge_Years | 33 | Derived | Computed in-file | FY end year - YearIncorporated |
| BNT | 2018/19 | DPS_Cash_NPR | 40 | Reported | https://www.sharesansar.com/newsdetail/bottlers-nepal-terai-to-convene-33rd-agm-on-kartik-20-2076-cash-dividend-worth-rs40-per-share-to-be-endorsed |  |
| BNT | 2018/19 | DPS_Stock_NPR | 0 | Reported | https://www.sharesansar.com/newsdetail/bottlers-nepal-terai-to-convene-33rd-agm-on-kartik-20-2076-cash-dividend-worth-rs40-per-share-to-be-endorsed |  |
| BNT | 2019/20 | YearIncorporated | 1986 | Reported | Tribhuvan University thesis chapter, elibrary.tucl.edu.np (specific PDF not pinned down via search) | LOW CONFIDENCE: single non-official source |
| BNT | 2019/20 | FirmAge_Years | 34 | Derived | Computed in-file | FY end year - YearIncorporated |
| BNT | 2019/20 | DPS_Cash_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-bottlers-nepal-terai-limited-bnt/ | Zero dividend; single source |
| BNT | 2019/20 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-bottlers-nepal-terai-limited-bnt/ | Zero dividend; single source |
| BNT | 2020/21 | YearIncorporated | 1986 | Reported | Tribhuvan University thesis chapter, elibrary.tucl.edu.np (specific PDF not pinned down via search) | LOW CONFIDENCE: single non-official source |
| BNT | 2020/21 | FirmAge_Years | 35 | Derived | Computed in-file | FY end year - YearIncorporated |
| BNT | 2020/21 | EPS_NPR | 350.19 | Reported | https://www.sharesansar.com/newsdetail/bottlers-nepal-balaju-and-terai-published-q4-report-both-report-a-significant-incline-in-net-profits-by-8219-and-6121-respectively-2022-08-15 | Prior-year comparative |
| BNT | 2020/21 | DPS_Cash_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-bottlers-nepal-terai-limited-bnt/ | Zero dividend; single source |
| BNT | 2020/21 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-bottlers-nepal-terai-limited-bnt/ | Zero dividend; single source |
| BNT | 2020/21 | ROE_pct | 15.74 | Derived | https://www.sharesansar.com/newsdetail/bottlers-nepal-balaju-and-terai-published-q4-report-both-report-a-significant-incline-in-net-profits-by-8219-and-6121-respectively-2022-08-15 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| BNT | 2021/22 | SP_NPR | 13001.59 | Derived | https://www.sharesansar.com/newsdetail/bottlers-nepal-balaju-and-terai-published-q4-report-both-report-a-significant-incline-in-net-profits-by-8219-and-6121-respectively-2022-08-15 | Qtr-end P/E x EPS (both reported in the same source); price not directly stated (23.03 x 564.55) |
| BNT | 2021/22 | YearIncorporated | 1986 | Reported | Tribhuvan University thesis chapter, elibrary.tucl.edu.np (specific PDF not pinned down via search) | LOW CONFIDENCE: single non-official source |
| BNT | 2021/22 | FirmAge_Years | 36 | Derived | Computed in-file | FY end year - YearIncorporated |
| BNT | 2021/22 | EPS_NPR | 564.55 | Reported | https://www.sharesansar.com/newsdetail/bottlers-nepal-balaju-and-terai-published-q4-report-both-report-a-significant-incline-in-net-profits-by-8219-and-6121-respectively-2022-08-15 | Unaudited Q4 FY2078/79 |
| BNT | 2021/22 | ROE_pct | 20.24 | Derived | https://www.sharesansar.com/newsdetail/bottlers-nepal-balaju-and-terai-published-q4-report-both-report-a-significant-incline-in-net-profits-by-8219-and-6121-respectively-2022-08-15 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| BNT | 2021/22 | DY_pct | 0.4615 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| BNT | 2021/22 | PE_times | 23.03 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| BNT | 2022/23 | YearIncorporated | 1986 | Reported | Tribhuvan University thesis chapter, elibrary.tucl.edu.np (specific PDF not pinned down via search) | LOW CONFIDENCE: single non-official source |
| BNT | 2022/23 | FirmAge_Years | 37 | Derived | Computed in-file | FY end year - YearIncorporated |
| BNT | 2023/24 | YearIncorporated | 1986 | Reported | Tribhuvan University thesis chapter, elibrary.tucl.edu.np (specific PDF not pinned down via search) | LOW CONFIDENCE: single non-official source |
| BNT | 2023/24 | FirmAge_Years | 38 | Derived | Computed in-file | FY end year - YearIncorporated |
| BNT | 2023/24 | EPS_NPR | 298.23 | Reported | https://nepsetrading.com/blog/bottlers-nepal-terai-q4-results-revenue-decline-and-heavy-losses-despite-strong-market-value | Prior-year comparative |
| BNT | 2024/25 | SP_NPR | 12800 | Reported | https://nepsetrading.com/blog/bottlers-nepal-terai-q4-results-revenue-decline-and-heavy-losses-despite-strong-market-value | Unaudited Q4; ROE as stated in the source; MeroLagani agrees on EPS |
| BNT | 2024/25 | YearIncorporated | 1986 | Reported | Tribhuvan University thesis chapter, elibrary.tucl.edu.np (specific PDF not pinned down via search) | LOW CONFIDENCE: single non-official source |
| BNT | 2024/25 | FirmAge_Years | 39 | Derived | Computed in-file | FY end year - YearIncorporated |
| BNT | 2024/25 | EPS_NPR | -502.13 | Reported | https://nepsetrading.com/blog/bottlers-nepal-terai-q4-results-revenue-decline-and-heavy-losses-despite-strong-market-value | Unaudited Q4; ROE as stated in the source; MeroLagani agrees on EPS |
| BNT | 2024/25 | ROE_pct | -14.96 | Reported | https://nepsetrading.com/blog/bottlers-nepal-terai-q4-results-revenue-decline-and-heavy-losses-despite-strong-market-value | Unaudited Q4; ROE as stated in the source; MeroLagani agrees on EPS |
| HDL | 2014/15 | DPS_Cash_NPR | 20 | Reported | https://www.investopaper.com/news/dividend-history-of-himalayan-distillery-limited-hdl/ ; https://www.sharesansar.com/company/HDL (AGM records) |  |
| HDL | 2014/15 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-himalayan-distillery-limited-hdl/ ; https://www.sharesansar.com/company/HDL (AGM records) |  |
| HDL | 2015/16 | DPS_Cash_NPR | 20 | Reported | https://www.investopaper.com/news/dividend-history-of-himalayan-distillery-limited-hdl/ ; https://www.sharesansar.com/company/HDL (AGM records) |  |
| HDL | 2015/16 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-himalayan-distillery-limited-hdl/ ; https://www.sharesansar.com/company/HDL (AGM records) |  |
| HDL | 2016/17 | DPS_Cash_NPR | 21.05 | Reported | https://www.investopaper.com/news/dividend-history-of-himalayan-distillery-limited-hdl/ ; https://www.sharesansar.com/company/HDL (AGM records) |  |
| HDL | 2016/17 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-himalayan-distillery-limited-hdl/ ; https://www.sharesansar.com/company/HDL (AGM records) |  |
| HDL | 2017/18 | SP_NPR | 1350.8 | Derived | https://www.sharesansar.com/newsdetail/himalayan-distillery-reports-a-staggering-52194-rise-in-net-profit-reaching-rs-3039-crore-in-q4-of-fy-207475-major-portion-of-revenue-driven-by-golden-oak-sales | Qtr-end P/E x EPS (both reported in the same source); price not directly stated (17.14 x 78.81) |
| HDL | 2017/18 | EPS_NPR | 78.81 | Reported | https://www.sharesansar.com/newsdetail/himalayan-distillery-reports-a-staggering-52194-rise-in-net-profit-reaching-rs-3039-crore-in-q4-of-fy-207475-major-portion-of-revenue-driven-by-golden-oak-sales | Unaudited Q4 |
| HDL | 2017/18 | DPS_Cash_NPR | 89.47 | Reported | https://www.sharesansar.com/company/HDL (AGM records) | SOURCES DIFFER: 21.05% regular + 68.42% special = 89.47% (ShareSansar) vs 68.42% (Investopaper); used 89.47 |
| HDL | 2017/18 | DPS_Stock_NPR | 0 | Reported | https://www.sharesansar.com/company/HDL (AGM records) | SOURCES DIFFER: 21.05% regular + 68.42% special = 89.47% (ShareSansar) vs 68.42% (Investopaper); used 89.47 |
| HDL | 2017/18 | ROE_pct | 37.86 | Derived | https://www.sharesansar.com/newsdetail/himalayan-distillery-reports-a-staggering-52194-rise-in-net-profit-reaching-rs-3039-crore-in-q4-of-fy-207475-major-portion-of-revenue-driven-by-golden-oak-sales | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| HDL | 2017/18 | DY_pct | 6.6235 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| HDL | 2017/18 | PE_times | 17.14 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| HDL | 2017/18 | NetProfitAfterTax_NPR | 303900000 | Reported | https://www.sharesansar.com/newsdetail/himalayan-distillery-reports-a-staggering-52194-rise-in-net-profit-reaching-rs-3039-crore-in-q4-of-fy-207475-major-portion-of-revenue-driven-by-golden-oak-sales | Rs 30.39 crore |
| HDL | 2018/19 | DPS_Cash_NPR | 52.63 | Reported | https://www.sharesansar.com/newsdetail/himalayan-distillery-proposes-50-bonus-and-5263-cash-dividend-agm-to-be-held-on-poush-01-2076 |  |
| HDL | 2018/19 | DPS_Stock_NPR | 50 | Reported | https://www.sharesansar.com/newsdetail/himalayan-distillery-proposes-50-bonus-and-5263-cash-dividend-agm-to-be-held-on-poush-01-2076 |  |
| HDL | 2019/20 | SP_NPR | 1599.31 | Derived | https://www.sharesansar.com/newsdetail/decline-in-demand-for-alcohol-due-to-lockdown-and-ongoing-pandemic-results-in-25-fall-in-sales-revenue-of-himalayan-distillery-in-q4 | Qtr-end P/E x EPS (both reported in the same source); price not directly stated (19.85 x 80.57) |
| HDL | 2019/20 | EPS_NPR | 80.57 | Reported | https://www.sharesansar.com/newsdetail/decline-in-demand-for-alcohol-due-to-lockdown-and-ongoing-pandemic-results-in-25-fall-in-sales-revenue-of-himalayan-distillery-in-q4 | Unaudited Q4 |
| HDL | 2019/20 | ROE_pct | 37.18 | Derived | https://www.sharesansar.com/newsdetail/decline-in-demand-for-alcohol-due-to-lockdown-and-ongoing-pandemic-results-in-25-fall-in-sales-revenue-of-himalayan-distillery-in-q4 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| HDL | 2019/20 | DY_pct | 3.1263 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| HDL | 2019/20 | PE_times | 19.85 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| HDL | 2020/21 | SP_NPR | 5512.44 | Derived | https://www.sharesansar.com/newsdetail/himalayan-distillery-reported-2021-08-13 | Qtr-end P/E x EPS (both reported in the same source); price not directly stated (45.96 x 119.94) |
| HDL | 2020/21 | EPS_NPR | 119.94 | Reported | https://www.sharesansar.com/newsdetail/himalayan-distillery-reported-2021-08-13 | Unaudited Q4 |
| HDL | 2020/21 | ROE_pct | 51.93 | Derived | https://www.sharesansar.com/newsdetail/himalayan-distillery-reported-2021-08-13 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| HDL | 2020/21 | DY_pct | 0.4535 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| HDL | 2020/21 | PE_times | 45.96 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| HDL | 2021/22 | DPS_Cash_NPR | 10 | Reported | https://www.sharesansar.com/company/HDL (22nd AGM) ; https://www.investopaper.com/news/dividend-history-of-himalayan-distillery-limited-hdl/ |  |
| HDL | 2021/22 | DPS_Stock_NPR | 60 | Reported | https://www.sharesansar.com/company/HDL (22nd AGM) ; https://www.investopaper.com/news/dividend-history-of-himalayan-distillery-limited-hdl/ |  |
| HDL | 2022/23 | SP_NPR | 2248.05 | Derived | https://www.sharesansar.com/newsdetail/hdl-makes-public-q4-report-with-decline-in-net-profit-eps-contracts-to-rs-2717-2023-08-15 | Qtr-end P/E x EPS (both reported in the same source); price not directly stated (82.74 x 27.17) |
| HDL | 2022/23 | EPS_NPR | 27.17 | Reported | https://www.sharesansar.com/newsdetail/hdl-makes-public-q4-report-with-decline-in-net-profit-eps-contracts-to-rs-2717-2023-08-15 | Unaudited Q4 |
| HDL | 2022/23 | ROE_pct | 19.69 | Derived | https://www.sharesansar.com/newsdetail/hdl-makes-public-q4-report-with-decline-in-net-profit-eps-contracts-to-rs-2717-2023-08-15 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| HDL | 2022/23 | DY_pct | 0.6672 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| HDL | 2022/23 | PE_times | 82.74 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| HDL | 2023/24 | EPS_NPR | 13.66 | Reported | https://www.sharesansar.com/newsdetail/himalayan-distillery-reports-161-surge-in-q4-net-profit-revenue-crosses-rs-720-arba-2025-08-14 | Prior-year comparative |
| HDL | 2023/24 | NetProfitAfterTax_NPR | 353050000 | Reported | https://www.sharesansar.com/announcementdetail/himalayan-distillery-limited-has-posted-a-net-profit-of-rs-35305-million-and-published-its-4th-quarter-company-analysis-of-the-fiscal-year-208081-2024-08-14 | Unaudited Q4 |
| HDL | 2024/25 | SP_NPR | 1236.77 | Derived | https://www.sharesansar.com/newsdetail/himalayan-distillery-reports-161-surge-in-q4-net-profit-revenue-crosses-rs-720-arba-2025-08-14 | Qtr-end P/E x EPS (both reported in the same source); price not directly stated (39.87 x 31.02) |
| HDL | 2024/25 | EPS_NPR | 31.02 | Reported | https://www.sharesansar.com/newsdetail/himalayan-distillery-reports-161-surge-in-q4-net-profit-revenue-crosses-rs-720-arba-2025-08-14 | Unaudited Q4 |
| HDL | 2024/25 | ROE_pct | 22.84 | Derived | https://www.sharesansar.com/newsdetail/himalayan-distillery-reports-161-surge-in-q4-net-profit-revenue-crosses-rs-720-arba-2025-08-14 | EPS / net worth per share (both reported in the same source); per-share proxy for ROE |
| HDL | 2024/25 | DY_pct | 0.4043 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| HDL | 2024/25 | PE_times | 39.87 | Derived | Computed in-file | SP_NPR / EPS_NPR |
| SHL | 2014/15 | FirmAge_Years | 49 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHL | 2014/15 | DPS_Cash_NPR | 0.6579 | Derived | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Cash % (reported) converted to NPR/share at face value Rs 10 |
| SHL | 2014/15 | DPS_Stock_NPR | 25 | Reported | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Bonus % (as in existing SHL rows) |
| SHL | 2014/15 | DY_pct | 0.1548 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHL | 2015/16 | FirmAge_Years | 50 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHL | 2015/16 | DPS_Cash_NPR | 1.1053 | Derived | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Cash % (reported) converted to NPR/share at face value Rs 10 |
| SHL | 2015/16 | DPS_Stock_NPR | 10 | Reported | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Bonus % (as in existing SHL rows) |
| SHL | 2015/16 | DY_pct | 0.2947 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHL | 2016/17 | FirmAge_Years | 51 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHL | 2016/17 | DPS_Cash_NPR | 0.6053 | Derived | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Cash % (reported) converted to NPR/share at face value Rs 10 |
| SHL | 2016/17 | DPS_Stock_NPR | 15 | Reported | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Bonus % (as in existing SHL rows) |
| SHL | 2016/17 | DY_pct | 0.1677 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHL | 2017/18 | FirmAge_Years | 52 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHL | 2017/18 | DPS_Cash_NPR | 1.6316 | Derived | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Cash % (reported) converted to NPR/share at face value Rs 10 |
| SHL | 2017/18 | DPS_Stock_NPR | 10 | Reported | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Bonus % (as in existing SHL rows) |
| SHL | 2017/18 | DY_pct | 0.6714 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHL | 2018/19 | FirmAge_Years | 53 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHL | 2018/19 | DPS_Cash_NPR | 1.1316 | Derived | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Cash % (reported) converted to NPR/share at face value Rs 10 |
| SHL | 2018/19 | DPS_Stock_NPR | 15 | Reported | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Bonus % (as in existing SHL rows) |
| SHL | 2018/19 | DY_pct | 0.4638 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHL | 2019/20 | FirmAge_Years | 54 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHL | 2019/20 | DPS_Cash_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Zero dividend; single source |
| SHL | 2019/20 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Zero dividend; single source |
| SHL | 2019/20 | DY_pct | 0 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHL | 2020/21 | FirmAge_Years | 55 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHL | 2020/21 | DPS_Cash_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Zero dividend; single source |
| SHL | 2020/21 | DPS_Stock_NPR | 0 | Reported | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ | Zero dividend; single source |
| SHL | 2020/21 | DY_pct | 0 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHL | 2021/22 | FirmAge_Years | 56 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHL | 2021/22 | DPS_Cash_NPR | 2.1316 | Derived | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ ; https://www.sharesansar.com/newsdetail/soaltee-hotel-distributed-21315-cash-dividends-directly-to-shareholders-bank-accounts-2023-01-31 | Cash % (reported) converted to NPR/share at face value Rs 10 |
| SHL | 2021/22 | DPS_Stock_NPR | 5 | Reported | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ ; https://www.sharesansar.com/newsdetail/soaltee-hotel-distributed-21315-cash-dividends-directly-to-shareholders-bank-accounts-2023-01-31 | Bonus % |
| SHL | 2021/22 | DY_pct | 1.0526 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHL | 2021/22 | NetProfitAfterTax_NPR | 297240000 | Reported | Soaltee Hotel 49th Annual Report 2022/23 https://soalteehotel.com/uploads/pdfs/241008071607.pdf | Official annual report (audited) |
| SHL | 2022/23 | FirmAge_Years | 57 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHL | 2022/23 | DY_pct | 0.548 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHL | 2022/23 | NetProfitAfterTax_NPR | 554980000 | Reported | Soaltee Hotel 49th Annual Report 2022/23 https://soalteehotel.com/uploads/pdfs/241008071607.pdf | Official annual report (audited) |
| SHL | 2023/24 | FS_lnTA | 21.6886 | Derived | Computed in-file | ln(TotalAssets_NPR) |
| SHL | 2023/24 | FirmAge_Years | 58 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHL | 2023/24 | DPS_Cash_NPR | 2.6842 | Derived | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ ; https://www.sharesansar.com/eventdetail/50th-agm-of-soaltee-hotel-limited-shl-2024-10-30 | Cash % (reported) converted to NPR/share at face value Rs 10 |
| SHL | 2023/24 | DPS_Stock_NPR | 10 | Reported | https://www.investopaper.com/news/dividend-history-of-soaltee-hotel-limited-shl/ ; https://www.sharesansar.com/eventdetail/50th-agm-of-soaltee-hotel-limited-shl-2024-10-30 | Bonus % |
| SHL | 2023/24 | DY_pct | 0.6073 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
| SHL | 2024/25 | FS_lnTA | 21.8437 | Derived | Computed in-file | ln(TotalAssets_NPR) |
| SHL | 2024/25 | FirmAge_Years | 59 | Derived | Computed in-file | FY end year - YearIncorporated |
| SHL | 2024/25 | DY_pct | 0.2874 | Derived | Computed in-file | DPS_Cash_NPR / SP_NPR x 100 |
