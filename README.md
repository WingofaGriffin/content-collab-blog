# Exploring Content Collaboration Platforms for Developer Blog Writing

As a Developer Relations professional, I spend a pretty large amount of my time writing, organizing, and collecting content for publication on our blog to the point where it is necessary to have a solid project management system to keep everything in order.

## The Requirements

![Dolby.io Blog](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/lotydjciqezlyxuuroj6.png)

At Dolby.io we collect content from a multitude of people in multiple different mediums, but at the end of the day we want to keep everything centralized and consistent when possible. Our blog is handled in the backend using [Wordpress](https://wordpress.com/), so when considering options for content management it was critical that it played well enough with Wordpress with little manual modifications needed. Because of this, there were a few "must haves" for the platforms to consider.

#### 1. Exceptional handling of code blocks and inline code

This is a developer blog after all, so there needs to be proper ways to share code. Ideally this will contain proper syntax highlighting for languages used as well, and has good copy-paste ability.

#### 2. Commenting and editing is simple

As this is a collaboration platform, we want the collaboration tools to be robust. Being able to comment on sections of text or the whole document easy to do and follow, with a bonus for tools like "Suggest Edits" for inline changes.

#### 3. Intuitive project management tools

With the scale of posts written over time and the large number of contributors, keeping track of the status and metadata of posts within the same system they are written in is a huge benefit. This helps managers figure out the status and what is missing at a glance, and automatically populates based on the original edit.

#### 4. Able to handle multiple users editing at the same time

We don't want collisions to happen if two people are editing at the same time, as that can result in a lot of lost work and wasted time. Ideally this will be a living document that updates automatically.

#### 5. Image and other media handling not tied to their servers

As the content will all be copied into Wordpress, we want to ensure media doesn't copy the internal reference instead of the base file. Otherwise it can look fine for people connected to the company network, but not to the public.

#### 6. Cross-platform

We have team members on multiple different platforms who should all be able to contribute. The best solution for this is a web app.

### Nice to Haves

There are a few other bonus points that can help separate the good from the great that I considered:

- Low price or a free tier that fits our needs
- Version history management
- Markdown based editor as either a default or an option alongside a rich-text editor

### Immediate Outs

With these rules, some popular tools were immediately thrown out and will not be discussed in further length.

[Google Docs](https://www.google.com/docs/about/), [Office 365](https://www.microsoft.com/en-us/microsoft-365), and [Box Notes](https://www.box.com/notes) all do not have great code block handling, and were taken out of consideration.

Tools like [GitHub](https://github.com/) are enticing for purely technical teams, especially with their [Projects](https://docs.github.com/en/issues/organizing-your-work-with-project-boards/managing-project-boards/about-project-boards) feature, but we work with a mixture of backgrounds that make these products too high a barrier of entry. The same applies for LaTex collaboration software like [Overleaf](https://www.overleaf.com/).

Similarly, cloud based Markdown editors such as [HedgeDoc](https://hedgedoc.org/), [StackEdit](https://stackedit.io/), [HackMD](https://hackmd.io/) and [Draft](https://draftin.com/) among others are not great choices for those who don't have Markdown experience, plus are a bit more barebones than desired for project management.

Apps like [Slick](https://slickdocs.com/) are MacOS only, which doesn't work for team members on Windows or other platforms.

## Products I trialed

In no particular order, here are the products I tried out, and my thoughts on how they worked for **us**. Keep in mind that just because something might not be a good fit for our workflows doesn't mean it isn't perfect for yours.

### 1. [Confluence](https://www.atlassian.com/software/confluence)
![Confluence Image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/46xziwfyosq0bfuhczzy.png)

Confluence is a tool that a vast majority of people working in tech in the last 15 years are familiar with due to it being a part of the Atlassian ecosystem, in which Jira has been a centerpiece of modern tech workflows. I've used Confluence in every single job I've worked at for this reason, and I tend to have a love/hate relationship with it. It's an extremely powerful tool that allows massive customization of the spaces it has, links very well with itself and Jira, and provides third party extension support for workflows that it doesn't support out of the box.

However, it feels dated with the implementation of a lot of these benefits, where just because the option is there doesn't mean that the option was elegantly implemented. For example, code blocks are supported, but require you specifically use a code block macro that is its own container instead of living with the other in line text. It also uses its own markup syntax, which makes taking existing Markdown that you may already have not as simple as copy-pasting it into the platform. Other small quirks like it needing to host every file you upload to it, having a functional, yet quirky way of dealing with simultaneous edits, and the typical Atlassian sentiments many tech workers know make it a compromise.

We use Confluence already at Dolby.io, and I imagine many of you reading this are also using this tool already, so the price is already right. The best way to sum up my feelings of Confluence are "if it ain't broke, don't fix it", which fits some team's philosophies more than others.

### 2. [Notion](https://www.notion.so/)
![Notion Image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ujei124wzqp20thlfqge.png)

Notion is the relative new big hitter coming to the block with a recent surge in users that has slowly started taking up the startup scene. Notion is what I would describe as the Atlassian suite if it was made with modern tech design, and it shows from the visual aesthetic to the technical decisions made in what it supports. Instead of separating the company into multiple products however, it is all grouped in one workspace, where you can link tables, docs, kanban boards, and more together seamlessly and it frankly feels very elegant.

Notion uses Markdown as its text processor, though instead of keeping the raw text, it automatically interprets it to make the lives of writers a bit easier, though not as intuitive as a traditional rich-text editor. If text is highlighted, it brings up the command palette, though this isn't the most intuitive behavior for new users. I would say it is similar to Slack's editor, which makes sense due to the high user base.

Overall I was a big fan of Notion, and its growth tends to support my sentiment, as I see more and more companies start using Notion as their main platform for nearly everything. I will note that I have had server issues in the past with Notion with issues like slowness to not being able to access my documents, though I have not experienced it in recent tests of the platform, and can likely attribute this to its growing pains.

### 3. [Quip](https://quip.com)
![Quip Animation](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/rrwunx5vx9zwo23khcny.gif)

Quip is Salesforce's option in the content collaboration space with a heavy focus on live discussions, with chat, edits, and its integration with Salesforce being its key marketing points.

While it was able to do match these claims in experience, overall it really does seem like this is built for sales teams, not content creation, where a lot of the project management assumes heavy Salesforce use, whom I imagine are the target customers for this product.

### 4. [Dropbox Paper](https://www.dropbox.com/paper)
![Dropbox Paper Animation](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/9l8tgusmlzvhsprda578.gif)

Unlike its major competitors in Google Docs and Box Notes, Dropbox Paper has native support for code blocks, which was a huge boon in its usability for technical content. It's another Markdown based editor with rich-text interpretation, not unlike Notion's offering. It still has commenting support and version history built in (including comment history) which makes it great as a living document solution.

This is where the benefits dwindle though, as its project management capabilities are virtually non-existent, being a cloud-storage solution first. Additionally it played strangely with Wordpress, where linespaces were not kept and code blocks weren't recognized properly. If your team is already using Dropbox as the storage provider, this is an option for consideration, though I wouldn't suggest it except for the most basic of needs.

### 5. [Coda](https://coda.io)
![Coda Animation](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/sjjjmnr6s361sn23nlkm.gif)

Upon asking my fellow DevRel community which tools they enjoyed using, Coda was one that was brought up a few times, but with the caveat that it was "highly technical" and more like a Smartsheet or Airtable than a collaboration document solution. I agree with this take, where instead of the previous couple feeling more like a document centric solution, this one felt like more of a project management solution, where content wasn't managed as well as Notion or Confluence.

To be fair, this is not Coda's intent with the platform, instead directly making the statement [Docs are the new blogs](https://coda.io/publishing), where they encourage you to use Coda as the publishing platform. Coda itself looks like a super promising and interesting tool for an alternative blogging process.

### 6. [Slab](https://slab.com/)
![Slab Image](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/fdzuumb9xn5rw4nf6478.png)

With Slab we return back to the "content-first" sub-category of solutions where we have another Markdown based editor with a few bells and whistles added for ease of use. Some of these include a content map that helps visualize the assortment of categories your documents live in, templating, and robust commenting solutions.

Once again, project management is limited, though they have built in integrations with Jira and Miro among others that imply that it isn't meant to be that and you should be using tools dedicated to that workflow for that purpose. 

### 7. [Walling](https://walling.app/)
![Walling Animation](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/hovwxd1no7bq8vp4gvbw.gif)

Walling is another project management based solutions which takes advantage of a "grid-like" workspace for organizing content between "walls" while using Markdown as the editor. This makes keeping information like publishing metadata and checklists very pleasant to work with, as they have their own dedicated space instead of needing to format your document in a way that has them live inline with the actual content.

Despite these features, there isn't a great tabling solution, and there isn't a great way to link to other posts in the workspace. It also didn't really feel like it was built for collaboration, as commenting isn't a super intuitive process at all. 

### 8. [Whimsical](https://whimsical.com/docs)
![Whimsical Animation](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/bsf54euypt0p7z8j8115.gif)

Whimsical is all about keeping all content in an organized, central place. They center around five main types of content: docs, flowcharts, wireframes, mind maps, and sticky notes that can all be embedded within another. However, it felt more catered towards a creative organization rather than a robust project management feature, as I couldn't find a distinct way to properly create a workflow that autopopulated content when a new document was made.

The benefits of small things like live cursors and linking content within content were useful. It also had the added benefit of working well with Wordpress, where images were not directly copied, but an image upload object was created in its stead, ensuring that you uploaded a proper copy of the image.


### 9. [ClickUp](https://clickup.com/)
![ClickUp Animation](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/t9t7nuz17kqm6jjwu2a4.gif)

ClickUp have been advertising heavily lately with banners all over San Francisco, and when I tried it there was a lot going for it. ClickUp has spaces dedicated for both "Spaces", or your tables of project management based content, and "Docs", which uses a Markdown based editor and organizes and shares your content.

The spaces section reminded me a lot of Airtable with a bit more stuff going on, letting you expand each entry to see the editing history, to do list, attachments, and all, really solidifying itself as a proper "entry" of work to be done. The docs had useful tools like attributing authors and having ample version history. As a major bonus, content copied itself super well into Wordpress, which is a major time save in not needing to reformat every piece of content posted.

Issues however started to appear once I tried mixing the spaces with the docs. Oddly, they didn't play super well together, where there was no great way to link a new doc as an entry into a specific space the same way you can with Notion and Confluence. You can paste the docs content into a space entry, or link a doc to an entry as an attachment that links to the doc, but I found no way to automate this process. This meant every single new doc I wanted to make also required me to make a new entry in the space I was recording the status on, and manually modify the metadata in the space each time the doc was updated.

I was close to being satisfied with ClickUp as my "Goldilocks" solution for my issues, but it just barely missed the mark for being something worth migrating to. It feels like they were trying so hard to replace a large number of competitors that they missed some of the nuances that made their competitors stand out. I am optimistic that as they grow, some of these missing features are implemented into the platform.

## Final thoughts

After my time trialing with all of these platforms (and unsubscribing from all of their mailing lists...), it helped me sort out what exactly was best for me in a content collaboration app, and where my biases landed. Clearly these solutions have their own strengths and weaknesses, and all have a very solid number of customers that use them daily.

If I had to choose my favorite today (October 2021), **Notion** was my overall winner, where if I was starting completely from scratch, Notion filled the majority of my needs and had a good user experience. It was easy to organize, edit, collaborate, and more in a way that facilitated as many automated processes as possible.

However, I am not starting from scratch, and there are tradeoffs to migrating interfaces. So for that reason, we have decided to stick with Confluence, as all of our content is already there, we already pay for it, and it doesn't require our team members to sign up for a new account anywhere. A bit anti-climactic, but none of the solutions we found offered enough more than Confluence to be worth the resource investment to migrate.

I suggest taking advantage of the free trials these platforms provide, though I hope this rundown provided some good context of what pros and cons each have to see if there is a good fit for your team. Remember that what my teams needs are might not be reflected in yours, and these products are all actively being worked on. Missing features can be added, and beloved features can be sunset. I'd love to hear what solutions you are using in the comments and see if there are any promising contenders I may have missed!
