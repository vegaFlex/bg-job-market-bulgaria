# Bulgarian Labour Market Analysis (NSI)

## Data source
National Statistical Institute Bulgaria (NSI) open data.
Files used:
- data/raw/nsi_employment_by_sector.csv
- data/raw/nsi_employment_by_education.csv
- data/raw/nsi_employment_15_64_by_region.csv

## Data dictionary
- periods: quarter in format YYYYQn
- Units: measurement unit (1000cp means thousand persons)
- GenderID: 0 total, 1 men, 2 women
- NACE2008A21: sector code (0 is total, letters are economic sectors)
- NUTS: region code (BG31 BG32 BG33 BG34 BG41 BG42 are NUTS2 regions)
- LFS_EDUlevel: education level code (NSI coding)

## Method
- Selected the latest available quarter using max(periods)
- Filtered GenderID == 0 to analyse total employment
- For education analysis used age group Age10_LFS == "15 - 64_gr"
- Aggregated values by sector, region and education for the latest quarter
- Generated figures in reports/figures

## Key findings (latest quarter)
1. Total employment (Bulgaria, all sectors): add your number here
2. Top sector by employment: add sector name and value
3. Second sector by employment: add sector name and value
4. Highest employment region (NUTS2): add region name and value
5. Education distribution (15-64): largest group and value

## Limitations
- Official statistical data, not job postings data
- No salary information by position
- Sector, region and education categories depend on NSI coding
