# Machine-Fault-Diagnosis-AI-Agent
The Machine Fault Diagnosis AI Agent is a smart assistant that analyzes sensor data and symptoms to diagnose mechanical faults. It delivers expert maintenance recommendations and critical safety precautions to minimize downtime and ensure workplace safety.

## Features :
- Conversational Interface: Interact with the agent using natural language questions.

- Sensor Data Analysis: Processes simulated temperature, vibration, and noise data.

- Diagnostic Reasoning: Identifies potential faults and explains the "why" behind the diagnosis.

- Maintenance Recommendations: Suggests specific, safe repair and maintenance steps.

- Safety Precautions: Provides automated safety warnings relevant to the diagnosed issue.

- Multilingual Support: Potential for future expansion to support multiple languages.

## Quick Start & Commands
This is a conceptual guide to illustrate how a user would interact with the deployed agent.

- Prerequisites: An IBM Cloud account and the project's codebase.

- Deployment: Deploy the Agentic AI core and associated Cloud Functions on IBM Cloud.

Command Examples:

- Query: What is the temperature of the hydraulic pump right now?

- Query: My CNC machine is making a grinding noise. What could be the problem?

- Query: The motor on the lathe is vibrating excessively. What should I do?

- Query: Tell me the safety procedures for checking the gearbox on a mill.

## How It Works

- User Input: A technician submits a query to the agent's interface.

- Agentic Reasoning: The agent, powered by the IBM Granite model, analyzes the query. It recognizes the need for external information to provide a good answer.

- Tool Call: The agent decides to call a specific "tool" (e.g., a function to get_vibration_data or query_knowledge_base). This tool is hosted on IBM Cloud Functions.

- Data Retrieval: The Cloud Function executes, simulates retrieving real-time data or knowledge base content, and returns the information to the agent.

- Synthesize and Respond: The Granite model takes the original query and the retrieved information and synthesizes a comprehensive response. It might say, "The CNC machine is vibrating due to a bearing failure. Based on the temperature data, the issue is critical. You should safely shut down the machine and replace the bearing."

## Features :

- Conversational Interface: Interact with the agent using natural language questions.

- Sensor Data Analysis: Processes simulated temperature, vibration, and noise data.

- Diagnostic Reasoning: Identifies potential faults and explains the "why" behind the diagnosis.

- Maintenance Recommendations: Suggests specific, safe repair and maintenance steps.

- Safety Precautions: Provides automated safety warnings relevant to the diagnosed issue.

- Multilingual Support: Potential for future expansion to support multiple languages.


## Example
User: "My CNC machine is vibrating excessively. What's the problem and what should I do?"

Agent's Thought Process (Conceptual):

- CNC Machining | Y-axis vibration | Practical Machinist - Largest ... - A forum discussion on Y-axis vibration in CNC machines, which could be caused by tacho feedback.

- CNC Machining Defects and Failures: Causes & Solutions - An article discussing various defects and failures in CNC machining, including excessive vibration.

- Tips on How to Reduce Vibration in CNC Machining - Tips on reducing vibration in CNC machining, including balancing spindle speeds.

- What is Causing My Spindle to Vibrate? - PDS - An article discussing the causes of spindle vibration in CNC machines.

- CNC Machine Vibration - Problem Overview | Sacher sp z o.o. - An overview of CNC machine vibration problems and their causes.

- Indicators of a Bad Spindle on a CNC Machine | Expert Guide - An expert guide on the indicators of a bad spindle on a CNC machine, including excessive vibration.


## Applications

- The core technology can be adapted for a wide range of applications:

- Manufacturing: Diagnosing faults in assembly line robots, conveyor systems, and industrial presses.

- HVAC Systems: Identifying issues with pumps, fans, and compressors in commercial buildings.

- Automotive: Assisting mechanics in diagnosing engine or suspension problems based on telemetry.

- Oil & Gas: Monitoring and diagnosing faults in pumps, valves, and pipelines.

## Deployment :

- The project can be deployed entirely on IBM Cloud's free Lite tier. The agent's core logic (e.g., a Python script using the Granite API) can run as a simple service, while the "tools" are deployed as IBM Cloud Functions. The knowledge base is hosted on IBM Cloud Object Storage. This setup allows for easy scaling and zero cost for development and demonstration.

## Acknowledgements :

- IBM Cloud: For providing a robust and accessible free-tier platform for developers and students.

- IBM Granite: For developing the powerful and versatile Granite AI model.

## A Big Thank you Aswini Kumar Motapothula sir, and Edunet Foundation Team For invaluable guidance and support throughout the project.


























