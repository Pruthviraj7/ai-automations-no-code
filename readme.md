# AI Automations No-Code  
A collection of no-code / low-code automations using Make.com + OpenAI + other tools to power LinkedIn workflows and more.

> 💡 You’ll find ready-to-import blueprints, instructions, prompts, and examples for automating LinkedIn tasks with minimal code.

---

## 🚀 Current Automations

| Name | Description |
|---|---|
| **LinkedIn Latest Jobs** | Fetch latest job listings from LinkedIn → enrich via OpenAI → append to Google Sheets |
| **LinkedIn Post Automation** | (Add a short description of what this module does) |

> More automations will be added over time — this repo is your central place for all active “AI + no-code” workflows.

---

## 📂 Repository Structure

```
ai-automations-no-code/
├── linkedin-latest-jobs/
│   ├── latest-jobs-make-automation.json
│   ├── instructions.md
│   └── (screenshots, helper files)
├── linkedin-post-automation/
│   ├── (json, instructions, assets)
│   └── …
├── readme.md  ← (this file)
└── LICENSE (if applicable)
```

- Each folder represents one automation blueprint + instructions.
- JSON files are importable into Make.com (or similar).
- `instructions.md` within each folder details step-by-step setup for that automation.
- Screenshots or visuals should be placed in each automation folder (e.g. `images/` subfolder).

---

## 🛠️ How It Works (Overview)

Here’s the typical flow for automations in this repo (e.g. **LinkedIn Latest Jobs**):

1. **RSS / Trigger**  
   Pull job or post URLs from an RSS feed, webhook, or other source.

2. **HTTP / Fetch Details**  
   Make an HTTP request to the URL from step 1 to get the full payload (HTML / JSON).

3. **OpenAI Module**  
   Use a GPT model to parse the raw payload into a clean JSON object containing fields (e.g. title, company, location, date, link).

4. **Destination / Storage**  
   Save or route the parsed job/post info to Google Sheets, databases, or downstream tools.

While each automation can differ slightly, this pattern (Trigger → Fetch → Enrich → Store) is common across all.

---

## ✅ Setup Guide (for a given automation folder)

1. Open the folder (e.g. `linkedin-latest-jobs`)  
2. Follow its `instructions.md` — ideally the steps are consistent across automations.  
3. Replace placeholder URLs, keys, and connections with your own (RSS feed, OpenAI key, Google Sheets, etc.).  
4. Import the `.json` blueprint into your automation tool (Make.com, etc.).  
5. Run a test to verify data flow end-to-end.

---

## ✍️ Prompt Templates

Each automation includes a prompt template used inside the OpenAI module.  
You’re free to tweak it, add more fields, or adjust formatting — just ensure the JSON schema aligns with your sheet/target.

---

## 🧪 Testing & Troubleshooting

- Use sample data with just a couple of items to test flow.
- Check execution history in Make.com (or your tool) to see failures or mapping issues.
- Confirm the output JSON fields exactly match your Google Sheets headers.
- Watch for API rate limits or malformed responses.

---

## 🗓️ Roadmap & Future Features

- Add more LinkedIn automations (e.g. auto-post, comment analyzer).  
- Expand beyond LinkedIn (e.g. Twitter, GitHub, job boards).  
- Make a central dashboard to run and monitor all automations.  
- Add retry logic, error alerts, logging, and versioning.

---

## 📜 License & Contributions

- (Optional) Specify your license, e.g. MIT.  
- Contributions are welcome — if you build a new automation, add its folder + instructions + blueprint.

---

## 🙏 Acknowledgments

Thanks to openAI, Make.com, and the broader no-code community for inspiring these automations.
