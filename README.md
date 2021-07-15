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
  * Perception of safety of travel 
* Accidents involving operations
  * Another event that may be difficult to control for in a look-ahead way, consider the 737 MAX crashes and their impact on airlines
* Challenges involving integration of technology
  * Not very idiosyncratic
* Challenges involving promotions or business models that are designed to increase revenues
  * This is something that is idiosyncratic and has certainly affected airlines before (consider the infamous unlimited AAirPass)
* Problems arising from theft of intellectual property and branding rights
  * Not very idiosyncratic
* Litigations from regular course of business
  * Unsure about this one, there can be lawsuits mentioned that are severe and quite idiosyncratic, however every airline will likely have similar lawsuits
* Net Operating Losses (NOL) tax deductions which can be carried forward can expire if unused
  * Not idiosyncratic whatsoever
* Full value of goodwill may not be realized
  * Again, this may be something that is difficult to control for

The next section speaks about risks related to the airline industry as a whole. If this project evolves into a long/short strategy like I plan, many of these aspects will be controlled for. However, in this section there are also aspects unique to the company listed including marketing relationships, joint business information, etc.


## Part 2: Properties

Naturally, the change in number of planes both owned and leased is very important to the business, both at full capacity, and at limited capacity i.e. during COVID. Having less planes is preferable during COVID because these assets depreciate, and without providing revenue, the company is forced to pay storage and maintenance costs and receive nothing in exchange. This is why some planes were forced to be retired during COVID. 

## Part 3: Legal Proceedings

This is perhaps of some great value to our analysis. Lawsuits can be generally idiosyncratic to companies, however, I'm not sure how material the decisions and outcomes are in general. This is something I will need to investigate. #ToDo

## Part 4: Mine Safety Disclosures

Not applicable.

## Part 5: Common Stock Information

Dividends and share repurchases are important drivers of a stock price (fundamentally). It also gives investors a general idea of how the company is performing. For example, raising a dividend generally indicates that revenues are up and the company is in a financially good position. Share repurchases indicate that the company fundamentally believes their shares are undervalued. Repurchases can allow the company to increase its own equity stake, or the shares could be retired. In any case, repurchases generally benefit investors by raising many important per-share accounting figures such as Earnings-Per-Share (EPS). 

## Part 6: Selected Consolidated Financial Data

While not necessarily natural language, these numbers will allow us to compare companies quantitatively. Naturally, the magnitude of the numbers may not be as relevant as the percent changes, since the big 4 airlines are different in size. (#ToDo verify this makes sense). 

The non-GAAP special items will also need to be verified. I'm not sure if these can be used to compare companies or not. #ToDo

The Operating Costs per Available Seat Mile (CASM) table may be extremely useful as these are the most important drivers of the companies, adjusted for the most important aspect of airfare (available seat-mile). 

## Part 7: Management's Discussion and Analysis

This section will be extremely important for any type of NLP task. It appears to offer commentary on the financial health of the company directly from management. Naturally, if management has a negative sentiment, then we know for sure that the company is not doing well. 
