# Bitcoin Tulip Trust Analysis

## Data

- Source: https://storage.courtlistener.com/recap/gov.uscourts.flsd.521536/gov.uscourts.flsd.521536.512.7.pdf
- 16404 Extracted addresses: [addresses.txt](addresses.txt)
  1. `pdftotext gov.uscourts.flsd.521536.512.7.pdf parsed.txt`
  2. `cat parsed.txt | grep -oP '^[1][a-km-zA-HJ-NP-Z1-9]{25,34}$' > addresses.txt`

## Disclaimer

It hasn't been verified that the addresses are actually part of the Tulip trust! There are even some addresses that are most likely not part of the trust: https://archive.md/Z1oB8 ([invalid_addresses.txt](invalid_addresses.txt)).

## TODO

Collect metrics for all addresses on the chains BTC, BCH, BSV:

- Total balance
- Total transferred out amounts
- Address activity dates
