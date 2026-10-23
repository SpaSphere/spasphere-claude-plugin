# SpaSphere for Claude

Run your spa or esthetics business on [SpaSphere](https://spasphere.ai) from a conversation with Claude.

## What it does

Ask Claude to update your services and prices, change your hours, add a closed day, or edit your intake forms, packages, memberships, treatment protocols and treatment plans. It can also turn your marketing automations on or off, import a client list, and show how the business is doing. Claude can build and update your SpaSphere website, write blog posts, and write and schedule email newsletters.

The plugin connects Claude to your SpaSphere account through the SpaSphere connector. It adds skills that teach Claude how to work with it: find before changing, show you every change, and wait for your yes.

## How to use it

1. Add SpaSphere from the Claude directory. In Claude Code, you can also run:

   ```
   /plugin install spasphere --marketplace SpaSphere/spasphere-claude-plugin
   ```

   Then connect SpaSphere and sign in with your SpaSphere owner account.
2. Ask in plain words, for example: "Raise the Signature Facial to $135", "We're closed on December 24", "Add a page about our new brow services", or "Write a newsletter for our winter peel promotion".

Changes to your business, such as services, hours, forms, packages and memberships, take effect only after you confirm them in the chat. Website pages, blog posts and newsletters are saved as drafts. They go live or get sent only when you say so.

## What data it sends

The plugin sends only what you ask for, through `https://mcp.spasphere.ai/mcp`, to and from your own SpaSphere account. That covers your business settings, services, website, blog and newsletter content, forms, packages, memberships, and business totals.

Claude never receives client names, contact details, appointment records, intake answers, notes, invoices or payment information. It can't take payments, refund, or delete records.

SpaSphere logs every change made through Claude, with what changed and when. The plugin itself stores nothing and runs no code on your computer.

SpaSphere is for businesses in the United States. Read the [Privacy Policy](https://spasphere.ai/privacy-policy) and the [Terms of Service](https://spasphere.ai/terms-of-service). For help, visit [support](https://spasphere.ai/support) or email hello@spasphere.ai.
