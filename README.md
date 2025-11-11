/**
 * Ak-GOAT README.md Generator
 * This script creates a stylish, feature-rich README.md for your WhatsApp bot repository.
 * Just run with Node.js (`node generate_readme.js`).
 */

const repoName = "Ak-GOAT"; // 1
const tagline = "âš¡ The ultimate WhatsApp bot for group management, fun, and AI chat! âš¡"; // 2

// 5, 29. Stylish ASCII header
const stylishHeader = `
â–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ•— â–ˆâ–ˆâ•—  â–ˆâ–ˆâ•—     â–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ•—  â–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ•—  â–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ•— â–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ•—
â–ˆâ–ˆâ•”â•â•â–ˆâ–ˆâ•—â–ˆâ–ˆâ•‘  â–ˆâ–ˆâ•‘    â–ˆâ–ˆâ•”â•â•â–ˆâ–ˆâ•—â–ˆâ–ˆâ•”â•â•â•â–ˆâ–ˆâ•—â–ˆâ–ˆâ•”â•â•â–ˆâ–ˆâ•—â•šâ•â•â–ˆâ–ˆâ•”â•â•â•
â–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ•‘â–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ•‘    â–ˆâ–ˆâ•‘  â–ˆâ–ˆâ•‘â–ˆâ–ˆâ•‘   â–ˆâ–ˆâ•‘â–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ•‘   â–ˆâ–ˆâ•‘   
â–ˆâ–ˆâ•”â•â•â–ˆâ–ˆâ•‘â–ˆâ–ˆâ•”â•â•â–ˆâ–ˆâ•‘    â–ˆâ–ˆâ•‘  â–ˆâ–ˆâ•‘â–ˆâ–ˆâ•‘   â–ˆâ–ˆâ•‘â–ˆâ–ˆâ•”â•â•â–ˆâ–ˆâ•‘   â–ˆâ–ˆâ•‘   
â–ˆâ–ˆâ•‘  â–ˆâ–ˆâ•‘â–ˆâ–ˆâ•‘  â–ˆâ–ˆâ•‘    â–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ•”â•â•šâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ–ˆâ•”â•â–ˆâ–ˆâ•‘  â–ˆâ–ˆâ•‘   â–ˆâ–ˆâ•‘   
â•šâ•â•  â•šâ•â•â•šâ•â•  â•šâ•â•    â•šâ•â•â•â•â•â•  â•šâ•â•â•â•â•â• â•šâ•â•  â•šâ•â•   â•šâ•â•   
              Best WhatsApp Group Bot! ðŸš€
`;

const badges = [
  "![Node.js](https://img.shields.io/badge/node-%3E=16.0-brightgreen.svg)",
  "![npm](https://img.shields.io/npm/v/ak-goat.svg)",
  "![Stars](https://img.shields.io/github/stars/akgoat008-sudo/Ak-GOAT?style=social)",
  "![MIT License](https://img.shields.io/badge/License-MIT-yellow.svg)",
  "![CI](https://github.com/akgoat008-sudo/Ak-GOAT/actions/workflows/node.yml/badge.svg)",
  "![Downloads](https://img.shields.io/npm/dm/ak-goat)"
].join(' '); // 7, 32

const screenshots = `
<p align="center">
  <img src="media/screenshot1.png" height="400"/>
  <img src="media/screenshot2.png" height="400"/>
</p>
`; // 8

const gifs = `
<p align="center">
  <img src="media/demo-tagall.gif" height="200"/>
  <img src="media/demo-fun.gif" height="200"/>
</p>
`; // 9

// 3, 4, 34. repo structure
const repoTree = `
\`\`\`
Ak-GOAT/
â”œâ”€â”€ commands/   # All bot commands/modules
â”‚   â”œâ”€â”€ tagall.js
â”‚   â”œâ”€â”€ fun.js
â”‚   â””â”€â”€ ai.js
â”œâ”€â”€ config/     # Settings, .env.example
â”‚   â””â”€â”€ bot.config.js
â”œâ”€â”€ media/      # Screenshots, demo GIFs
â”œâ”€â”€ libs/       # Third-party libraries
â”œâ”€â”€ README.md
â”œâ”€â”€ package.json
â””â”€â”€ LICENSE
\`\`\`
`;

const funFacts = `
#### ðŸ¦„ Fun Fact
Did you know Ak-GOAT can detect spam and auto-mute users? Try !spamshield today!
`; // 30

const featuresSection = `
## ðŸŒŸ Features

- ðŸ·ï¸ One-touch tag-all members in group
- ðŸ¤– AI chat (GPT-powered), ask anything!
- ðŸŽ® Fun commands and games
- ðŸ›¡ï¸ Group anti-link & spam shield
- ðŸ› ï¸ Easy configuration via .env or config file
- ðŸ’Œ Custom welcome & goodbye messages
- ðŸ“ˆ Fast, lightweight, zero downtime
`; // 11

const commandList = `
| Command     | Description                        | Example Usage |
|-------------|------------------------------------|--------------|
| \`!tagall\`     | Tag everyone in group             | \`!tagall\`         |
| \`!ai\`         | Chat with GPT AI                  | \`!ai What's the weather?\` |
| \`!joke\`       | Get a random joke                 | \`!joke\`           |
| \`!welcome\`    | Set welcome message               | \`!welcome Hello!\`  |
| \`!spamshield\` | Enable/Disable spam shield         | \`!spamshield on\`   |
`; // 12

const installationSteps = `
## ðŸš€ Installation & Setup

1. **Clone repo:** \`git clone https://github.com/akgoat008-sudo/Ak-GOAT.git\`
2. **Install dependencies:** \`npm install\`
3. **Setup config:** Copy \`.env.example\` to \`.env\`, fill with your WhatsApp API keys.
4. **Run bot:** \`npm start\`

**Tip**: For more help, see [Installation Troubleshooting](#faq). 
`; // 13, 14, 35

const usageExamples = `
## ðŸ’¡ Usage Examples

- **Tag all:** \`!tagall\`
- **AI chat:** \`!ai Who are you?\`
- **Fun command:** \`!joke\`
`; // 14

const configGuidance = `
## âš™ï¸ Configuration

Edit \`.env\` for credentials and customizations.

\`\`\`
WHATSAPP_API_TOKEN=YOUR_TOKEN_HERE
GROUP_WELCOME=Welcome to Ak-GOAT!
ENABLE_AI=true
\`\`\`

See \`config/bot.config.js\` for advanced settings.
`; // 15

const contributeSection = `
## ðŸ¤ Contribution

Got ideas? Want to fix bugs?  
- Fork this repo!
- Open a PR
- Report issues via GitHub

All contributions welcome. See [CONTRIBUTING.md](CONTRIBUTING.md)!
`; // 16

const licenseInfo = `
## ðŸ“„ License

MIT License â€“ see [LICENSE](LICENSE)
`; // 17

const acknowledgements = `
## ðŸ™ Acknowledgements

Built with [@whatsapp-api-node](https://github.com/whatsapp-api-node).  
Inspired by open-source bots & community.
`; // 18

const changelog = `
## ðŸ“œ Changelog

- v1.1 â€“ Added spamshield ðŸ›¡ï¸
- v1.0 â€“ Initial release ðŸš€
`; // 19

const demoLink = `
## ðŸš§ Demo / Live

[Try Ak-GOAT here!](https://ak-goat-demo.example.com)
`; // 20

const callToAction = `
## â­ Like Ak-GOAT?

- Star ðŸŒŸ this repo!
- Share with friends!
- Submit suggestions for cool new features!
`; // 21

const contactSupport = `
## ðŸ“¬ Contact & Support

Telegram: [@akgoatsupport](https://t.me/akgoatsupport)  
Discord: \`akgoat008-sudo#1234\`  
Email: \`akgoat@botmail.com\`
`; // 22

const friendlyLanguage = `
Ak-GOAT is super easy for beginners â€“ and made for group admins!  
We love friendly questions, silly suggestions, and curious contributors ðŸ™‚
`; // 23

const versionInfo = `
**Current Version:** v1.1 (Stable)  
`; // 24

const ciStatus = `
![CI Status](https://github.com/akgoat008-sudo/Ak-GOAT/actions/workflows/node.yml/badge.svg)  
`; // 25

const securityNotes = `
## ðŸ” Security & Privacy

Ak-GOAT **never** stores chat data or personal info.  
Your groups are safe!  
See [Privacy Policy](PRIVACY.md) for details.
`; // 28

const easterEggs = `
#### ðŸ¥š Easter Egg
Thereâ€™s a hidden command: try \`!goatify\` on any meme!
`; // 31

const whyDifferent = `
## ðŸ¦ Why Ak-GOAT is Different?

Built for SPEED, ease of use, and maximum fun.  
Most bots are boring â€“ Ak-GOAT brings excitement, group safety, and superpowers!
`; // 33

const faqSection = `
## â“ FAQ

- **Bot isnâ€™t responding?**  
  Make sure your WhatsApp API key is set in .env!

- **AI response too slow?**  
  Try enabling fast mode in config/bot.config.js.

- **Where to request features?**  
  Open an issue or ping us on Telegram!
`; // 35

// Final README generator â€“ mixes everything together in right order, with emojis, formatting (6,10)
const readme = `
${stylishHeader}

# ${repoName} ${badges}
_${tagline}_

${screenshots}
${gifs}

${repoTree}

${featuresSection}

${whyDifferent}

${versionInfo}
${ciStatus}

${funFacts}
${easterEggs}

${commandList}

${installationSteps}

${usageExamples}

${configGuidance}

${contributeSection}

${licenseInfo}

${acknowledgements}

${changelog}

${demoLink}

${callToAction}

${contactSupport}

${friendlyLanguage}

${securityNotes}

${faqSection}
`

// Output to README.md file
const fs = require('fs');
fs.writeFileSync('README.md', readme, 'utf8');

console.log('README.md generated successfully! ðŸŽ‰');
