# Airline-Sentiment-and-Churn-Analysis
## Executive Summary:
SkyWings Airlines faced a sharp revenue decline (Business −26%, Economy −18% YoY) alongside rising dissatisfaction posted online. Using KNIME text mining and Tableau KPI dashboards, my team and I linked customer reviews + transactions to pinpoint the biggest drivers: cancellations at 15% vs 2% industry benchmark, and complaints concentrated in poor customer service (35.08%) and low quality perception (34.6%). Hence, we recommended the company to:

1. Reduce flight cancellations with a 3-stage “Service Netting” plan (prevent, respond, recover).
2. Win back returning Economy customers (core revenue segment) via loyalty perks + targeted recovery offers.
3. Redesign promotions (only 16.91% promo usage) to be more visible and targeted.

## Business Problem:
For an airline, bookings and reputation are closely tied to revenue. SkyWings is seeing booking decline while negative reviews online increase, suggesting a breakdown in customer experience and trust.  Despite having relevant data, Skywings has not utilised relevant tools to uncover root causes and take targeted action. What is causing the decline in business performance and what changes should be prioritised to reverse it?

## Methodology:

1. KNIME text cleaning & document prep to convert Cust_Reviews into analysable text (Excel/CSV import → Strings to Document → de-dup → remove punctuation/numbers/stop words → lowercase + stemming).
2. KNIME sentiment + keyword extraction using MPQA lexicons (Dictionary Tagger → Bag of Words + Term Frequency → convert tags/terms to strings → filter missing → group/sum term frequencies → split positive vs negative → Tag Cloud) and export the cleaned sentiment-keyword output to Excel.
3. Tableau dashboard + story combining Fact_Trans, Cust_Reviews, and the KNIME export to visualise (a) positive/negative word clouds + (b) transaction KPI charts, add interactivity, and translate insights into retention + service-recovery recommendations.

## Skills:
KNIME (Text Mining): Excel/CSV Reader, Strings to Document, Case Converter, Kuhlen Stemmer, Dictionary Tagger (MPQA), Document Viewer, Bag of Words Creator, TF, Tags to Strings, Term to Strings, Row Filter, GroupBy (SUM), Tag Cloud (JavaScript), Excel Writer

Tableau: multi-source data setup, calculated fields, dashboards, story points, KPI trend charts, segmentation views, filters/tooltips/parameters

Analytics: lexicon-based sentiment analysis, text preprocessing, keyword frequency/theme extraction, KPI diagnostics, benchmarking, recommendation storytelling

## Results & Business Recommendation:

