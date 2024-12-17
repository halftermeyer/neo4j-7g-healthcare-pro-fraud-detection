# neo4j-7g-healthcare-pro-fraud-detection

## Dataset presentation

This is a synthetic dataset created as a demo to address french insurance companies.
It contains data about healthcare professionals and the way they interact between each other and with patients (Beneficiary in the insurance company perspective).

## Database presentation

#### In the same database lives the data for several use cases:

- Healthcare professional fraud detection
- Healthcare professional fraud investigation

![healthcare_model](https://github.com/halftermeyer/neo4j-7g-healthcare-pro-fraud-detection/blob/main/media/healthcare_model.png?raw=true)

- Case Management

![case_mngt_model](https://github.com/halftermeyer/neo4j-7g-healthcare-pro-fraud-detection/blob/main/media/case_mngt_model.png?raw=true)


- KYW - Know Your Whoever

![kyw_model](https://github.com/halftermeyer/neo4j-7g-healthcare-pro-fraud-detection/blob/main/media/kyw_model.png?raw=true)

- HR database


![hr_model](https://github.com/halftermeyer/neo4j-7g-healthcare-pro-fraud-detection/blob/main/media/hr_model.png?raw=true)

#### The dataset could be upgraded for other use cases like:

- Healthcare insurance beneficiary fraud detection (not in the demo)
- Fire, Accidents and Miscellaneous Risks
- AML/CFT

## Demo presentation
#### The demo is broken down into parts:
- NeoDash-based app for:
  - Know Your Healthcare professional (Pro 360)
    [![video of pro 360](https://img.youtube.com/vi/dMyeZlyMNMo/0.jpg)](https://www.youtube.com/watch?v=dMyeZlyMNMo)
  - Fraud detection scenarios: they are part of the Pro 360 view (Investigation) and some are also processed at the whole database scale in dedicated tabs (Detection).
    - Unlikely association of cares during same visit
    [![Unlikely association](https://img.youtube.com/vi/uub31K26SSU/0.jpg)](https://www.youtube.com/watch?v=uub31K26SSU)
    - Suspicious distance Pro/Beneficiary
    [![Suspicious distance Pro/Beneficiary](https://img.youtube.com/vi/yHFxZcJOyNQ/0.jpg)](https://www.youtube.com/watch?v=yHFxZcJOyNQ)
    - Repeated same acts by a Pro
    [![Repeated same acts by a Pro](https://img.youtube.com/vi/QhO74O4Cf8s/0.jpg)](https://www.youtube.com/watch?v=QhO74O4Cf8s)
    https://youtu.be/QhO74O4Cf8s
    - Prescriber to Executor suspicious flow
    - Prescriber and Executor are the same person
  - Case Management: a case can be created in the Pro 360 tab and cases are visible in the Case Management tab
    [![Case Management](https://img.youtube.com/vi/w0mxS5Laf1g/0.jpg)](https://www.youtube.com/watch?v=w0mxS5Laf1g)
    
- Bloom-based investigation:
  - *show investigations* search phrase
  - lasso selection
  - *show common PIIs* scene action [there's a twist here]
  - *label fraudulent* scene action