# COVID-19 US State Scraper

## Project Overview

This is a Python web scraper to get current case counts by US state.

I'm using the [list of state info pages on this page](http://coronavirusapi.com/) to get data sources.

Output is available as CSV, Markdown, or JSON. Specify `--format` as `csv`, `json`, or `md`.

## Current Counts (March 22 2020)

These are the only 30 states I plan to support for now. Others have bot-blockers, client-side rendering, or iframes
loading from arcgis. Any help pulling data from those sources would be greatly appreciated.

state | total_cases
--- | ---
AK | 22
AL | 157
AR | 165
CA | 1468
CO | 591
FL | 1007
GA | 620
HI | 56
ID | 2
IL | 1049
KS | 64
KY | 99
MA | 646
ME | 89
MI | 249
MN | 169
MO | 90
NC | 255
NE | 42
NH | 78
NJ | 1914
NM | 65
NY | 15168
OH | 351
OK | 67
OR | 161
PA | 479
SD | 21
TN | 505
TX | 334
VT | 52
 
## Features Needed

### Dynamic Page Support

Some sites are rendered client-side. I'll need either a more full-featured parser than BeautifulSoup or to
dig in and find the apps' data sources.
