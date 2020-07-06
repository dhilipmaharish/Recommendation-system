# Recommendation-system
Amazon Apparel Recomdation system

Objective of the Project:

Recommending the similar product (apparel) to the given product(apparel) by the user in the E-commerce websites.The process of algorithm is based on two features. They are
1.Title/Text Based recommendation system
2.Image based recommendation system
Each product/item has 19 features in the raw dataset out of these 19 features, we will be using only 6 features

1. ASIN ( Amazon standard identification number)

2.brand ( brand to which the product belongs to )

3,color ( Color information of apparel, it can contain many colors as a value ex: red and black stripes )

4.product_type_name (type of the apparel, ex: SHIRT/T SHIRT )

5.medium_image_URL ( URL of the image )

6.title (title of the product.)

7.formatted_price (price of the product)

Work process:

Step 1: The product image id and the product id is collected using the web scraping on the amazon api web-page

Step 2: Data cleaning

Step 3: separating the title features:
Done some of the text preprocessing like stop-words removal,stemming.

Step 4: Text based Recommending features
In this step text is converted into vector using some of the NLP techniques like Bag of Words,TF-IDF,sentiment analysis Word2vec and the identified closest vector(increase in similarities and decrease in distance) by using the Euclidean distance concept.

Step 5:Image Based Recommending Features.
In this step using Transfer learning (means using already processed algorithm on some other data),here use VGG(Visual Geometry Group) 16 CNN algorithm to convert images data into vectors.

Step 6: combining both Text/Tile features and image features
For flexibility in the system I combined both the features and provided weights for each features based on more weight the product is recommend with heavy weight features.

The project link is provided below you can refer it.
