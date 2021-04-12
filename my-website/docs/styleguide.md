---
title: Style Guide
---

## Documentation Style Guide

A style guide is a set of standards, principles and rules every developer or designer should follow in order to improve the digital presence of the product.

This document defines the standards for the DevOps Portal documentation, including grammar, formatting, word use, and more

## Purpose

The purpose of this document is to define unified standards and guidelines for contributors to the DevOps Portal.

As a developer-focused product, DevOps Portal depends on its documentation to provide a good experience to users who wish to use our product. Thus, it is important that our documentation is complete, concise, and well-written.

Hence, this guide aims to provide some basic guidelines for those wishing to contribute to the documentation.

## Guidelines

### Golden Rule: Assume Nothing (Almost)

Assume as little as possible about your reader regarding the topic at hand. Whenever possible, you should provide links to other Docs and pages which describe how to download, update, and debug certain tools, so that your reader can easily solve an issue without having to go out searching on their own.

Regarding this point, there is a tradeoff. You do not want your text to get too long by teaching your reader how to turn on their laptop (they hopefully have that down), but you do want to instruct them on anything that is **essential** for completing a certain action.

It is dangerous to assume that because something is obvious to you, it will also be obvious to your reader - just keep that in mind.

### Additional Suggestions

#### Use British English

DevOps Portal will be accessed globally, as a result, to keep our communication consistent, we use British spelling for our documentation.

#### Use the Oxford comma for lists

Example: Write "bananas, apples, and oranges", not "bananas, apples and oranges".

#### Capitalise the names of tools, protocols, and technologies

Example: Write "Redis server", not "redis server".

#### Capitalise acronyms

Example: Write "URLs", not "urls".

On another note, try to avoid acronyms unless they're so common that it's weird not to. For example, Hyper Text Transfer Protocol is a weird way to say HTTP.

#### Capitalise every word in a title (except for prepositions)

Example: Write "Documentation Style Guide" instead of "Documentation style guide".

"Style Guide **for** Documentation" is fine, however.

#### Adhere to the style standards of each programming language

In code snippets, you should follow the conventions of the language the code is written in.

Example: Use `camelCase` for JavaScript, and `snake_case` for Python variables names.

#### Where there is a Call to Action, always provide a link

When you write: "You can contact us to learn more", make sure to provide the reader with the means to do so immediately. This could be a link to another page or an email address, for example.

Making sure readers always have immediate access to the next suggested step significantly enhances the reading experience. This way, a reader doesn't have to scour the website to find where the hell the link to the Slack group is.

#### Use in-line code for everything that is found somewhere on the code

Rule of thumb: If it has an underscore, put a backtick around it.

Examples: `API_KEY`, `distinct_id`, `reset()`.

#### Avoid repetition of terms

Example: "We believe this because we believe …"

#### The documentation includes all media types

Include any media types/sources if the content is relevant to readers. You can freely include or link presentations, diagrams, and videos. No matter who it was originally composed for, if it is helpful to any of our audiences, we can include it.

If you use an image that has a separate source file (for example, a vector or diagram format), link the image to the source file so that it may be reused or updated by anyone.

`Do not copy and paste` content from other sources unless it is a limited quotation with the source cited. Typically it is better to either rephrase relevant information in your own words or link out to the other source.

#### Topic types

In the software industry, it is a best practice to organise documentation in different types. For example:

`Concepts`
`Tasks`
`Reference`
`Troubleshooting`

Each page should contain multiple topic types. For example, a page with the title Pipelines, which is generated from a file called index.md, can include a concept and multiple task and reference topics.

#### Work with directories and files

When working with directories and files:

1. When you create a new directory, always start with an index.md file. Don’t use another filename and do not create README.md files.

2. Do not use special characters and spaces, or capital letters in file names, directory names, branch names, and anything that generates a path.

3. When creating or renaming a file or directory and it has more than one word in its name, use underscores (_) instead of spaces or dashes. For example, proper naming would be import_project/import_from_github.md. This applies to both image files and markdown files.

4. For image files, do not exceed 100KB.

5. Do not upload video files to the product repositories. link or embed videos instead.

6. There are four main directories: `user`, `administration`, `api`, and `development`.

7. The `doc/user/` directory has five main subdirectories: `project/`, `group/`, `profile/`, `dashboard/` and `admin_area/`.

       doc/user/project/ should contain all project related documentation. 

       doc/user/group/ should contain all group related documentation.

       doc/user/profile/ should contain all profile related documentation. Every page you would navigate under /profile should have its own document, for example, account.md, applications.md, or emails.md.
       
       doc/user/dashboard/ should contain all dashboard related documentation.
       
       Every category under /admin/application_settings/ should have its own document located at doc/user/admin_area/settings/. For example, the Visibility and Access Controls category should have a document located at doc/user/admin_area/settings/visibility_and_access_controls.md.

8. The `doc/topics/` directory holds topic-related technical content. Create `doc/topics/topic_name/subtopic_name/index.md` when subtopics become necessary. General user and administrator documentation should be placed accordingly.

9. If you’re unsure where to place a document or a content addition, this shouldn’t stop you from authoring and contributing. Use your best judgment, and then ask the reviewer of your MR to confirm your decision. You can also ask a technical writer at any stage in the process. The technical writing team reviews all documentation changes, regardless, and can move content if there is a better place for it.
