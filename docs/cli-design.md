# CLI Design: Social Media Trend Analyzer

## Objective
Create a user-friendly, interactive CLI application that guides content creators to find trending topics. This tool will replace the raw API response with a conversational interface and clean, formatted output.

## User Interface & Experience
- **Interaction:** The tool will interactively prompt the user:
  1. `Enter Platform:` (user types: `tiktok`, `youtube`, or `instagram`)
  2. `Enter NICHE:` (user types: e.g., `gaming`, `cooking`)
- **Visuals:** Use the `rich` library to present data in formatted tables for better readability.
- **Feedback:** Use spinners/progress bars while the scraper is running to provide visual feedback.
- **Robust Error Handling:** Catch scraping errors (e.g., connection issues) and display user-friendly messages.

## Implementation Steps
1. **Interactive CLI:** Use `questionary` or `click.prompt` for sequential user input.
2. **UI Formatting:** Integrate `rich` for tables and console output.
3. **Refactoring:** Move scraping logic from the FastAPI skeleton into reusable modules.
4. **Validation:** Implement input validation for platform and niche.

## Proposed Output Example
```
Enter Platform: instagram
Enter NICHE: gaming

Analyzing... [Spinner]

| Topic              | Growth |
|--------------------|--------|
| Easy Vegan Dinners | High   |
| Air Fryer Recipes  | Medium |
```

## Next Steps
- Review this updated design plan.
- Confirm approval to proceed with CLI development.
