## Week 5 - Graph Data

For week 5, we can no longer use Python as GraphX is not supported by PySpark. We need to shift to Scala. Luckily, we can do so from the Jupyter Notebook we have been using.

After logging onto your Vagrant box using ```Vagrant shh```, please enter the following command before launching your Jupyter notebook:

```jupyter toree install --spark_home=/usr/local/spark --user```

### Neo4j

Installation:

1. Go the Neo4j [Download](www.neo4j.com/download) page.
2. Download the community edition for your OS
3. Follow the instructions

Objective:

Create a graph database with 4 types of Nodes (attributes in parantheses):

1. Patient (Name, Age, Gender)
2. Doctor (Name)
3. Disease (Name, Stage)
4. Hospital (Name, City, State)

Write the Cypher queries for the following questions:

1. Populate the tables with data where there are at least 3 of each type, and create the relationships accordingly.
2. Update the stage for patient 3.
3. Who are the male patients who has been treated by Doctor "A" (choose your name accordingly) who had Stage 3 Cancer in San Francisco. You may use the names of your own choosing.


