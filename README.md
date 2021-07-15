# 10K-10Q-NLP-Project

Analyzing the quarterly 10K/10Q reports from companies. As the project stands right now, I will be more specifically looking at these reports from airlines domiciled in USA. I view the industry as a zero-sum game, which means that even the slightest sentimental difference between reports can be exploited. More information can be found here: https://medium.com/@spandey16/game-theory-and-the-airline-business-865f0a5f0f5b

A 10-K provides investors with information including an outline of the company's business, the risks the company faces, and operating/financial results for the past fiscal year. It is divided into 4 parts which contain a total of 15 items. 

For the sake of this project, I will initially be looking at the largest airline in America: American Airlines ($AAL). Here are some initial thoughts:

## Part 1

I believe in this case, much of the information required to extract alpha is not found here. While an overview of the business as a whole is important, many of these ideas are explored in more depth in later sections of the filing. For example, the section regarding COVID-19 is explored in far more depth in the proceeding section, ITEM 1A.

### Part 1A

This section outlines the risks related to the business. Naturally, at the very top is information about the COVID-19 pandemic. Here is an overview of the risks:

* COVID has severely impacted the business effectively cutting demand by more than half, forcing the company to retire aircraft earlier than expected, forcing the company to furlough employees, ask for government financial assistance, raise capital by issuing securities on the open market, etc. 
* High levels of debt may hinder ability to acquire additional financing, which the company says they **need** in order to operate successfully
 * Unhedged interest rate exposure? See PDF page 55.  
* Liquidity problems may arise from pension (etc.) obligations and obligations towards advance ticket sales
 * Credit card companies may withhold part of the payment until service has been provided (many refunds as well are occurring)
* Loss of key personnel/inability to attract talent
* Economic conditions beyond control
 * Covid is mentioned here again, naturally, but also includes topics such as geopolitical events, interest rate events, disease outbreaks, and other so-called Acts of God
* Union disputes
 * I can imagine that events such as this are stochastic and cannot necessarily be controlled for. Each airline has many unions representing their employees, each with their own mandates. 
* Problems with third-party regional operators
 * Third party operators can suffer from similar risks, thus creating a service outage in a strategic area
 * Service providers including maintenance and ground services can also pose such risks
* Damage to reputation/brand image
 * Hard to control for in a systematic way (I assume) 
