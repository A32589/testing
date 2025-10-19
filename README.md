# testing
Linking

I am learning R, this repository is for same.

- Don't give me high-level advice. Respond with actual code and avoid fluff.
- Be casual and treat me as an expert.
- No need to mention you're an AI.
- Give the answer immediately, then explain if needed.
- Prefer functional code over imperative where possible.
- Always use [your preferred style guide/framework conventions].
- No moral lectures—discuss safety only when crucial.

How to set up MCP in Cursor:​

Create/update ~/.cursor/mcp.json (global) or .cursor/mcp.json (project-specific)

Install MCP servers: pip install mcp-server-time or npx -y @mui/mcp@latest

Configure in your mcp.json:

json
{
  "mcpServers": {
    "mui-mcp": {
      "type": "stdio",
      "command": "npx",
      "args": ["-y", "@mui/mcp@latest"]
    }
  }
}
Invoke in Chat with queries like: "What are the latest MUI DataGrid props?"​

Browse available MCP servers at glama.ai/mcp/servers.​

Global Rules (apply across all projects):​

Click the book icon → Global

Example: "Use TypeScript, avoid semicolons, prefer British-English spelling"

Project Rules (.windsurf/rules directory):​

Tied to specific globs or natural language descriptions

Example: "When starting a new conversation, first read the README file"​

Can be shared with teams via version control

Discover community rules and MCPs at windsurf.run.​

When stuck:

Ask AI to add detailed logging/console.log statements

Run the code and collect output

Paste logs back to AI

Let it analyze actual vs. expected behavior

6. Ignoring Warning Signs of AI Drift​

Stop immediately if you see:

Same error being "fixed" multiple times

AI keeps apologizing and starting over

Solutions getting more complex instead of simpler

Different approaches suggested in each attempt

Fix: Hit stop, revert to last working state, start new conversation with clearer constraints.

1. Notepads for Repeatable Prompts​

Create reusable prompt templates in Cursor's Notepads feature for frequently used instructions or code patterns. Reference seamlessly in future prompts for consistency.

5. Documentation-Driven Development​

For Windsurf projects:

Create Mermaid diagrams to visualize component relationships​

Maintain comprehensive markdown docs covering core components, interactions, use cases

Save conversation summaries in a Chatlog folder​

Update agent memory with new insights via 'Additional Options'​

Implement checkpoint system: save working versions in Checkpoints folder with timestamps​


----- 

For PPT : 
→ LLMs are knowledge bases, not cognitive problem-solvers. You provide the intelligence through well-crafted prompts.
→ For complex integrations or features, start with questions to align with the LLM; creates a shared understanding and can produce a requirements document to reference throughout development
→ Break complex features into the smallest possible version
→  Context Management
→ Create a /docs folder in your project root with:
→ Project plans and feature requirements : Database schemas : Architecture decisions :Tutorials and examples
→ 
