# Problem Statement
Amazon catalog consists of billions of products that belong to thousands of browse nodes (each browse node represents a collection of items for sale). Browse nodes are used to help customer navigate through our website and classify products to product type groups. Hence, it is important to predict the node assignment at the time of listing of the product or when the browse node information is absent.

As part of this hackathon, you will use product metadata to classify products into browse nodes. You will have access to product title, description, bullet points etc. and labels for ~3MM products to train and test your submissions. Note that there is some noise in the data - real world data looks like this!!

Data Description

Full Train/Test dataset details:

Key column – PRODUCT_ID
Input features – TITLE, DESCRIPTION, BULLET_POINTS, BRAND
Target column – BROWSE_NODE_ID
Train dataset size – 2,903,024
Number of classes in Train – 9,919
Overall Test dataset size – 110,775
Important Note:

In case you are using pandas to read the csv train and test datasets, use escapechar = "\\" and quoting = csv.QUOTE_NONE options with read_csv to avoid errors during import.

## Solution:
This problem is the multiclass problem. It is solved by using two methods.

1. Information Retrieval
2. Using H2O