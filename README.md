# Construction ML Models from Dissertation

This repository contains deployable .jar files for machine learning models from the dissertation "The Evolution and Forecasting of Satisfaction & Project Success in Construction." These models predict cost/duration deviations and satisfaction based on project attributes. All models use the same input.csv and output.csv file names for consistency.

## Models Included
- model-01-cost.jar: For Cost Deviation Percentage.
- model-02-duration.jar: For Duration Deviation Percentage.
- Contractor Models:
  - model-04-contractor-oversight.jar: Contractor Satisfaction with Oversight & Coordination of Subcontractors.
  - model-05-contractor-conflict.jar: Contractor Satisfaction with Handling Conflict.
  - model-06-contractor-material.jar: Contractor Satisfaction with Solving Material Supply Problems.
  - model-07-contractor-communication-client.jar: Contractor Satisfaction with Communication Quality with Client.
  - model-08-contractor-communication-subs.jar: Contractor Satisfaction with Communication Quality of Subcontractors, Suppliers & Regulatory Agencies.
  - model-09-contractor-teamwork.jar: Contractor Satisfaction with Level & Quality of Contractor Teamwork.
  - model-10-contractor-site-management.jar: Contractor Satisfaction with Level & Quality of Site Management.
  - model-11-contractor-initiation.jar: Contractor Satisfaction with Initiation Stage with Work by Client.
  - model-12-contractor-planning.jar: Contractor Satisfaction with Planning Stage.
  - model-13-contractor-execution.jar: Contractor Satisfaction with Execution, Monitoring & Control Stages by Contractor Team.
  - model-14-contractor-closing.jar: Contractor Satisfaction with Closing Stage Client Interactions.
- Client Models:
  - model-15-client-specifications.jar: Client Satisfaction with Adherence to Specifications.
  - model-16-client-workmanship.jar: Client Satisfaction with Workmanship Quality.
  - model-17-client-planning.jar: Client Satisfaction with Planning Stage Progress.
  - model-18-client-execution.jar: Client Satisfaction with Execution, Monitoring & Control Stages Progress.
  - model-19-client-closing.jar: Client Satisfaction with Closing Stage Progress.
  - model-20-client-relationship.jar: Client Satisfaction with Relationship Quality with Contractor.
  - model-21-client-communication.jar: Client Satisfaction with Communication Quality with Contractor.
  - model-22-client-overall.jar: Client Satisfaction Overall.
- input.csv: Sample input file with headers (e.g., PFS, CYE, PIU, RMU).

## Requirements
- Java Runtime Environment (JRE) 8+ (download from https://www.oracle.com/java/technologies/downloads/).
- Windows PowerShell or terminal.

## Setup and Usage
1. Download the repo as ZIP or clone it (git clone https://github.com/TDoerga/construction-ml-models.git).
2. Edit input.csv with your data (e.g., PFS = "Public", CYE = 20).
3. Open PowerShell, navigate to the folder (cd path/to/repo).
4. Run: java -jar model-01-cost.jar -input input.csv -output output.csv
   - For other models: java -jar model-04-contractor-oversight.jar -input input.csv -output output.csv (use the same input/output names for all).
5. Open output.csv to view outputs (e.g., predicted CDP or satisfaction score).

## Troubleshooting
- Java not found? Add to PATH or run with full path (e.g., C:\Program Files\Java\jre\bin\java -jar ...).
- Errors? Ensure CSV headers match model features (list in template notes).
- Contact: For questions, email [tarun.doerga@utt.edu.tt].

Note: Models are approximations; test with your data for accuracy.
