# Deep Crawl Prompt: Check for New Components

To check for new components:
- Periodically perform a deep crawl of the Apollo UI documentation site (https://cjx-apollo-ui.netlify.app/docs/components/) to detect any new or updated components.
- Compare the discovered components with the local `docs/` directory and `components.md` list.
- For any new components found, repeat the extraction and JSON creation process as described in the documentation sync process.

This ensures the local JSON documentation stays in sync with the official Apollo UI documentation and is structured for easy consumption by other tools or documentation systems.
