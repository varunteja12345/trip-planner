# Weekend Trip Planner

This project now works as a normal local frontend agent with no GitHub token or Azure setup required.

## What it does

- Plans a weekend trip for a chosen city
- Uses a mock activity catalog for Paris, Tokyo, New York, and Lisbon
- Schedules activities by day with rough timing and capacity checks
- Runs fully in the browser or from the local CLI

## Frontend mode

1. Open a terminal in the project folder.
2. Start a simple local web server:
   ```bash
   python -m http.server 8000
   ```
3. Open this in a browser:
   ```text
   http://localhost:8000
   ```
4. Pick a city, enter the trip request, and click Plan trip.

## CLI mode

```bash
python agent.py
```

Then try prompts like:

```text
Plan a 2-day trip to Paris with a museum and landmark each day.
Plan a 3-day Tokyo trip with food and a day trip.
```

## No-token setup

This version does not require:

- GITHUB_TOKEN
- AZURE_AI_ENDPOINT
- AZURE_AI_KEY

The planner is local and uses the built-in mock catalog.
