

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

Got it! Here's the updated version of the instructions based on the new method to run the project:

---


#### **1. Clone the Repository**
```bash
git clone https://github.com/your-username/social-media-performance.git
cd social-media-performance
```

---

#### **2. Install Dependencies**
- Ensure you have **Python 3.8+** installed on your system.
- Install **Langflow** using pip:
  ```bash
  pip install langflow
  ```

---

#### **3. Create and Activate Virtual Environment**
- Create a virtual environment named `langflow_env`:
  ```bash
  python -m venv langflow_env
  ```
- Activate the virtual environment:
  ```bash
  langflow_env\Scripts\activate  # On Windows
  ```
  Or on macOS/Linux:
  ```bash
  source langflow_env/bin/activate
  ```

---

#### **4. Configure Environment Variables**


---

#### **5. Set Up Astra DB**
- Use the [DataStax Astra DB dashboard](https://www.datastax.com/) to:
  - Create a database.
  - Add a table for storing engagement data (`social_engagement`).
- Import the sample data provided in the `sample_data.json` file:
  ```bash
  python scripts/import_data.py
  ```

---

#### **6. Run the Project**
- Run the project using Langflow:
  ```bash
  uv run langflow run
  ```
- Open the application in your browser (if applicable) or view console outputs.

---

#### **7. Testing**
To test functionality:
- Update the `tests/` folder with your API keys and sample data.
- Run the tests:
  ```bash
  pytest
  ```

---

This should be aligned with your new setup. Let me know if any further changes are needed!
