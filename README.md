# Amazon Health & Baby Care Ranking Analysis

## 📝 Project Overview  
This project investigates **what factors influence product ordering in Amazon’s Health & Baby Care search results**. Using data scraped from Amazon’s public site, we explored how visible product attributes—like ratings, reviews, prices, and recent demand—relate to product ranking.

---

## 🔍 Data Collection  
- **Scope:** Health & Baby Care categories across 8–14 subcategories each.  
- **Method:** Scraped the first 3 pages per subcategory over 3 weeks using Python (`requests`, `BeautifulSoup`) in incognito mode to reduce preference bias.  
- **Dataset:** Combined search results (product position) with product detail pages (attributes like price, reviews, brand) to create a unified dataset for modeling.

---

## ⚙️ Approach  
- **Feature Engineering:** Created rank-based, interaction, and log-transformed features to reduce skew and capture category-specific patterns.  
- **Modeling:** Tested linear regression, Lasso regression, and random forest classification to predict product order.  
- **Evaluation:** Used metrics such as R², MSE, RMSE, and F1 scores to assess model performance.

---

## 📊 Key Findings  
- **Low Predictability:** Visible features (ratings, reviews, stock, recent demand) showed weak correlation with ranking.  
- **Black Box Evidence:** Placement likely shaped by hidden factors—such as sponsored ads, fulfillment preferences (FBA/Prime), and engagement signals not visible to consumers.  
- **Transparency Concerns:** Especially in health-related categories, ranking systems may influence consumer choices without clear accountability.

---

## 🚀 Future Directions  
- Integrate richer data, such as sponsored status, keyword relevance, user engagement, or even **clinical efficacy** to improve model accuracy.  
- Explore Amazon’s seller and advertising ecosystem to understand how sellers influence visibility.  
- Develop interpretability tools (e.g., SHAP) and fairness audits to assess ranking systems.

---

## 💡 Impact  
### For Sellers  
Insights into which visible product attributes matter less for ranking, and how hidden factors might drive visibility. This can inform pricing, branding, and promotional strategies to compete more effectively.

### For Consumers  
Increased awareness of how rankings shape choices, helping them make more informed decisions—especially important for health-related products where trust and efficacy are critical.

## ⚠️ Disclaimer  
This project is for **educational and research purposes only**. It does not reveal Amazon’s proprietary algorithms but rather explores publicly available data to understand patterns in product visibility.

