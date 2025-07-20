### **🛒 Market Basket Analysis Project**

### 

#### **📑 Project Description**

#### 

Market Basket Analysis (MBA) is a popular technique used to uncover product purchase patterns in retail or e-commerce businesses. This project combines Python for data preparation and Power BI for interactive visualization, focusing on:



Frequent Itemset Extraction

Association Rule Generation

Cross-Sell Opportunities Identification





#### **🎯 Project Objectives**

#### 

* Extract frequent item combinations using Apriori Algorithm.
* Identify product pairs with high support, confidence, and lift using Association Rules.
* Build an interactive Power BI dashboard for business decision-making.
* Provide actionable recommendations to increase sales through product bundling.





#### **🔥 Key Features**

#### 

* End-to-End Workflow: From raw transactions → Association Rules → Dashboard.
* Python + Power BI Integration: Combines the best of both worlds.
* Two-Pages Clean Layout: Frequent Itemset Combination and Association Rules.



#### 

#### **💻 Tools \& Technologies Used**



* Python (Pandas , Mlxtend)
* Jupyter Notebook
* Power BI Desktop





#### **✅ Workflow Overview**



**1️⃣ Python Side: Market Basket Analysis**



* Data Preprocessing
* Remove Canceled Orders
* Group by Invoice and Product
* Transaction Encoding using mlxtend.preprocessing.TransactionEncoder
* Frequent Itemsets Extraction
* Using mlxtend.frequent\_patterns.apriori
* Minimum Support Threshold Applied
* Association Rules Generation
* Using mlxtend.frequent\_patterns.association\_rules
* Metrics Used: Support, Confidence, Lift
* Exporting Results to CSV for Power BI





**2️⃣ Power BI Side: Dashboard Building**



* Import Data: Import the processed CSV containing itemset and association rules.
* Page Layout Setup: Canvas Border + Theme Color: Light background + Purple borders.
* Title: MARKET BASKET ANALYSIS (Shape + Text box).
* Visualizations:

1. KPI Cards:
   Total Itemsets
   Max Support
   Max Confidence
   Max Lift
2. Treemap: Top 10 Itemsets by Support
3. Table: Rules Table with antecedents, consequents, confidence, lift, support.





#### **💡 Business Insights \& Recommendations**





##### ✅ Observations and Business Recommendations



1️⃣ Observation: Popular Product Combinations Identified



Finding:



Top frequent itemsets show high support for combinations like:



"WHITE HANGING HEART T-LIGHT HOLDER"



"JUMBO BAG RED RETROSPOT"





Recommendation:



* Create product bundles or combo packs for these popular items.
* Promote them on the homepage or in-store displays as “Most Loved Combos.”





2️⃣ Observation: High Lift Rules Highlight Strong Cross-Sell Opportunities



Finding:



Rules such as:



"ALARM CLOCK BAKELIKE GREEN" → "ALARM CLOCK BAKELIKE RED"



Lift Value: 24.03





Recommendation:



* Offer special bundle discounts for these combinations.
* Place these items next to each other in physical stores or add “Frequently Bought Together” sections online.





3️⃣ Observation: Single Item Dominance in Frequent Itemsets



Finding:



Some items appear repeatedly in multiple frequent itemsets as antecedents.





Recommendation:



* Treat these as anchor products in upselling strategies.
* Always suggest complementing products with anchor products on checkout pages.





4️⃣ Observation: Certain Item Combinations Have High Confidence but Low Support



Finding:



Example rule:



"SET/6 RED SPOTTY PAPER PLATES" → "SET/6 RED SPOTTY PAPER CUPS"



Confidence: 0.75



Support: Low (<1%)





Recommendation:



* Focus marketing efforts on niche or targeted customer segments.
* Use personalized email campaigns rather than general homepage promotions.





5️⃣ Observation: Products with Low Lift \& Low Confidence Exist



Finding:



Some rules have lift values close to 1.0, meaning no strong association.





Recommendation:



* Avoid prioritizing these combinations in bundling or marketing.
* Consider reviewing inventory and reducing stock for such slow-moving pairs.
