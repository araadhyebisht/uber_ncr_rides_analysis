🚖 Uber NCR Ride Bookings Analysis (2024)

What is this?

This is an exploratory data analysis (EDA) project looking at a dataset of 150,000 Uber ride bookings in the Delhi National Capital Region (NCR) for the entire year of 2024. Digging into the unit economics, figuring out where the funnel is leaking (cancellations), and mapping out the actual geospatial demand across the city.
Total Gross Booking Value (GBV) in the dataset: ₹5.18 Crore (~₹51.8M)

Tools Used:
• Python (Pandas for heavy lifting) 

• Seaborn & Matplotlib for visualizations 

• A bit of manual mapping (using Google/Gemini) to group 100+ raw neighborhood names into 8 actual NCR zones (South Delhi, Noida, Gurgaon New City, etc.) for the route analysis to make sense

📊 The Real Business Insights

• We have an "Auto" supply problem: Auto rickshaws are the most popular vehicle choice for completed rides (nearly 25%). But they also have the highest rate of "No Driver Found" errors (over 25% of that category). The demand is there, but the fleet supply isn't keeping up.

• Premium rides are leaking: Go Sedan yields the highest average booking value per km (~₹34.6) , but a massive 38.5% of Go Sedan requests are never completed  (mostly due to drivers cancelling).

• UPI is is the most preferred payment option : 45% of all completed rides are paid via UPI. Cash is second (24.8%). Uber Wallet is barely used (12%), which means there's a missed opportunity to lock in user cash and reduce transaction fees.

• The Money Routes: The highest traffic volume is on the "South Delhi ↔ Gurgaon Old City & Industrial" corridor. But the best yield per kilometer rides was given by  the "Noida & Greater Noida" to "Gurgaon New City" route with ₹47.43/km.

🕵️‍♂️ About Data Integrity

It was found out that the dataset contains heavily synthetic/mocked data.
