# Methodology Notes

## Why 44.8 minutes as the suspicious threshold?
Based on the data distribution, 78% of flagged cases occurred in Metropolitan areas.
A sub-45 minute delivery in a metro during adverse weather is physically improbable
during peak hours given traffic, building access, and parking constraints.
The 44.8 minute average emerged from the data — it was not pre-set.

## Risk Scoring Logic
Medium Risk = Delivery time < 60 mins AND (Weather = Stormy/Windy/Sandstorm OR Area = Metropolitan)
High Risk = Would require OTP fraud evidence — not available in this dataset

## Data Source
Kaggle Amazon Delivery Dataset — 43,739 records
Public dataset representing Indian last-mile logistics operations
