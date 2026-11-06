**Bring the workflow, not just the API specification**

_From API Workflows to Tests with_ **_ReadyAPI MCP_** _server_

An OpenAPI definition tells you what an API can do. It doesn’t tell you what anyone is meant to do with it.

I’ve been looking at how far you can get by starting from the second question. I used two OpenAPI files, one for authentication and one for banking, plus an Arazzo file that describes six journeys across both. I then used the ReadyAPI MCP server to turn those journeys into test cases.


**Prompt**

    Create a new ReadyAPI project named Arazzo-API-WorkFlow and create individual test cases that test the BearerAuthenticationAPI and banking-management-api separately  
    
    Once complete, use the banking-workflows.arazzo-2.0.0 arazzo workflow file to create a ReadyAPI Test Case for each of the workflows described in the file.  
    Ensure that propertys from responses are correctly passed to subsequent test steps.  
    
    For example, the login test step should receive an access token that should be passes as a header in banking api test steps
