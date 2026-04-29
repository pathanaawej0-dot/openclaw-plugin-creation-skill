# OpenClaw Plugin Development Skill

An expert agent skill for building, testing, and publishing native OpenClaw plugins.

## 🚀 The Core Motive: Seamless Self-Extensibility

The primary goal of this skill is to grant **OpenClaw the capability to create plugins for itself.** 

By equipping your agent with this skill, you transform it into a self-evolving system. Instead of waiting for manual updates, the agent can:
- **Write its own tools:** Dynamically generate new tool definitions to handle specialized tasks.
- **Create new channels:** Connect itself to new platforms (Slack, Discord, Telegram) on the fly.
- **Integrate new providers:** Add support for the latest LLM providers or specialized APIs.

Essentially, OpenClaw can now build its own capabilities as easily as creating a custom skill, making its feature set truly seamless and limitless.

## 🛠️ How to Use This Skill

Once installed, this skill is triggered whenever you ask the agent to perform OpenClaw development tasks.

### Example Prompts:
- **"Create a new tool for searching my local database."**
- **"Build an OpenClaw provider for the XYZ API."**
- **"I want to add a Discord channel to my OpenClaw gateway."**
- **"Help me debug my custom plugin manifest."**

The agent will use its expert knowledge of the OpenClaw SDK, manifest schema, and runtime helpers to guide you through the entire development lifecycle—from scaffolding files to final testing.

## 📦 Publishing to ClawHub

ClawHub is the central marketplace for OpenClaw plugins and skills. Since ClawHub auto-indexes the public npm registry, publishing your skill is straightforward.

### 1. Initialize your package
Ensure your skill directory has a `package.json`. If it doesn't, run:
```bash
npm init -y
```

### 2. Configure for OpenClaw
Add the `openclaw` metadata to your `package.json` to help ClawHub identify your plugin's capabilities.

### 3. Build and Package
If your skill requires bundling, ensure your build scripts are ready. For a standard `.skill` file, you can use the `package_skill.cjs` script provided by the `skill-creator` tool.

### 4. Publish to npm
Run the following command to make your skill available on ClawHub:
```bash
npm publish --access public
```
*Note: Once published to npm, ClawHub will automatically discover and index your skill.*

---

*Built for the OpenClaw Ecosystem.*
