# Real Estate Recommender System

## Project Summary

This project demonstrates the development of a personalized real estate recommender system using a Large Language Model (LLM). The system integrates various AI technologies to generate, store, and search real estate listings based on user preferences. The project is structured into several key tasks:

### Generating Real Estate Listings with an LLM

**Objective**  
Generate a minimum of 10 diverse and realistic real estate listings containing factual information using a Large Language Model.

**Methodology**  
- **Synthetic Database Creation:**  
  - Employed a Large Language Model to generate 10 diverse and realistic real estate listings.
  - Each listing encompasses details such as neighborhood, price, number of bedrooms, number of bathrooms, house size, and descriptions of the house and neighborhood.
 
- **Integration of Real Dataset:**  
  - Incorporated a real dataset titled \"House Price Estimation from Visual and Textual Features\" by H. Ahmed E. and Moustafa M. (2016).
  - Randomly assigned 4 images to each listing from this dataset to develop a multimodal recommender system.

### Creating a Vector Database and Storing Listings

**Objective**  
Create a vector database and store real estate listing embeddings generated from the LLM-created listings.

**Methodology**  
- **Vector Database Creation:**  
  - Established a vector database to store embeddings of the listings.
  - Utilized embedding techniques to convert textual and visual features of listings into embeddings.
 
- **Storage and Organization:**  
  - Successfully stored and organized the embeddings within the vector database for efficient retrieval.

### Semantic Search of Listings Based on Buyer Preferences

**Objective**  
Implement functionality that enables semantic search of listings based on buyer preferences.

**Methodology**  
- **Buyer Preferences Collection:**  
  - Collected buyer preferences to tailor the search functionality.
 
- **Semantic Search Implementation:**  
  - Developed semantic search algorithms to match buyer preferences with the stored listings.
  - The search functionality returns listings that closely align with the input preferences.

### Augmented Response Generation

**Objective**  
Enhance real estate listings based on buyer preferences by implementing logic for searching and augmenting listing descriptions.

**Methodology**  
- **Search and Augment Descriptions:**  
  - Formulated a logical flow where buyer preferences are used to search and augment real estate listings.
  - Ensured augmentations personalize the listings without altering factual information.
 
- **Use of LLM:**  
  - Leveraged the LLM to generate personalized descriptions for real estate listings based on buyer preferences.
  - The descriptions were ensured to be unique, appealing, and tailored to the provided preferences.

### Web UI for Demonstration

**Objective**  
Create a web-based user interface to demonstrate the basic functionality of the recommender system.

**Methodology**  
- **Web UI Development:**  
  - Developed a web UI using Gradio to showcase the system's functionalities.
  - Included features for inputting buyer preferences, viewing personalized listings, and searching through the database.

## Conclusion

Integrating URLs within the prompt template fed into the Large Language Model (LLM) significantly enhances the robustness and reliability of the real estate recommender system. This approach ensures that augmented descriptions are accurately matched with corresponding property images, addressing challenges previously encountered with separate image retrieval processes. By embedding URLs directly within the prompt, the system simplifies the workflow, aligns descriptions with images effectively, and reduces the potential for mismatches.

However, this method also increases token usage, which impacts the overall cost, especially during production and scaling. It is crucial to optimize prompt templates and employ cost-effective strategies to manage token consumption efficiently. The benefits of this robust solution can be fully realized by balancing the need for detailed, accurate outputs with cost management considerations.

### The Importance of Agents in AI Applications

In the realm of AI applications, agents play a pivotal role in automating tasks and enhancing business processes. An agent is a software program endowed with a degree of autonomy, capable of performing tasks, making decisions, and interacting with other systems or users without continuous human intervention. Agents possess several key characteristics:

- **Autonomy:** They operate independently, managing tasks without requiring constant user input.
- **Proactivity:** They can anticipate needs and take initiative, performing actions to achieve specific goals.
- **Reactivity:** They respond to changes in their environment or user inputs in real-time.
- **Social Interaction:** They can communicate and collaborate with other agents or systems to complete tasks.
- **Planning:** They can devise strategies to achieve objectives, optimizing their actions over time.

LLMs can be used to create such agents, mimicking human tasks and decision-making processes. These agents can interact with both proprietary and external data sources, providing a comprehensive solution for various business needs.

### Interaction with the Agent in Gradio

The developed web UI using Gradio allows users to interact with the real estate recommender agent seamlessly. Users can input their home preferences, and the agent will provide personalized property recommendations along with corresponding images. This interaction demonstrates the practical application of AI agents in enhancing user experience and automating complex tasks in real estate.

## Setup Instructions

1. **Clone the Repository**:
   \`\`\`bash
   git clone https://github.com/aciuffolini/Real-Estate-Agent.git
   cd Real-Estate-Agent
   \`\`\`

2. **Create a Virtual Environment and Activate It**:
   \`\`\`bash
   python -m venv venv
   source venv/bin/activate  # On Windows use \`venv\Scripts\activate\`
   \`\`\`

3. **Install the Required Packages**:
   \`\`\`bash
   pip install -r requirements.txt
   \`\`\`

4. **Run Jupyter Notebook**:
   \`\`\`bash
   jupyter notebook
   \`\`\`

## License

This project is licensed under the MIT License - see the LICENSE file for details." > README.md
