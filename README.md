# MeshStudio Website  <img src="https://avatars3.githubusercontent.com/u/15943839?s=200&v=4" width="30" height="30"> 
This is the repository for the Mesh Studio website.

## Developing

#### Site Generation

To simply transpile all of the site code, running:
```
$ hugo
```
Will deposit all final artifacts into the `./public` directory.

#### Site Development

If you would like to develop on the site, it is best to run the server that Hugo provides. To start the development server, run: 
```
$ hugo server
```

The resulting site will be located at `http://localhost:1313`. Hugo server comes with LiveReload support. To enable LiveReload, you need to have the appropriate browser plugin. Please check with your browser's add-on market for the applicable add-on

## Deployment

TBD... not there yet.

## Content

### Site Content

There should never be any content embedded directly in the HTML. All content for the site needs to be sourced from the `/content` directory. This includes all site copy, blog posts, and case studies.

### Site Pages

A site page is considered one of the main naviagatable pages (e.g. `/blog` or `/services`). The content for these pages is derrived from the `_index.md` file in the respective folder in the `/content` directory.

For example, the `/services` page's content can be found in `/content/services/_index.md`

### Case Studies

A case study is an overview of our engagment with a client. The content for these pages is sourced from the name of the casestudy (e.g. `staples.md`), which can be found in the  `/content/work` directory.

#### How to create a new case study

To create a new case study, you can simply run the following command:

```
$ hugo new work/{CASE_STUDY_NAME}.md
```

This will create a new case study template in the `/content/work` directory. The top portion will is templated meta information needed about the case study for it to work properly with the site.

#### Required Images (Case Studies)

##### Logo

All logos should be in a vector format, SVG is preferred. If you need help sourcing one of these, ask a team member for help.

##### Hero Image

- A 200x770px hero image is required for all case studies. We are enforcing a resizing at 200px height, so the 770px width should be considered a maximum. Again, if you need help sourcing/creating one of these, grab a team member.

### Blog Posts

Our blog posts will be hosted on this site as well in the `/content/blog` directory. 

#### How to create a new blog post

Our blog post filenames need to be prefaced with the date they were created in the following format:
`YYYY-MM-DD`. To create a new case study, you can simply run the following command:

```
$ hugo new blog/{YYYY-MM-DD-BLOG-TITLE}.md
```

This will create a new case study template in the `/content/work` directory. The top portion will is templated meta information needed about the case study for it to work properly with the site.


#### Required Images (Blog)

##### Hero Image

- A 200x770px hero image is suggested for all blog posts. We are enforcing a resizing at 200px height, so the 770px width should be considered a maximum.
