---
name: website-and-blog
description: Build, redesign or update the owner's SpaSphere website, or write and publish blog posts. Use when the owner asks to change their website, copy a site, add a page or section, change images, or write a blog post.
---

Website and blog changes are saved as drafts. The live site doesn't change until the owner reviews the draft and says to publish.

## Website

1. Before building, redesigning or copying a site, call `website_list_blocks` to learn the sections SpaSphere offers.
2. Call `website_get`. A website is every page it lists, not just the homepage. Build or update each live page the owner's request touches.
3. Save changes with `website_save_draft`. For a photo, use `website_set_image`.
4. Run `website_validate` and fix everything it reports.
5. Call `website_get_preview` and give the owner the preview link. Tell them what you changed.
6. Call `website_publish` only when the owner says to publish. Pass the `revision` they reviewed. If the draft changed since, nothing is published, and you show them the new preview.

To undo, `website_list_revisions` shows earlier versions, and `website_restore_revision` brings one back as a draft.

## Images

Content tools use images from the business's media library only. `media_list` shows what's there. To add one, ask the owner for a public link to the image and pass it to `media_import`. You can't create images yourself here. Ask the owner for a photo, or use one already in the library.

## Blog

1. `blog_list` and `blog_get` show posts. Write or edit with `blog_save_draft`, in Markdown. A post that is already live can't be edited here.
2. Show the owner the draft.
3. Call `blog_publish` only when they say to. Pass the `updated_at` they reviewed. `blog_unpublish` takes a post off the site.

## Writing

Write like the owner talks to their clients: warm, calm and specific to their services. No made-up awards, reviews, prices or credentials. Use only what the business's own data says.
