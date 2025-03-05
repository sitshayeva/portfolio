
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Data Projects Portfolio</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f9fa;
            margin: 0;
            padding: 20px;
        }
        .header {
            background-color: #FFC107;
            padding: 20px;
            text-align: center;
            color: #FFF;
            font-size: 24px;
            font-weight: bold;
        }
        .container {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            max-width: 1200px;
            margin: 20px auto;
        }
        .project {
            background: white;
            padding: 15px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        .project img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px;
        }
        .project h3 {
            font-size: 18px;
            margin: 10px 0;
        }
        .project p {
            font-size: 14px;
            color: #666;
        }
        .project a {
            display: inline-block;
            margin-top: 10px;
            text-decoration: none;
            color: #007bff;
            font-weight: bold;
        }
        @media (max-width: 992px) {
            .container {
                grid-template-columns: repeat(2, 1fr);
            }
        }
        @media (max-width: 600px) {
            .container {
                grid-template-columns: repeat(1, 1fr);
            }
        }
    </style>
</head>
<body>
    <div class="header">DATA PROJECTS</div>
    <div class="container">
        
        <script>
            const projects = [
                { title: "Indicators of Heavy Traffic on I-94", image: "53" },
                { title: "EUR Exchange Rate Trends & Volatility Analysis (1999-2021)", image: "54" },
                { title: "London Weather Forecasting with Prophet, Requests (Open-Meteo API)", image: "55" },
                { title: "UK Online Retail Data Quality Validation Project (GX)", image: "51" },
                { title: "Toy Store KPI Report", image: "47" },
                { title: "Global CO2 Emissions Interactive Dashboard", image: "52" },
                { title: "LEGO Set Explorer", image: "48" },
                { title: "Coffee Shop Dashboard", image: "49" },
                { title: "Global CO2 Emissions", image: "50" },
                { title: "AirBnB Listing Analysis", image: "44" },
                { title: "Restaurant Order Analysis", image: "45" },
                { title: "CRM Sales Dashboard", image: "46" },
                { title: "Market Basket Analysis", image: "43" },
                { title: "PySpark Diabetes Prediction ML Project", image: "42" },
                { title: "iTunes Podcast Reviews Dashboards Tableau", image: "41" },
                { title: "Customer K-means clustering in Python", image: "30" },
                { title: "Machine Learning: Decision Tree with KNIME", image: "31_1" },
                { title: "Machine Learning: Decision Tree with KNIME", image: "31_2" },
                { title: "NLP Challenge: IMDB Dataset of 50K Movie Reviews to perform Sentiment Analysis", image: "32" },
                { title: "Recommendation System. Collaborative Filtering", image: "35" },
                { title: "Book Recommendation Model. K-Nearest Neighbors", image: "37" },
                { title: "Amazon Customer Reviews Sentiment Analysis", image: "33" },
                { title: "Image Classifier using TensorFlow. Keras", image: "36" },
                { title: "Linear Regression Health Costs Calculator", image: "38" },
                { title: "Neural Network SMS Text Classifier", image: "39" },
                { title: "Sentiment Analysis of Yelp Business Reviews", image: "15" },
                { title: "Using Streamlit for Data Visualisation", image: "18_1" },
                { title: "Using Streamlit for Data Visualisation", image: "18_2" },
                { title: "WEB scraping and Sentiment Analysis British Airways Customer Reviews", image: "24_1" },
                { title: "WEB scraping and Sentiment Analysis British Airways Customer Reviews", image: "24_2" },
                { title: "Creating Dynamic Filters in Streamlit", image: "19_1" },
                { title: "Creating Dynamic Filters in Streamlit", image: "19_2" },
                { title: "Predicting Customer Behaviour British Airways", image: "25_1" },
                { title: "Predicting Customer Behaviour British Airways", image: "25_2" },
                { title: "Kaggle Housing Prices Competition", image: "28" },
                { title: "Kaggle Store Sales - Time Series Forecasting", image: "34" }
            ];
            
            projects.forEach(proj => {
                document.write(`
                    <div class="project">
                        <img src="images/${proj.image}.png" alt="Project Image">
                        <h3>${proj.title}</h3>
                    </div>
                `);
            });
        </script>
        
    </div>
</body>
</html>

































