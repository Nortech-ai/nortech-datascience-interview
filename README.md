# Nortech Data Science Interview Challenge: Power Output Prediction

## Introduction
Welcome to the Nortech Data Science Interview Challenge. Nortech specializes in installing IoT devices on customer assets across various sectors, including marine, industrial, and logistics. These IoT devices collect data from the assets, which is stored both locally and in the cloud. This data enables our customers to visualize and utilize it for operational optimization, reducing costs and carbon emissions.

Read more about Nortech [here](https://nortech.ai/).

## Challenge Overview
In our marine division, we encounter a critical challenge: **Vessel A** lacks direct power output measurements from its main engine, which are vital for calculating important performance and health KPIs, such as Hull Propeller Performance, Fuel Efficiency, and Trim Optimization. However, we do have access to several sensor readings from the engine that could potentially be used to estimate power output.

Contrastingly, **Vessel B** is equipped with a power measurement sensor and several other sensors that overlap with those on Vessel A.

Additionally, we have conducted **engine shop trials** for both Vessel A and Vessel B. During these trials, the vessel's engine is run at various setpoints, and several sensors are measured, including the power output. These trials aim to test the engine's performance at those setpoints.

### Goal
Your challenge is to predict the power output of **Vessel A** using the available data. The ideal solution will leverage the sensor readings from Vessel A, the data from Vessel B, and the insights gained from the engine shop trials.

## Data Description
The dataset includes sensor readings from **Vessel A** and **Vessel B**, along with the results from the engine shop trials for both vessels. Here is a brief overview of the dataset structure:

- [Vessel A Data](nortech_datascience_interview/data/vessel_a_data.parquet): Sensor readings from Vessel A (excluding power output measurements).
- [Vessel A MetaData](nortech_datascience_interview/data/vessel_a_metadata.json): Metadata of sensor readings from Vessel A.
- [Vessel A Engine Shop Trials Data](nortech_datascience_interview/data/vessel_a_engine_shop_trials_data.csv): Results from the engine shop trials for Vessel A.
- [Vessel B Data](nortech_datascience_interview/data/vessel_b_data.parquet): Sensor readings from Vessel B, including power output measurements.
- [Vessel B MetaData](nortech_datascience_interview/data/vessel_b_metadata.json): Metadata of sensor readings from Vessel B.
- [Vessel B Engine Shop Trials Data](nortech_datascience_interview/data/vessel_b_engine_shop_trials_data.csv): Results from the engine shop trials for Vessel B.

The dataset is only for use in the challenge and any other use is not permitted.

## Evaluation Criteria
Your submission will be evaluated based on the following criteria:
- **Accuracy**: How well does your model predict the power output of Vessel A?
- **Innovativeness**: How creative and effective are the approaches you used to tackle the challenge?
- **Clarity**: How well do you explain your assumptions, decision-making process, and the impact of your choices?
- **Reproducibility**: Can your results be easily reproduced using your provided code and methodology?

## Submission Guidelines
Please include the following in your submission:
- **Code**: All the code you used in the challenge.
- **Documentation**: A clear explanation of your approach, including assumptions made and reasons for your decisions.
- **Results**: A summary of your findings and any recommendations for further investigation or improvements.

Submissions should be a [pull request](https://github.com/Nortech-ai/nortech-datascience-interview/pulls) to this repository until the deadline: **April 30, 2024**.

After reviewing your submission, we may try to schedule a meeting where it will be expected for you to do a small 5-10 minute presentation of your findings followed by a discussion on the results and the challenges you faced.

## Getting Started
To get started with the challenge, clone this repository and explore the datasets provided in the `data` folder.

To install the project, run the following command:

```bash
poetry install
```

This will install all the required dependencies and create a virtual environment for the project.

If you are not familiar with poetry, you can learn more about it [here](https://python-poetry.org/).

Feel free to add any additional dependencies as needed. You can use any tool or library that you are familiar with (Jupyter Notebook, Pandas, NumPy, Scikit-learn, Plain Python, etc.).

## Support
Should you have any questions or require clarification, please do not hesitate to open an [issue](https://github.com/Nortech-ai/nortech-datascience-interview/issues) in this repository or contact us at [challenge@nortech.ai](mailto:challenge@nortech.ai).

Good luck, and we look forward to your innovative solutions!
