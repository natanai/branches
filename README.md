# Branching Dialogue Editor

A lightweight, single‑page web app for designing and testing branching dialogue. Built to run entirely in the browser—no server required—and optimized for mobile and desktop use.

## Features

- **Create Branching Dialogues**: Add NPC lines and multiple player responses for each node. Player responses can link to existing nodes or create new branches.
- **Playable Conversation**: Use the “Play” button on any response to walk through the conversation and see the dialogue exchange as it would appear in-game.
- **Conversation Log**: A vertical log shows the back‑and‑forth between the NPC and the player as you navigate, with clickable NPC lines to jump back to any previous point.
- **History & Navigation**: A history trail lets you move backwards through the conversation or jump directly to any node from the dropdown.
- **NPC Naming**: Specify an NPC name, which is reflected in the conversation log and in the saved filename.
- **Save / Load**: Export and import conversations as plain text (`.txt`). Saved files include the NPC name in their filename (e.g. `Cranberry-dialogue.txt`), and importing will always start the dialogue from the first node. JSON support has been removed to keep things simple.

## Using the Editor

1. **Add a Node**: Click **New Node** to add a fresh dialogue node.
2. **Edit NPC Dialogue**: Enter the NPC’s line in the large text box.
3. **Add Player Responses**: Click **Add Response** to create a new player option. Use:
   - **Create Branch** to make a new node linked to this response.
   - **Link…** to connect the response to an existing node.
   - **Play** to simulate the conversation by following that response.
4. **Navigate**: Use the **Go to Node** dropdown, the **Back** button, or click NPC lines in the conversation log.
5. **Refresh Names**: If you edit a node’s text or the NPC name, click **Refresh Names** to update all dropdowns and logs.
6. **Save**: Click **Save TXT** to download a `.txt` file containing all nodes and links. The NPC name is part of the filename.
7. **Load**: Click **Choose File** and select a previously saved `.txt` file. The editor will load the conversation, set the NPC name from the filename, and start at the first node.

## Hosting on GitHub Pages

This app is a single HTML file, so you can host it easily with GitHub Pages:

1. Create a new repository and add `index.html`.
2. In the repository settings, enable GitHub Pages from the root of the `main` branch.
3. Visit the Pages URL (e.g., `https://yourusername.github.io/your-repo`) on your phone or desktop to use the editor.

## Roadmap

The current feature set is stable—future improvements will maintain existing functionality. Potential enhancements include:
- Search/filter nodes by content.
- Visual graph view of dialogue flow.
- Export adapters for specific game engines.
