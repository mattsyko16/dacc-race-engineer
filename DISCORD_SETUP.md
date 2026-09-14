# Discord setup

1. Open the Discord Developer Portal:
   https://discord.com/developers/applications

2. Create or open **DACC Race Engineer**.

3. Copy the public **Application ID** from General Information and paste it into `config.js`.

4. Host the app on HTTPS. For a first test, GitHub Pages is sufficient.

5. In the Developer Portal, enable/configure the app as an **Activity** and add a URL mapping to your hosted app URL in the Activities / URL Mappings area.

6. Install/add the application to your DACC Discord server using the install settings in the Developer Portal.

7. Launch the Activity from Discord and confirm the top-right badge changes from **Standalone** to **Discord Activity**.

Do not paste a bot token or client secret into `config.js`, GitHub, Discord chat, or ChatGPT.

## Slash commands

The current MVP is front-end only. The UI is race-ready without a bot backend.
A second phase can add `/fuel`, `/next`, `/swap`, and `/stints` using a very small serverless backend.
