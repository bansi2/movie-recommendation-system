🎬🚀 Movie Recommendation System | NLP + Machine Learning + Streamlit

Hello LinkedIn network!
I'm excited to share one of my recent hands-on projects — a Movie Recommendation System that combines Natural Language Processing (NLP), vectorization techniques, and an interactive Streamlit web app to suggest movies based on content similarity.

🧠 Main Idea:
The system recommends movies by analyzing and comparing their content-based metadata, such as:

Overview (plot summary)

Genres

Keywords

Top 3 Cast members

Director

All this information is combined into a single 'tag' field and then transformed using text vectorization techniques to compute similarity between movies.

🔍 Step-by-Step Approach:
1. Data Preprocessing

Merged the TMDB movies and credits datasets on the title field.

Selected relevant columns: overview, genres, keywords, cast, and crew.

Cleaned and converted stringified JSON using Python's ast module.

Extracted top 3 cast members and the director from each movie.

Removed unnecessary spaces and transformed all textual data to lowercase.

2. Tag Creation

Combined all meaningful textual data into a single list and joined them to form a "tags" column.

Applied stemming using nltk.PorterStemmer to normalize the words.

3. Feature Extraction

Used CountVectorizer to convert text into numerical vectors (Bag of Words model with 5000 most frequent terms, excluding stopwords).

Calculated cosine similarity to measure how close movies are to each other in vector space.

4. Recommendation Function

For any selected movie, the function retrieves the top 5 most similar movies based on cosine similarity.

Stored the processed data and similarity matrix using pickle for fast loading in the web app.

🌐 Streamlit Web App
Built an intuitive and responsive Streamlit front-end, where:

Users can select a movie from a dropdown.

The app returns 5 recommended movies along with their posters (fetched using TMDb API).

🔧 Tools & Libraries Used:
Python

Pandas, NumPy

NLTK, AST, Scikit-learn

Streamlit

TMDb API

Pickle

✅ Key Takeaways:
Improved my skills in text preprocessing, vector space modeling, and web deployment.

Learned how to structure a real-world ML pipeline from raw data → model → deployment.

Demonstrated how to build an end-to-end ML-powered application that provides real value to users.

💬 I'd love to hear your feedback or suggestions!
🔗 DM me if you want to collaborate or need help building your own ML app.
📢 Open to internships, collaborations, and full-time opportunities in Data Science / ML / AI.

#MachineLearning #NLP #Python #Streamlit #DataScience #RecommendationSystem #MovieRecommendation #AI #PortfolioProject #MLProject #OpenToWork


![result1](https://github.com/user-attachments/assets/010e8c20-ac07-4598-9c6d-86aaf1ea5806)


