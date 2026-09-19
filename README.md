# LangGraph Learning Lab

A structured collection of hands-on projects, notebooks, implementations, and notes covering **LangChain, LangGraph, Agentic AI, RAG, MCP, memory, persistence, streaming, human-in-the-loop workflows, and LangSmith observability**.

This repository documents my learning and experimentation with building stateful, workflow-driven LLM applications using LangGraph and the surrounding LangChain ecosystem.

---

## 📚 Topics Covered

The repository progresses from fundamental concepts to more advanced LangGraph applications.

### 1. LangChain vs LangGraph

Introduction to the differences between LangChain and LangGraph, their abstractions, and when graph-based orchestration is useful for LLM applications.

**Topics:**
- LangChain fundamentals
- LangGraph fundamentals
- Chains vs graphs
- Stateful workflows
- Graph-based orchestration

---

### 2. LangGraph Core Concepts

Fundamental building blocks of LangGraph.

**Topics:**
- State
- Nodes
- Edges
- START and END
- StateGraph
- Graph compilation
- State updates
- Graph execution

---

### 3. Sequential Workflows

Building workflows where nodes execute sequentially.

**Examples:**
- BMI workflow
- Simple LLM workflow
- Prompt chaining

**Topics:**
- Sequential execution
- Node composition
- State passing
- Prompt chaining
- Multi-step LLM pipelines

---

### 4. Parallel Workflows

Executing multiple independent operations concurrently.

**Examples:**
- Batsman analysis workflow
- UPSC essay workflow

**Topics:**
- Parallel execution
- Fan-out / fan-in
- Independent node execution
- Combining parallel results

---

### 5. Conditional Workflows

Building workflows where execution depends on the current state or the output of previous nodes.

**Examples:**
- Quadratic equation workflow
- Review/reply workflow

**Topics:**
- Conditional edges
- Routing
- Dynamic execution paths
- State-based decisions

---

### 6. Iterative Workflows

Building workflows that repeatedly execute nodes until a condition is satisfied.

**Example:**
- X post generator

**Topics:**
- Cyclic graphs
- Iteration
- Conditional loops
- Evaluation and refinement
- Generator-evaluator patterns

---

### 7. Building a Chatbot with LangGraph

A basic stateful chatbot implemented using LangGraph.

**Topics:**
- Message state
- HumanMessage / AIMessage
- LLM integration
- Graph-based chatbot architecture
- Conversation state

---

### 8. Persistence in LangGraph

Understanding how LangGraph maintains state across executions.

**Topics:**
- Checkpoints
- Persistence
- Threads
- Thread IDs
- MemorySaver
- State recovery
- Fault tolerance
- Resuming interrupted workflows

---

### 9. Building a Chatbot UI with Streamlit

Connecting a LangGraph backend to a Streamlit frontend.

**Topics:**
- Streamlit chat interface
- `st.session_state`
- Chat input/output
- Backend/frontend separation
- Thread-based conversations
- Stateful UI

---

### 10. Streaming in LangGraph

Streaming intermediate and final LLM outputs to the user.

**Topics:**
- Streaming
- `stream()`
- Streaming modes
- Incremental responses
- LangGraph + Streamlit integration
- Real-time chatbot responses

---

### 11. Resume Chat Feature

Building a chatbot that can interact with resume information and maintain conversation context.

**Topics:**
- Resume-based conversations
- Document-aware chat
- Thread management
- Stateful interactions
- ChatGPT-style conversation flow

---

### 12. LangGraph + SQLite

Using SQLite as a persistent storage layer for LangGraph applications.

**Topics:**
- SQLite
- Database-backed persistence
- Checkpoint storage
- Persistent chatbot state
- LangGraph database integration

---

### 13. LangSmith

Introduction to LangSmith for developing and debugging LLM applications.

**Topics:**
- LangSmith
- Tracing
- Runs
- Debugging
- LLM application monitoring
- Prompt/application inspection

---

### 14. Observability in LangGraph

Applying observability concepts to LangGraph applications.

**Topics:**
- Tracing
- Execution monitoring
- Debugging workflows
- LangSmith integration
- Database-backed applications
- Observability for agentic systems

---

### 15. Tools and Agentic AI

Using tools inside LangGraph to build more capable agentic systems.

**Topics:**
- Tool calling
- Tool nodes
- Tool execution
- Agents
- Agentic workflows
- LLM decision-making
- External tool integration

---

### 16. MCP Client with LangGraph

Building Model Context Protocol (MCP) clients and integrating them with LangGraph.

**Topics:**
- MCP
- MCP clients
- MCP tools
- Async MCP communication
- Tool discovery
- LangGraph + MCP integration

---

### 17. RAG with LangGraph

Building Retrieval-Augmented Generation pipelines using LangGraph.

**Topics:**
- Document loading
- Text splitting
- Embeddings
- Vector stores
- Retrieval
- Context injection
- RAG pipelines
- LangGraph-based RAG orchestration

---

### 18. Human-in-the-Loop (HITL)

Adding human intervention to LangGraph workflows.

**Topics:**
- Human approval
- Interrupts
- Resume execution
- Human validation
- Controlled agentic workflows
- Human + AI collaboration

---

### 19. Subgraphs

Breaking complex LangGraph applications into smaller reusable graphs.

**Topics:**
- Subgraphs
- Shared state
- Nested graphs
- Modular workflows
- Graph composition
- Reusable workflow components

---

### 20. LLM Memory

Understanding how memory can be implemented around LLM applications.

**Topics:**
- Stateless LLMs
- Conversation history
- Context management
- Short-term memory
- Long-term memory

---

### 21. Short-Term Memory

Implementing short-term conversational memory using LangGraph.

**Topics:**
- Short-term memory
- Checkpointing
- Persistence
- Message trimming
- Message deletion
- Conversation summarization
- Context-window management

---

### 22. Long-Term Memory

Implementing persistent memory that can survive beyond an individual conversation thread.

**Topics:**
- Long-term memory
- Memory storage
- Semantic memory
- Persistent memory
- PostgreSQL
- Cross-session information
- User-specific memory

---

## 🏗️ Repository Structure

```text
langgraph-learning-lab/
│
├── 02+03_Generative AI vs Agentic AI/
│
├── 4_LangChain Vs LangGraph/
├── 5_LangGraph Core Concepts/
├── 6_Sequential Workflows in LangGraph/
├── 7_Parallel Workflows in LangGraph/
├── 8_Conditional Workflows in LangGraph/
├── 9_Iterative Workflows in LangGraph/
│
├── 10_How to build a Chatbot using LangGraph/
├── 11_Persistence in LangGraph/
├── 12_Building a Chatbot with UI in LangGraph & Streamlit/
├── 13_Streaming in LangGraph/
├── 14_How to build a Resume Chat feature like ChatGPT/
├── 15_LangGraph + SQLite Chatbot with Database Integration/
├── 16_LangSmith Crash Course/
├── 17_Observability in LangGraph/
├── 18_Tools in LangGraph Agentic AI using LangGraph/
├── 19_How to build MCP Client using LangGraph/
├── 20_RAG using LangGraph/
├── 21_Human in the loop (HITL) using LangGraph/
├── 22_How to build Subgraphs in LangGraph/
├── 23_LLMs Don't Have Memory — So How Do They Remember/
├── 24_How To Implement Short Term Memory Using LangGraph/
├── 25_Long Term Memory in LangGraph/
│
├── requirements.txt
└── .gitignore
