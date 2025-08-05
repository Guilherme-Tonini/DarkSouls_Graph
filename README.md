# DarkSouls Knowledge Graph

This project builds an interactive knowledge graph based on entities and relationships extracted from the *DarkSouls* game universe. It uses natural language processing (NLP) and graph analysis to reveal narrative structures, character relationships, lore connections, and more.

## Install Dependencies

pip install -r requirements.txt

## Project Structure


├── AI_usage.md               # Description of how AI tools supported the project
├── README.md                 # Project overview and setup instructions
├── Extract & Transformation.ipynb
├── Insights & QA.ipynb
├── dark_souls_graph.graphml # Full graph file for offline exploration
├── web_graph_info.txt        # Neo4j access info (URI, username, password)
├── dfdialogs.csv             # In-game dialogue lines
├── dfitens.csv               # Item names and descriptions
├── dfother.csv               # System messages, character names, and locations
├── entidades.csv             # All entities and their types
├── relacoes.csv              # Entity relationships
├── nodes.csv                 # Formatted node list for Neo4j import
├── edges.csv                 # Formatted edge list for Neo4j import

## Run Locally

Open *Extract & Transformation.ipynb* to explore how data was collected and processed. ⚠️ Running the code is not recommended, as the notebook is a bit messy. Use it mainly for reference or if you're curious about the data extraction and transformation steps.

Open *Insights & QA.ipynb* to see the insights generation and question-answering process. This notebook is much more organized and can be run smoothly if you'd like to reproduce the analysis.

If you prefer manual graph exploration, open the .graphml file using tools like Gephi or yEd.

## Web Graph (Neo4j Aura)

To access it:
Visit [Neo4j Aura Console](https://console.neo4j.io/)
Use the credentials provided in *web_graph_info.txt*

## Deploy to Your Own Neo4j Instance (Optional)

If you'd like to use your own Neo4j Aura instance:

1. Create a free AuraDB instance at [Neo4j Aura Console](https://console.neo4j.io/)
2. Open the *Import* section and upload:
   - `nodes.csv`
   - `edges.csv`
3. Use the provided import Cypher commands shown by the interface to create the graph.
4. Your knowledge graph will be ready to explore via the Neo4j browser.


## Workflow and Brainstorm

A visual workflow and ideation board was created using Figma to illustrate the project's structure, thought process, and decision-making path.

Please note: the content is in Portuguese (BR), as it reflects my native language.
This resource is a bonus and not a required part of the main project.

Figma Board: [Click Here](https://www.figma.com/board/WTGtokIuKeznweRgdtNB8A/DarkFlows-Project?node-id=0-1&p=f&t=IntPs3BzTGIMUjxE-0)

## Disclaimer

This is a fan-made, non-commercial academic project created for educational purposes only. All characters, names, locations, and related content are the intellectual property of FromSoftware and Bandai Namco Entertainment. This project is not affiliated with, endorsed by, or associated with the official creators of Dark Souls.

## Acknowledgements

This project was made possible thanks to the incredible Dark Souls community.
Special thanks to [leminerva.github](https://leminerva.github.io/Dark-Souls-Documents/) and all contributors to open-source tools like NetworkX and BeautifulSoup