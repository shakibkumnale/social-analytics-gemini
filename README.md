Here’s the complete merged description for your GitHub repository:

---

# **Social Media Performance Analysis**

### **Overview**  
This project is an analytics module that evaluates the performance of social media posts by calculating engagement rates and generating actionable insights.

### **Key Features**  
- Calculates engagement rates using the formula:  
  \[
  \text{Engagement Rate} = \left(\frac{\text{Likes} + \text{Comments} + \text{Shares}}{\text{Reach}}\right) \times 100
  \]
- Provides insights comparing different post types (Reels, Carousel, Static).
- Utilizes **Gemini AI API (Google Generative AI)** for advanced generative insights.

### **Tech Stack**  
- **Database**: DataStax Astra DB for storing and querying engagement data.  
- **API**: Gemini AI API for generating insights.  
- **Workflow**: Langflow for streamlined integration and analytics.  

### **Why Gemini AI API?**  
Due to unavailability of an OpenAI API key, the Gemini AI API was used as an alternative, offering similar functionality for the assignment's requirements.  

### **How It Works**  
1. Fetches engagement data from Astra DB.  
2. Calculates engagement metrics and rates for each post type.  
3. Uses Gemini AI API to generate actionable insights.

---

### **Installation and Run**

Follow these steps to set up and run the project locally:

---

#### **1. Clone the Repository**
```bash
git clone https://github.com/your-username/social-media-performance.git
cd social-media-performance
```

---

#### **2. Install Dependencies**
- Ensure you have **Python 3.8+** installed on your system.
- Create and activate a virtual environment:
  ```bash
  python -m venv venv
  source venv/bin/activate  # On Windows: venv\Scripts\activate
  ```
- Install the required packages:
  ```bash
  pip install -r requirements.txt
  ```

---

#### **3. Configure Environment Variables**
- Create a `.env` file in the root directory:
  ```bash
  touch .env
  ```
- Add the following variables to the `.env` file:
  ```
  GEMINI_API_KEY=your_gemini_api_key
  ASTRA_DB_CLIENT_ID=your_astra_client_id
  ASTRA_DB_CLIENT_SECRET=your_astra_client_secret
  ASTRA_DB_KEYSPACE=your_keyspace_name
  ASTRA_DB_HOST=your_database_host
  ```

---

#### **4. Set Up Astra DB**
- Use the [DataStax Astra DB dashboard](https://www.datastax.com/) to:
  - Create a database.
  - Add a table for storing engagement data (`social_engagement`).
- Import the sample data provided in the `sample_data.json` file:
  ```bash
  python scripts/import_data.py
  ```

---

#### **5. Run the Project**
- Launch the project:
  ```bash
  python main.py
  ```
- Open the application in your browser (if applicable) or view console outputs.

---

#### **6. Testing**
To test functionality:
- Update the `tests/` folder with your API keys and sample data.
- Run the tests:
  ```bash
  pytest
  ```

---

Feel free to adjust the details as needed. Let me know if you need further customization!
