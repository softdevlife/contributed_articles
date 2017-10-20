
**Original Article can be found at @weidongzhou:** https://weidongzhou.wordpress.com/2017/06/10/google-cloud-sql-vs-cloud-datastore-vs-bigtable-vs-bigquery-vs-spanner/

I like the decision tree made by Google Cloud. For analysis, I love NoSQL databases like Bigquery (and Redshift) for its aggregation and dumping capabilities to google cloud storage and S3 respectively.

Sometimes, people want to fetch individual records with a mass amount of joins, which even normal relational databases cannot handle and do not make sense to run them in a columnar database due to their huge costs. I would love Spanner have no overhead costs and be a pay as you go serverless model like Bigquery, but it seems the architecture of most standard SQL environments are resource intensive with only incremental updates and no paradigm shifts. No wonder they call Spanner as "NewSQL".

About the post below: Overhead costs for Bigtable are recently introduced as you now need to rent a minimum of 3 nodes. Price changes are hard to keep track of. Thankfully, Google has an all-in-one calculator to its cloud services that gets updated on a regular basis: https://cloud.google.com/products/calculator/

![0-jzmmfy-htugwlvzx-](https://user-images.githubusercontent.com/12673581/31823433-bd83c22e-b5de-11e7-85a1-dbb069d8b336.png)
