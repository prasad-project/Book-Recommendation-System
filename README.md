📚 BookRecs - Book Recommendation System
A sophisticated book recommendation system built with Flask that uses collaborative filtering to suggest books based on user preferences. The application features a clean, modern interface showcasing popular books and personalized recommendations.

✨ Features

Popular Books Showcase: Displays top 50 highly-rated books with ratings and vote counts
Personalized Recommendations: Get 4 similar book suggestions based on your favorite book
Similarity-Based Algorithm: Uses collaborative filtering with cosine similarity
Responsive Design: Modern UI with smooth navigation
Rich Book Information: Displays book covers, authors, ratings, and number of votes

🎯 Demo
Home Page - Top 50 Books
The home page displays a curated collection of the most popular books with:

Book cover images
Author names
Average ratings (⭐)
Number of user votes
![alt text](<Screenshot 2025-11-09 191859.png>)

Recommendation Page
Enter a book title you love, and get 4 similar book recommendations instantly!
🚀 Tech Stack
Backend:

Python 3.x
Flask - Web framework
NumPy - Numerical computations
Pandas - Data manipulation (implied from pickle files)
Scikit-learn - Machine learning algorithms (for similarity scores)

Frontend:

HTML5
CSS3
Modern responsive design

Data Processing:

Pickle - Serialized model and data storage

📁 Project Structure
BookRecs/
│
├── app.py                      # Main Flask application
├── templates/
│   ├── index.html             # Home page template
│   └── recommend.html         # Recommendation page template
│
├── static/                     # Static assets (CSS, images)
│
├── models/                     # Pickled model files
│   ├── popular.pkl            # Popular books dataset
│   ├── pt.pkl                 # Pivot table for recommendations
│   ├── books.pkl              # Complete books dataset
│   └── similarity_scores.pkl  # Precomputed similarity matrix
│
└── README.md                   # Project documentation
🛠️ Installation
Prerequisites






Run the application

bashpython app.py

Access the application
Open your browser and navigate to:

http://127.0.0.1:5000/
💡 How It Works
Recommendation Algorithm

Data Preprocessing: Books data is processed into a pivot table where rows represent books and columns represent user ratings
Similarity Computation: Cosine similarity is calculated between books based on user rating patterns
Recommendation Generation: When a user inputs a book title:

The system finds the book in the pivot table
Retrieves its similarity scores with all other books
Returns the top 4 most similar books



🔮 Future Enhancements

 User authentication and profile management
 Personal library to save favorite books
 Advanced filtering (genre, author, year)
 Book reviews and ratings system
 REST API for mobile app integration
 Integration with Goodreads API for updated book data
 Machine learning model retraining pipeline
 Search functionality with autocomplete
 Dark/Light theme toggle

🤝 Contributing
Contributions are welcome! Here's how you can help:


🙏 Acknowledgments

Book data sourced from Book-Crossing Dataset
Flask framework documentation
Scikit-learn for machine learning tools

📧 Contact
For questions or feedback, please reach out:

Email: prasadpalei360email@gmail.com
