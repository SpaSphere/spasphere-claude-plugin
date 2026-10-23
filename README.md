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

## Examples

### Create a blog post

> Write a blog post about how to care for your skin after a chemical peel. Keep it warm and practical, and mention our Brightening Peel.

1. Claude looks up your Brightening Peel so the post uses your real service name and price.
2. It writes the post and saves it as a draft. Nothing is on your website yet.
3. Claude gives you a preview link, so you can see the post as it will look on your site.
4. Ask for changes in plain words, such as "make it shorter" or "add a section on sunscreen". Claude updates the draft.
5. When you're happy, say "publish it". The post goes live on your website's blog.

### Create a newsletter

> Write a newsletter for our winter facial promotion: 20% off the Hydrating Facial through January. Feature the facial and our Winter Glow package.

1. Claude finds the Hydrating Facial and the Winter Glow package so the newsletter shows your real services and prices. If you have a shareable coupon for the promotion, it can add that too.
2. It writes the newsletter and saves it as a draft. Nothing is sent.
3. Claude tells you who can receive it, with how many people in each audience, such as "All subscribers", "Haven't visited in 60+ days" or "Members".
4. Ask Claude to send a test to your own team, up to 5 addresses, and check it in your inbox.
5. When it's ready, tell Claude who it's for and when to send, such as "send it to all subscribers Tuesday at 10 am". Claude confirms the audience and how many people it reaches, then schedules it. You can cancel any time before it sends.

## What data it sends

The plugin sends only what you ask for, through `https://mcp.spasphere.ai/mcp`, to and from your own SpaSphere account. That covers your business settings, services, website, blog and newsletter content, forms, packages, memberships, and business totals.

SpaSphere never sends Claude your client names, contact details, appointment records, intake answers, notes, invoices or payment information. Claude can't take payments, refund, or delete records.

One exception is a client list you import yourself. If you attach a CSV of your clients and ask Claude to import it, Claude reads the file, including names and contact details, and passes it to SpaSphere, which adds the clients to your account. SpaSphere answers with counts only, and Claude is told not to repeat client details. The file you attach is handled by Anthropic under its own terms and privacy policy. If you'd rather not share it, import it in SpaSphere under Clients > Import.

SpaSphere logs every change made through Claude, with what changed and when. The plugin itself stores nothing and runs no code on your computer.

SpaSphere is for businesses in the United States. Read the [Privacy Policy](https://spasphere.ai/privacy-policy) and the [Terms of Service](https://spasphere.ai/terms-of-service). For help, visit [support](https://spasphere.ai/support) or email support@spasphere.ai.
