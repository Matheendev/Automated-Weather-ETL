<!DOCTYPE html>
<html>
<head>
</head>
<body>
<h1>About the Project</h1>
<p>This project aims to establish a robust and automated ETL pipeline to efficiently extract, transform, and load weather data from an external API into an AWS S3 bucket. By leveraging Apache Airflow, the pipeline ensures reliable scheduling and execution of the ETL process. Real-time notifications are sent via Slack to provide updates on successful data uploads to the S3 bucket.</p>

<h2>Tech Stack</h2>
<ul>
<li>Apache Airflow: Orchestrates and manages the ETL workflow.</li>
<li>Amazon Web Services (AWS): Provides cloud infrastructure for data storage AWS Simple Storage Service (S3) and AWS Elastic Cloud Compute (EC2) to run Airflow using Ubuntu OS.</li>
<li>Python: Used for data extraction, transformation, and loading logic.</li>
<li>Slack: For real-time notifications of ETL process completion.</li>
</ul>

<h2>Architecture</h2>

![weather_ETL_Airflow](https://github.com/user-attachments/assets/9c42fbb5-388d-4d0f-b1ae-1db2f6315e8f)

<h2>Working of the Project</h2>
<p>The ETL pipeline follows these steps:</p>
<ul>
<li><strong>Extraction:</strong> Weather data is fetched from the specified API using Python.</li>
<li><strong>Transformation:</strong> Extracted data undergoes necessary transformations to align with desired output format.</li>
<li><strong>Loading:</strong> Transformed data is loaded into the designated S3 bucket on AWS.</li>
<li><strong>Notification:</strong> A Slack message is sent upon successful data upload to the S3 bucket.</li>
</ul>
<p>Airflow orchestrates these steps, ensuring timely execution and recovery from failures.</p>

<h2>Airflow DAG Graph</h2>

![DAG graph](https://github.com/user-attachments/assets/61cdbc76-ffe0-4128-9695-78746c6dc698)

<h2>Impact of the Project</h2>
<ul>
<li>Improved data accessibility: Real-time weather data is readily available for downstream applications and analysis.</li>
<li>Increased efficiency: Automation of the ETL process saves time and reduces manual effort.</li>
<li>Enhanced data reliability: Regular data updates and error handling mechanisms ensure data quality.</li>
<li>Real-time monitoring: Slack notifications provide immediate feedback on pipeline status.</li>
</ul>
</body>
</html>

