# ACM SIGHPC Education Chapter Website

## Contributing events or content

Chapter members can contribute events or edit / add content to the SIGHPC Edu 
website. The workflow is

1. Fork the [website repository](https://github.com/sighpcedu/sighpcedu.github.io) on GitHub.
2. Make your changes or add your event.
3. Submit a [Pull Request](https://github.com/sighpcedu/sighpcedu.github.io/pulls) to the main repository and tag @georgiastuart, @stevengordon22, or @scallag for review.
4. Once your PR is approved, it will be merged into the main website and deployed.

If you have questions or need assistance adding your event or content, please email [Georgia Stuart](mailto:gstuart@umass.edu).

### Creating an event

Events are markdown files with the following format (note, anything inside `{{/* COMMENT */}}` is a comment about the field and should be removed prior to ):

```markdown
---
Title: Event title {{/* A descriptive title for the event */}}
EventDate: 2023-12-31 {{/* Event date in YYYY-MM-DD format */}} 
EventTime: 14:00:00 {{/* Event time in 24 hour HH:MM:SS format */}}
TimeZone: America/Denver {{/* Event time zone in TZ Database format  */}}
category: event
Date: 2023-10-02T-9:00:00-06:00 {{/* This is the PUBLISHED date, any date in the future will not be published to the deployed website */}}
location: Example Location, Anywhere, USA {{/* OPTIONAL: location of the event */}}
Summary: A short summary {{/* OPTIONAL: A summary that replaces the autogenerated summary in list view. Useful for events with ugly previews. */}}
---

Event description here.

```

Event files are located in `content/events`. Note that event files must have a unique name (e.g., `youreventname.md`) in the events directory to not conflict with or overwrite a prior event. 

### Editing content

The page files for committees are located in `content/committees/<committee name>/index.md`. Any content following the frontmatter (e.g., the variables enclosed in `---` at the top of the document) will be rendered in markdown on the committee page.

### Building the website locally

Coming soon!


