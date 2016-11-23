# sg-retirement-pension
Number of State Pension claimants in Edinburgh by age and gender.

State Pension is available to people who have reached State Pension age, currently 60 for women and 65 for men. 

Pensions are based on National Insurance (NI) contributions. Additional money is paid to those aged 80 and over. A married personwho does not qualify fora full State Pension based on their own NI contributions, may be able to get a pension based on their spouse's NI record. For detailed eligibility conditions and rules for claiming State Pension see the pension service website: http://www.thepensionservice.gov.uk/ 

Data shown here are derived from a 100% data source; the Work and Pensions Longitudinal Study (WPLS) which is not subject to any sampling error. The dataset provides counts of total claimants and breakdowns by age and gender from a snapshot in time and will therefore exclude a small number of clerically held cases. The snapshots are taken at quarterly intervals at the end of February (Q1), May (Q2), August (Q3) and November (Q4). The data in the WPLS datasets are not directly comparable to the annual individual level data previously released as they were a single snapshot at a point in time and did not reflect late notifications and removals from the systems. Every effort has been made by the DWP to ensure that data do not allow the disclosure of confidential information and all counts have been adjusted using a variant of controlled rounding to base 5. Any counts that are shown as zero may not be a real zero. 

Source: Department for Work and Pensions. Comprehensive information on Working Age Claimants is available from the DWP tabulation tool http://www.dwp.gov.uk/asd/tabtool.asp.

Statistics provided by Scottish Government:  http://statistics.gov.scot/data/retirement-pension

## License

Data is licensed under the Open Government License: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/

## Requirements

- NodeJS
- npm

## Installation

Clone the repository

```
git clone https://github.com/EdinburghCityScope/sg-retirement-pension.git
```

Install npm dependencies

```
cd sg-retirement-pension
npm install
```

Run the API (from the sg-retirement-pension directory)

```
node .
```

Converting the extracted data into loopback data.

```
node scripts/featureCollectionToLoopbackJson.js
```

Re-build data files from the statistics.gov.scot API

```
node scripts/build-data.js
```
