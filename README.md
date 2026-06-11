# RANDE NY — Sample Notebook

Sample notebook for the **RANDE NY** race/ethnicity imputation model package on AWS Marketplace.

Deploy the model in your own AWS account (real-time endpoint or Batch Transform) and call it:
- **Input:** CSV — `fname,mname,lname,housenumber,street,city,state,zip` (New York addresses)
- **Default output:** privacy-preserving aggregate race/ethnicity summaries by census tract and ZCTA (White/Black/Hispanic/Asian + unclassified residual)
- **Per-row output:** set request header `X-Amzn-SageMaker-Custom-Attributes: mode=rows`

See [`rande_ny_sample.ipynb`](rande_ny_sample.ipynb).

> Outputs are statistical estimates of the race/ethnicity signaled by name and geography — not statements of any individual's actual or self-identified race. New York State scope. See the product EULA.
