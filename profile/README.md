## Support Flow

### An extensible LLM-powered customer support chatbot with a no-friction AI-to-Human handoff.
### Won 1st Place in the Overall Beginner Track in the 2023 AI ATL Hackathon

> Team Members: Saketh Reddy, Colin Fluek, Cullen Steber, Anisha Ali
> Devpost: https://devpost.com/software/supportflow

### Project Components:

- support-flow-chat-ui: Streamlit chatbot application. Leverages OpenAI's function calling to: determine it's capabilities, intelligently prompt customers for necescary information, and transfer the conversation to a human representative when it is given a task it knows it cannot fulfil.

- supportflow-agent: React application that monitors our Firestore database for updates and sends agents to an agent dashboard when a new chatbot escalation is created. Agent dashboard includes customer information, the full chat history, the customer pain point the chatbot was unable to resolve, and instructions on what the agent needs to do in order to resolve the customers' issues.

- supportflow-agent-ui: Flask application for rendering static templated agent dashboards based off of URL parameters. 
