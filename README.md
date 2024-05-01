All the operations in this project are given below:
 • AWS Lambda function, executed at defined intervals via AWS CloudWatch, to retrieve data from the Spotify Web
 API and seamlessly put into an S3 bucket.
 • Another AWS Lambda function triggered when S3 new json gets staged, which efficiently converts raw JSON data into
 structured CSV files and transfers them to another S3 bucket.
 • Snowpipe seamlessly loads newly transformed data from the S3 staging area to Snowflake tables, that triggers via S3
 event notification.
 • Developed a Tableau dashboard presenting insights on the top 100 songs globally, derived from transformed data,
 offering concise and comprehensive visualization.
