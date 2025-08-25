# IBM-CLOUD-Eco-Lifestyle-Agent

# 🌱 Eco Lifestyle Agent  

An **AI-powered assistant** that helps users live more sustainably by providing personalized, practical tips on eco-friendly habits, products, recycling methods, and government schemes. Using **Retrieval-Augmented Generation (RAG)** with **IBM Cloud Lite Services** and **IBM Granite**, the agent retrieves and delivers trusted information in natural language to promote greener daily decisions.  

This repository contains the **AI Service Deployment Notebook** to set up, test, and deploy the Eco Lifestyle Agent on **IBM watsonx.ai**.  

***

## 🚀 Features  
- Provides **sustainable living tips** tailored to user queries.  
- Retrieves eco-friendly product recommendations and recycling guidelines.  
- Suggests green travel options and local government schemes.  
- Powered by **IBM Granite models** and deployed via **watsonx.ai AI Service**.  
- Uses **RAG (Retrieval-Augmented Generation)** with search + curated environmental knowledge.  

***

## ⚙️ Technologies Used  
- **IBM watsonx.ai**  
- **IBM Cloud Lite Services**  
- **IBM Granite Foundation Models**  
- **LangChain + LangGraph**  
- **Python 3.11**  

***

## 📒 Notebook Structure  

The included Jupyter notebook contains the following steps:

1. **Setup**  
   - Connect to **watsonx API** using IBM Cloud Personal API Key.  
   - Set up project and space IDs.  

2. **Define the AI Service Function**  
   - Build chat service (`gen_ai_service`) using **ChatWatsonx** and tools (GoogleSearch, DuckDuckGo, Wikipedia, WebCrawler).  
   - Add memory, instructions, and tool orchestration logic.  

3. **Test Locally**  
   - Test prompts locally before deployment to ensure functionality.  

4. **Deploy the AI Service**  
   - Store AI service in **watsonx.ai repository**.  
   - Deploy with metadata for online usage.  

5. **Test Deployment**  
   - Query the deployed agent with natural language questions.  
   - Verify responses for correctness and eco-awareness.  

***

## ▶️ Quick Start  

### Prerequisites  
- Python **3.11**  
- IBM Cloud account with access to **watsonx.ai**  
- IBM Cloud **API Key**  

### Run the Notebook  

1. Clone this repository:  
   ```bash
   git clone https://github.com/your-username/eco-lifestyle-agent.git
   cd eco-lifestyle-agent
   ```

2. Launch Jupyter Notebook or JupyterLab:  
   ```bash
   jupyter notebook
   ```
3. Open `Eco_Lifestyle_Agent.ipynb` notebook.  

4. Enter your **IBM Cloud API Key** when prompted during setup.  

5. Run all cells to deploy the AI Service.  

***

## 🌍 Example Queries  
You can ask the Eco Lifestyle Agent:  
- *"How can I reduce plastic use at home?"*  
- *"What are eco-friendly travel options in my city?"*  
- *"Which government schemes support renewable energy adoption?"*  

***

## 📡 Deployment as REST API  

Once deployed, the agent is available as a **REST API** via your IBM Cloud deployment. Example payload:  

```json
{
  "messages": [
    { "role": "user", "content": "Suggest eco-friendly alternatives to single-use plastics." }
  ]
}
```

The response will include assistant recommendations with actionable tips.  

***

## 📜 License  

Licensed Materials – Copyright © 2024 IBM.  
This notebook and its source code are released under the terms of the **ILAN License**.  

***

## 🤝 Contributing  

Contributions are welcome! Feel free to open issues or submit pull requests to improve the agent’s eco-knowledge and features.  

***

🌱 Let’s make sustainability simple and accessible — one query at a time!  
