# Definition
* MCP = Model Context Protocol
* MCP is a protocol which enables LLM applications to interact with Tools / Resources ( Outside of LLM )
* MCP is a standardization for connecting AI assistants with Tools / Resources
* MCP is
  * Connector for API / DB
  * Adapter for API / DB
  * Tool Interface for AI Agent

```java
* API = for developers
* MCP = for AI agents
```java

# ToRead
* MCP acts as USB port for all device types to connect to PC

# MCP Architecture
* LLM(Chat GPT, Claude etc) interacts with MCP Client
* MCP Server(Drive server, Calender server, Weather server etc) interacts with Tools(Drive app/API, Calender app/API, Weather app/API etc)
* Each Tool should have its own MCP server
* Each MCP server has its own MCP client
* LLM should maintain MCP client and Tool provider should maintain MCP server 
* <img width="797" height="398" alt="image" src="https://github.com/user-attachments/assets/95891d3d-27b0-4c2f-8e77-6d688efaa3bf" />


# What MCP does ?
1. Send email
2. Execute query on Database
3. Get weather data

# LLM
1. ChatGPT
2. Claude

# Tools
1. Drive API / Drive App
2. Calender API / Calender App
3. Weather API / Weather App

# Flow
```java
LLM --> MCP(MCP Client, MCP Server) --> Tools

We are trying to provide **Context** of **Tools** to **Model**

**Protocol** is Standard
```

# Images
* <img width="1189" height="650" alt="image" src="https://github.com/user-attachments/assets/b6ead2d9-9916-4f8f-944e-46a109138325" />
* <img width="1584" height="828" alt="image" src="https://github.com/user-attachments/assets/43159e1e-e753-4c7f-a542-022bfdd1e8d4" />


