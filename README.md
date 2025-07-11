# 🚀 N8N Workflows Repository - 2000+ Automation Templates

A comprehensive collection of **2000+ n8n workflow automation templates** with AI-focused blueprints, educational resources, and an interactive documentation system.

## 📍 Quick Navigation

- [🔍 Browse Workflows](#-how-to-find-workflows)
- [📁 Repository Structure](#-repository-structure)
- [⚡ Quick Start](#-quick-start)
- [🤖 AI Workflow Categories](#-ai-workflow-categories)
- [📊 Interactive Documentation](#-interactive-documentation)
- [🛠️ Installation](#️-installation)

## 🔍 How to Find Workflows

### Option 1: Interactive Documentation (Recommended)
1. Navigate to the `n8n` directory
2. Run `python3 generate_documentation.py`
3. Open `workflow-documentation.html` in your browser
4. Use the search and filter features to find workflows by:
   - **Integration** (e.g., OpenAI, Slack, Google Sheets)
   - **Trigger Type** (Manual, Webhook, Scheduled)
   - **Complexity** (Low, Medium, High)
   - **Keywords** in workflow names

### Option 2: Browse by Category
Navigate directly to category folders:
- **Production Workflows**: `n8n/workflows/` - 2000+ ready-to-use workflows
- **AI Templates**: `AI Workflow Blueprints(n8n)/` - Educational resources organized by use case

### Option 3: Search Repository
Use GitHub's search feature or your local file search for specific integrations or use cases.

## 📁 Repository Structure

```
workflows-n8n/
├── 📚 n8n/                                    # Main workflow collection
│   ├── workflows/                             # 2000+ production-ready workflow JSONs
│   ├── generate_documentation.py              # Interactive docs generator
│   ├── workflow-documentation.html            # Browse all workflows (generated)
│   ├── import-workflows.sh                    # Bulk import script
│   └── README.md                              # Detailed usage guide
│
├── 🤖 AI Workflow Blueprints(n8n)/           # AI-focused educational content
│   ├── AI Integration, Data Handling & Workflows/
│   ├── AI Tools for thinking, Research & Content/
│   ├── N8n Templates/                         # YouTube tutorial workflows
│   ├── n8naiagents/                         # AI agent examples
│   └── 🤖 AI Agents, Chatbots & Automation/
│
├── CLAUDE.md                                  # AI assistant context
└── README.md                                  # This file
```

## ⚡ Quick Start

### 1. Generate Interactive Documentation
```bash
cd n8n
python3 generate_documentation.py
# Open workflow-documentation.html in your browser
```

### 2. Import a Single Workflow
1. Open n8n Editor UI
2. Menu (☰) → Import workflow
3. Select any `.json` file from `n8n/workflows/`
4. Configure credentials and test

### 3. Bulk Import All Workflows
```bash
cd n8n
./import-workflows.sh
```

## 🤖 AI Workflow Categories

### AI Integration & Data Handling
Located in `AI Workflow Blueprints(n8n)/AI Integration, Data Handling & Workflows/`:
- **Web Scraping**: AI-powered data extraction with Jina, Apify
- **Document Processing**: PDF extraction, invoice processing with LlamaParse
- **Email Automation**: Gmail labeling, auto-responders with AI
- **Data Enrichment**: Lead qualification, customer insights with AI
- **API Integrations**: OpenAI, Claude, Gemini, Mistral implementations

### AI Tools for Research & Content
Located in `AI Workflow Blueprints(n8n)/AI Tools for thinking, Research & Content/`:
- **Content Creation**: Blog automation, SEO optimization
- **Research Tools**: Web research, competitor analysis with Exa.ai
- **Voice Applications**: AI voice chat with ElevenLabs
- **Knowledge Management**: RAG implementations, vector databases

### AI Agents & Chatbots
Located in `AI Workflow Blueprints(n8n)/🤖 AI Agents, Chatbots & Automation/`:
- **Customer Support**: Multi-channel support bots
- **Slack/Discord Bots**: Team automation assistants
- **WhatsApp Integration**: Business automation
- **Memory Systems**: Conversation persistence

## 📊 Interactive Documentation

The documentation system provides:
- **Search & Filter**: Find workflows by integration, trigger, or complexity
- **Visual Stats**: Workflow distribution charts and metrics
- **Workflow Details**: Descriptions, node counts, integrations used
- **JSON Viewer**: Examine and copy workflow configurations
- **Dark/Light Mode**: Comfortable viewing experience

### Key Features
- **2053+ Workflows** indexed and searchable
- **100+ Integrations** detected automatically
- **Complexity Analysis** based on node count
- **Auto-generated Descriptions** for each workflow

## 🛠️ Installation

### Prerequisites
- n8n instance (self-hosted or cloud)
- Python 3.6+ (for documentation generator)
- Basic command line knowledge

### Workflow Import Tips
1. **Update Credentials**: Replace placeholder tokens with your API keys
2. **Test First**: Run workflows in test mode before production
3. **Check Webhooks**: Update webhook URLs to match your domain
4. **Version Compatibility**: Ensure n8n version matches workflow requirements

## 🔐 Security Notes

All workflows have been sanitized with API tokens replaced by placeholders:
- `YOUR_OPENAI_API_KEY_HERE`
- `YOUR_APIFY_API_TOKEN_HERE`
- `YOUR_GOOGLE_API_KEY_HERE`
- etc.

Always review workflows before running them in production.

## 📈 Repository Stats

- **Total Workflows**: 2053+
- **AI-Focused Workflows**: 500+
- **Integrations**: 100+ platforms
- **Categories**: 15+ use cases
- **Complexity Range**: 2-50+ nodes

## 🤝 Contributing

Contributions welcome! Please:
1. Test workflows before submitting
2. Remove all sensitive data
3. Use descriptive filenames
4. Update documentation if adding new categories

## 📚 Additional Resources

- [n8n Official Documentation](https://docs.n8n.io)
- [n8n Community Forum](https://community.n8n.io)
- [n8n Cloud](https://n8n.io/cloud)

---

*Built with ❤️ for the n8n community*