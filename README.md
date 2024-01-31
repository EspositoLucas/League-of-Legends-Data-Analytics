# League of Legends Data Analytics

### Overview
Analyzing the League of Legends API, this project explores player and match data to uncover trends and provide insights for a fictional stakeholder. Despite not playing the game, the inspiration came from watching the renowned player *Faker*, leading to the creation of a comprehensive data analytics portfolio.

All documentation can be found here: https://developer.riotgames.com/apis

### Technologies Used
- **Docker**: Set up a PostgreSQL database to efficiently manage and store data.
- **SQL**: Utilized for querying and extracting valuable information from the database.
- **Python**: Leveraged the power of pandas and plotly libraries for in-depth data analysis and visualization.

### Project Structure
- **Data Collection**: Gathered information from the League of Legends API to create a robust dataset.
- **Database Setup**: Employed Docker to establish a PostgreSQL database for seamless data storage and retrieval.
  - **Instructions for Setting Up PostgreSQL with Docker**:
    ```bash
    docker run \
    --name pg \
    -e POSTGRES_USER=postgres \
    -e POSTGRES_PASSWORD=test1234 \
    -e POSTGRES_DB=postgres \
    -v ${PWD}/postgres-docker:/var/lib/postgresql/data \
    -p 5432:5432 postgres
    ```
- **Notebooks**: Contains three Jupyter notebooks for different stages of the project:
  - **research.ipynb**: Initial research and exploration of the League of Legends API data.
  - **data_modeling.ipynb**: Implementation of data modeling techniques and feature engineering.
  - **business_intelligence.ipynb**: Application of business intelligence methodologies for actionable insights.

### Key Findings
- Identified player performance trends.
- Uncovered patterns in match outcomes.
- Developed actionable insights for a hypothetical stakeholder.

### Instructions for Replication
1. Clone the repository to your local machine.
2. Set up a Docker container with PostgreSQL using the provided configuration files.
3. Run the Jupyter notebooks in the [notebooks](notebooks/) folder in the specified order for a step-by-step walkthrough of the project.

### Visualization Highlights
- **Player Performance Trends**: Interactive charts showcasing key metrics.
- **Match Outcome Analysis**: Visual representation of match outcomes and influencing factors.

### Future Improvements
- Explore additional data sources for a more comprehensive analysis.
- Implement machine learning models for predictive insights.

