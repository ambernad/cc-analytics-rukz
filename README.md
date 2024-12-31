# Contact center analytics solution in RU and KZ languages
1. Create S3 bucket
2. Upload files from Data folder of this repository to your bucket
3. Create Sagemaker domain. Ensure that its execution role has permission to read from S3 Bucket, call Bedrock models and initiate Transcribe jobs
4. In Sagemaker domain create Studio and Jupyter Lab instance.
5. Import cc-analytics-rukz-notebook.ipynb from this repository to your JupyterLab. In notebook change bucket names to yours.
6. Enable Claude Sonnet 3.5 model in Bedrock
7. Run notebook in JupyterLab
8. Check that output csv file with analytics results was created in the output bucket
9. Optionally, set up table in Glue catalog and query your results with Athena
10. Optionally, set up Quicksight account and visualize metrics from output csv-file
