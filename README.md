ca_housing_analytical_matrix.csv is the original CSV Brett shared

Currently at (144299 rows, 23 columns)

Columns:

['brokered_by', 'status', 'price', 'bed', 'bath', 'acre_lot', 'street', 'city', 'state', 'zip_code', 'house_size', 'prev_sold_date', 'sold_year', 'sold_month', 'median_hh_income', 'urban_density_ratio' 'state_in_migration_rate', 'west_cpi_inflation', 'us_30yr_mortgage_rate', 'ca_unemployment_rate', 'log_price','log_house_size', 'is_cost_burdened']


---------------------------------------------------------------


realtor-data-ca.csv is the Kaggle data set (176KB) filter down to Califoria state only to fit into the repository 

Current shape is (227215 rows, 12 columns)

https://www.kaggle.com/datasets/ahmedshahriarsakib/usa-real-estate-dataset?resource=download

Columns:

['brokered_by', 'status', 'price', 'bed', 'bath', 'acre_lot', 'street', 'city', 'state', 'zip_code', 'house_size', 'prev_sold_date']


---------------------------------------------------------------


ca county population 2020-25.csv is the E-2. California County Population Estimates and
Components of Change by Year — July 1, 2020-2025 that accounts for population for each year from 2020 to 2025 for 58 different counties 

https://dof.ca.gov/forecasting/demographics/estimates/E-2/

Columns:

['County', 'Revised  July 1, 2020', 'Revised  July 1, 2021', 'Revised  July 1, 2022', 'Revised  July 1, 2023', 'Revised  July 1, 2024', 'Preliminary  July 1, 2025']

Counties:

Alameda, Alpine, Amador, Butte, Calaveras, Colusa, Contra Costa, Del Norte, El Dorado, Fresno, Glenn, Humboldt, Imperial, Inyo, Kern, Kings, Lake, Lassen, Los Angeles, Madera, Marin, Mariposa, Mendocino, Merced, Modoc, Mono, Monterey, Napa, Nevada, Orange, Placer, Plumas, Riverside, Sacramento, San Benito, San Bernardino, San Diego, San Francisco, San Joaquin, San Luis Obispo, San Mateo, Santa Barbara, Santa Clara, Santa Cruz, Shasta, Sierra, Siskiyou, Solano, Sonoma, Stanislaus, Sutter, Tehama, Trinity, Tulare, Tuolumne, Ventura, Yolo, Yuba.


--------------------------------------------------------------------


hpi_at_county.csv is House Price Index that is comprehensive​ collection of publicly available house price indexes that measure changes in single-family home values based on data that extend back to the mid-1970s and includes all 58 counties in CA as well after filtering.

 https://www.fhfa.gov/data/hpi/datasets

Columns: 

['State', 'County', 'FIPS code', 'Year', 'Annual Change (%)', 'HPI', 'HPI with 1990 base', 'HPI with 2000 base']

hpi_at_zip5.csv is virtually the same but my Zip code, may be an easier merge onto the real estate unless we expand a county column onto real estate for our joins

Columns:

['Five-Digit ZIP Code', 'Year', 'Annual Change (%)', 'HPI','HPI with 1990 base', 'HPI with 2000 base']


---------------------------------------------------------------------------------


CAINC4_CA.csv is the BEA Personal Income by County Dataset provides annual estimates of total personal income, per capita personal income, and income by major source (wages, proprietors' income, dividends, interest, rent, and government transfers) for every county in the United States. 

CAINC4 = Personal Income and Employment by Major Component by County (Confirmed 58 Counties)

https://www.bea.gov/data/income-saving/personal-income-by-county

More Important Rows:

["Per capita personal income (dollars) 4/",
    "Wages and salaries ",
    "Personal income (thousands of dollars)",
    "Equals: Net earnings by place of residence ",
    "Plus: Dividends, interest, and rent 7/",
    "Population (persons) 3/"]