# My First Project in ML 
# California House Price Predictor in ML 🏡🤖

Welcome to my machine learning journey! This project is a living diary of me building a real estate AI, following the systematic, data-first approach taught by Aurélien Géron in *Hands-On Machine Learning*. 

Rather than just throwing a fancy algorithm at a dataset on day one, I wanted to document the actual process of exploring, cleaning, and engineering data to see how much it improves the AI's understanding.

Here is the story of how this project has evolved so far:

## 🗓️ Project Timeline & Dev Journal

### April 11, 2026: Day One - The Setup 
* **Commits:** *"Official first commit", "Added data exploration and checked stats", "fixed"*
* **What happened:** Got the project off the ground. Downloaded the 1990 California census data and spent the day just looking at the shape of it. Plotted some basic histograms, checked for missing data, and got a feel for what I was working with. Also had the classic developer moment of immediately needing a "fixed" commit right after starting!

### April 13, 2026: The Baseline AI
* **Commit:** *"Trained Linear Regression model. Achieved ~60% R-squared score"*
* **What happened:** Time to see what a basic AI could do without any help. I split the data into a training set and a test set (so it couldn't cheat by memorizing), and fed it to a standard Linear Regression model. It scored about 60%. Not terrible for a blind guess, but a straight line struggles to map complex things like geography. I knew I had to clean the data to get a better score.

### April 27, 2026: Housekeeping
* **Commit:** *"Update project title to include 'in ML'"*
* **What happened:** Just some minor repo cleanup to make the project intent clearer. 

### April 30, 2026: The Data  Improvements 🚀
* **Commits:** *"Update: Removed capped prices, added Bedrms_per_Room feature"*
* **What happened:** This was the big breakthrough day. I stopped focusing on the algorithm and started fixing the data itself:
  1. **Removed Artificial Caps:** Discovered the original dataset arbitrarily capped expensive houses at $500,000. I sliced those out so the AI wouldn't learn a fake "ceiling" for the housing market.
  2. **Feature Engineering:** The AI was struggling to understand the difference between a cramped 5-room apartment and a spacious 5-room luxury home. I engineered a new ratio (`Bedrms_per_Room`) to serve as a "Luxury Space Indicator." 
  3. **Scaling:** Prepped the data with `StandardScaler` so massive numbers (like Population) wouldn't overshadow smaller numbers (like Income).

