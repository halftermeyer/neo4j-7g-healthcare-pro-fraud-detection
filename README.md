# neo4j-7g-healthcare-pro-fraud-detection

## Dataset presentation

This is a synthetic dataset created as a demo to address french insurance companies.
It contains data about healthcare professionals and the way they interact between each other and with patients (Beneficiary in the insurance company perspective).

## Database presentation

#### In the same database lives the data for several use cases:

- Healthcare professional fraud detection

![alt text](https://github.com/halftermeyer/neo4j-7g-healthcare-pro-fraud-detection/blob/main/media/image.jpg?raw=true)

- Healthcare professional fraud investigation
- Case Management
- KYW - Know Your Whoever
- HR database

#### The dataset could be upgraded for other use cases like:

- Healthcare insurance beneficiary fraud detection (not in the demo)
- Fire, Accidents and Miscellaneous Risks
- AML/CFT

## Demo presentation
#### The demo is broken down into parts:
- NeoDash-based app for:
  - Know Your Healthcare professional (Pro 360):
  - Fraud detection scenarios: they are part of the Pro 360 view (Investigation) and some are also processed at the whole database scale in dedicated tabs (Detection).
    - Unlikely association of cares during same visit 
    - Suspicious distance Pro/Beneficiary
    - Repeated same acts by a Pro
    - Prescriber to Executor suspicious flow
    - Prescriber and Executor are the same person
  - Case Management: a case can be created in the Pro 360 tab and cases are visible in the Case Management tab
- Bloom-based investigation:
  - *show investigations* search phrase
  - lasso selection
  - *show common PIIs* scene action [there's a twist here]
  - *label fraudulent* scene action