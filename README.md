# DeepResearch

🔬 Just built a Deep Research AI Agent using n8n + Google Gemini + Tavily – a full-scale pipeline that takes a single topic input and outputs a well-structured, AI-generated, multi-chapter PDF research report.

🧠 This agent mimics the research work of a human assistant — planning, writing, refining, formatting, sourcing, and exporting — all automatically.

🧩 What the Workflow Does:

✅ Takes user topic + email from a form then I write AI vs Agentic AI as I/p
✅ Splits the topic into 5 detailed research chapters
✅ Each chapter uses AI Agents (Gemini Flash Lite) for content generation
✅ Adds real-time context using Tavily Research API
✅ Stores all content in Google Sheets for transparency
✅ Uses custom logic to merge, format, and clean outputs
✅ Builds a clean Table of Contents + References section
✅ Sends final content to a PDF generation API
✅ Returns a downloadable professional report

⚙️ STACK USED
 • 🧠 AI Model: Google Gemini Flash Lite (Chat)
 • 🌐 Research Source: Tavily API
 • 📤 PDF API: HTTP node integration
 • 📄 Storage: Google Sheets
 • ⚙️ Automation Platform: n8n.io

🔧 Nodes/Modules I Used:

✅ HTTP Node
For Tavily API + PDF Generation API calls
🧩 Split Out Node
Branching into 5 parallel chapters
🧠 AI Agent Node
AI content generation using Gemini
📄 Google Sheets Node
Storing chapter-wise & final outputs
🔁 Merge Node
Combining all chapters into one body
🧮 Aggregate Node
Handling arrays and content joins
🔧 Set Node
Assigning and formatting data
🔀 Switch Node
Logic-based routing
💻 Code Node
Custom JavaScript logic for formatting
🌐 HTML Node
Rendering structured report content
 📈 Highlights:
 • Built on n8n with zero backend code
 • Modular and scalable – new chapters or logic can be added easily
 • Can be adapted to any domain: legal reports, startup research, education, etc.
