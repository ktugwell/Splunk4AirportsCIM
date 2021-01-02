# Passengers CIM

Fields in the CIM are compiled mainly from the ACRIS and IATA standards. A-CDM does not have many suitable conventions for passenger related data. To see more about the data sources used, see the [about](./About.md) page.

| Dataset Name  | Field Name  | Data Type | Description | Examples |
|:--------------|:------------|:----------|:------------|:---------|
| Security      | passengerName | String(<=20)  | Passenger name - Following IATA Passenger Services Resolution Manual format | TUGWELL/KL MR |
| Security | from | String | The departing airport and/or country | Gatwick, London |
| Security | to | String | The arriving airport | Amsterdam, Schiphol |
| Security | airline | String | The IATA code of the airline, sometimes called "Carrier" | EZY |
| Security | flightNumber | int(4) | The flight number | 1234 |
| Security | FQFC | String | The Fully Qualified Flight Code, a concatenation between airline and flightNumber | EZY1234 |
| Security | seat | String | The seat the passenger will occupy on the flight | 17B |
| Security | passengerGate | String | The public gate the aircraft is departing from | 10A |
| Security | boardTime | int(4) | 4 digit 24hr time format scheduled boarding time of the flight | 0900 |
| Security | BPSOBT | String | The scheduled off block time as printed on the boarding pass. The IATA standards does *not* include the year, so it's better to link the flight from the Airfield dataset to this record if you wish to do year-on-year analysis. | 01JAN0900 |
| Security | class | int(1) | The class of travel - refer to PADIS Codeset 9873 | 1, 2, 3 |
| Security | dateOfIssue | String | The date the boarding pass was issued. DDMONYY | 01JAN21 |




[Contents](./contents.md)<br />
[Home](./)