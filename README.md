# VS Electronics: a webscraping project

## The e-commerce domain in Germany

E-commerce was invented around 40 years ago, and has been booming in the last 20. The products are simply displayed on a website, 24/7 and 365 days a year, and can be easily bought with a couple of clicks. E-commerce has helped countless businesses grow with the help of new technologies, faster internet connection speeds, and added payer security features.
There are three main e-commerce types:

a) B2C (Business to Customer) is the most common type of e-commerce. For example, electronics from Amazon or Otto.de.

b) B2B (Business to Business) is often done between manufacturers and retailers. It focuses on raw materials.

c) C2C (Consumer to Consumer) is one of the earliers forms of e-commerce. Ebay is one of the best examples.

The main advantages of e-commerce are:

1) Customers can buy your products much faster than in traditional retail.

2) It is easier to reach new customers via targeted ads.

3) The overall shipping costs are lower since all the products can be kept in a single warehouse instead of different shops.

Currently, e-commerce is booming in Germany. A vast majority of the population has an internet access and the logistics infrastructure is excellent. In 2018, Germany was the second e-commerce market in Europe after the UK and the fifth in the world. The e-commerce platforms that Germans use the most are Amazon, Otto and Zalando. Moreover, possible direct competitors for the electronics market are Notebooksbilliger, MediaMarkt, Cyberport and Conrad.

Both the average conversion rate (purchases/visits) and the average order price are higher than the average in Germany. Also the number of mobile transaction is remarkable, since they make up 40-50% of the total volume. 

The biggest problem faced by German e-commerce in the last years is privacy and security issues. These problems were partly solved via the new European GDPR, which however in turn reduced German e-commerce temporarily by 10%. Moreover, strict laws on purchase returns have led to an impressive return rate, of up to 70% 

The biggest opportunity for e-commerce consists in the global pandemic, which has forced people to stay at home and only shop online. It is predicted that e-commerce will soar by approximately 15% due to this.

Moreover, the biggest e-commerce market in Germany consists in electronics and media. Therefore it is a great idea for VS Electronics to take this road as well.

All in all, the German e-commerce business appears to be in excellent health and to provide great opportunities in the field.

## The concept of webscraping

The web works like follows: first of all, you type a domain into your browser. This domain name gets first translated into an IP address via a DNS server. 
Then, the browser goes ahead and makes a request to the server with the IP address, sending the data via a protocol known as HTTP. 
After that, the server will send a response, that is, it returns the code to display the website. 
The browser will then parse this response using the HTTP protocol and display the page. 

What does beautiful soup do? 

Beautiful Soup 4 pulls data out of HTML and XML files. Its main aim is to fetch data and create databases out of it, automatizing a manual process which would be time-consuming and annoying. This allows us to do data mining in a fraction of the time in order to create datasets, test or train algorithms or machine learning models. Sometimes, a website offers API's which are the best way of fetching data. However, sometimes they aren't available or you want to bypass the registration process. 

The main problem with webscraping is that often websites do not like to have their data harvested automatically. Therefore, they will deny your requests once they have reason to suspect that a bot is doing them (e.g. by doing too many requests in a short period of time). Another important issue is legal problems. It is highly illegal (and unethical) for example to webscrape social networks such as Facebook. For consumer data (e.g. Amazon), it is just illegal to sell the data or any analysis, while it is legal to webscrape for didactical purposes. This is because any commercial entity has high interest in webscraping its rivals' offer in order to compare it with its own. 

## Beautiful Soup: technical details

To import the data, we need requests.get(). We then need json() to parse the data. The data we got is in the form of a dictionary, and we then need to call the key of the value to get the value itself. 

print(data) gives the code of the response. If the download worked correctly, we would get <Response[200]>. <Response[404]> on the other hand means the page doesn't exist. To get the status code (200/404) only, you can also use print(data.status_code).

To write your response to a file, you can do:
file = open("xyz.txt", "w")
file.write(response.text)
file.close()
