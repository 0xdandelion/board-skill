# Board

**A Claude Code skill that turns strategic planning into alignment between spend and strategy.**

Most companies plan in a vacuum, which results in:

- **Wasteful Spending**: Subscriptions accumulate without clear ownership or measurable impact.
- **Vague Strategy**: Plans are often too abstract to dictate how resources should actually be used.
- **The Execution Gap**: Teams plan for the future without accounting for the resources they are already using today.

Board acts as alignment between your commitments (subscriptions), your intent (strategy), and your output (OKRs).

## What is Board?

Board is a skill for Claude Code. It transforms Claude into a strategic consultant that leads structured planning sessions. Instead of a static document, Board is an interactive process that runs directly in your terminal.

## The Four-Phase Process

Board guides department leads through a high-signal interview:

1. **Q4 Review**: A look back at the previous quarter to turn past performance into 2026 insights.
2. **2026 Strategy**: A deep dive into department vision, major initiatives, and explicit "non-priorities."
3. **The Resource Audit**: The "game-changer" phase. You inventory every tool and map it directly to an initiative. If a tool doesn't support a goal, it is flagged for removal.
4. **Q1 OKRs**: The creation of 2-3 measurable objectives that are hard-linked to your strategy and your tech stack.

## Why Board Wins

| Feature | Traditional Planning | Board |
|---------|---------------------|-------|
| Strategy | Abstract and disconnected | Hard-coded to actual spend |
| OKRs | Created in isolation | Referenced to specific tools |
| Resources | Unexamined "sunk costs" | Every tool must justify its value |
| Output | Inconsistent notes | Structured, ready-to-use artifacts |

## Quick Start

Board requires Claude Code and a Claude Pro subscription.

### Option 1: Clone the repository

```bash
# Clone the repo
git clone https://github.com/0xdandelion/board-skill.git
cd board-skill

# Start Claude Code
claude

# Run the skill
> Run Board
```

### Option 2: Install skill manually

```bash
# Create the directory
mkdir -p .claude/skills/board

# Copy SKILL.md into that folder

# Start Claude Code
claude

# Run the skill
> Start strategic planning
```

Never used Claude Code? See the [Getting Started Guide](https://code.claude.com/docs/en/getting-started).

## Notion Integration (Recommended)

To enable automatic saving to Notion, add the Notion MCP server:

```bash
# Add server
claude mcp add --transport http notion https://mcp.notion.com/mcp

# Restart Claude Code
claude

# Authenticate
# Type: /mcp
# Select: "Authenticate notion"
# Follow the prompts
```

Once authenticated, Board will automatically create a formatted Notion page with a shareable link for your company. If you do not use Notion, Board still generates HTML and Markdown outputs.

## What You Get

Board generates a comprehensive planning artifact including:

- **Q4 Review**: Outcomes, learnings, and lessons.
- **2026 Strategy**: Success criteria, challenges, and initiatives.
- **Subscription Inventory**: Tools categorized by alignment (Aligned, Review Needed, or Misaligned).
- **Spend Map**: Visual clarity on how budget aligns with strategy.
- **Q1 OKRs**: Key results, projects, and subscription mappings.
- **Planned Launches**: Targets and dates.

## Integration and Privacy

**Notion Sync**: Board can automatically generate and save your planning artifacts to a formatted Notion page for company-wide access.

**Professional Output**: If you don't use Notion, Board provides styled HTML files and clean Markdown.

**Privacy First**: All data stays on your local machine. Your planning conversations are not shared with the skill author, and no raw data is stored outside of your Claude session.

The output isn't just a document; it is a **Spend → Initiative → OKR map** that ensures your money and your goals are moving in the same direction.

## Cost and ROI

**Board Skill**: Free

**Claude Pro**: $20/month

A single strategic planning session often uncovers thousands of dollars in misaligned spend. The subscription pays for itself by identifying immediate waste.

## Who is this for?

**Department Leads**: Preparing for annual or quarterly planning.

**Founders**: Prepping for board meetings or investor updates.

**Finance Teams**: Auditing subscription spend against actual output.

**Executives**: Ensuring strategy and resource allocation are perfectly synced.

## FAQ

**How long does a session take?**
Typically 30 to 60 minutes for a thorough interview, depending on the complexity of your department.

**Can I customize the questions?**
Yes. You can edit the `.claude/skills/board/SKILL.md` file to modify interview questions, change the output format, or add custom sections.

**What if I don't have Q4 OKRs documented?**
Board is adaptable. If you don't have existing OKRs, it will guide you through a free-form reflection to capture the necessary context.

**Does this work for personal planning?**
Absolutely. You can replace "company strategy" with personal goals and "subscriptions" with your recurring personal expenses.

## Inspiration

This skill was built on the philosophy that strategic planning is meaningless without resource allocation. It was specifically inspired by:

- Brandon Gell's generous prompt sharing on AI-powered strategic planning (he works at [Every](https://every.to/)).
- [just-fucking-cancel](https://github.com/rohunvora/just-fucking-cancel) by @rohunvora: A brilliant Claude skill for auditing personal subscriptions.
- The realization that strategic planning should be connected to actual resource allocation.

## License

[MIT License](LICENSE) — Use it, customize it, share it.

---

**Built with Claude Code** • [Documentation](https://code.claude.com/docs) • [Report Issues](https://github.com/0xdandelion/board-skill/issues)
