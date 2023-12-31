# Posit-CS-Quarto-Deck

Basic Quarto slides for agenda and team review

## Before Use

Fill in the parameter values in the YML frontmatter of the "Posit_Agenda_and_Contact_Slides.qmd" and edit the "Agenda", "Strategic Goals for your Posit software", and "Posit Resources & News" slides as needed. The "The Teams" slide will automatically populate based on the parameters.

"embed-resources" is set to "true" by default. This setting allows you to send the rendered html document to your meeting attendees without having to include a folder of assets. This significantly slows rendering so if this is not a feature you need consider setting this to false in the YAML front matter of the quarto document.

### Required Packages

[Quarto](https://cran.r-project.org/web/packages/quarto/index.html)

[Knitr](https://cran.r-project.org/web/packages/knitr/index.html)

[bizdays](https://cran.r-project.org/web/packages/bizdays/index.html)

## Usage
### Parameters
To customize your presentation populate the YAML parameters at the top of the document with the relevant information. To alter your agenda or goals navigate to the slides that render those sections and modify the bullet lists as needed. The team and license slides will pull the relevant information from the parameters that you define and automatically render.

### Images

Image links can be acquired by right clicking the relevant linkedin profile picture or company logo and clicking "Copy Image Address" from the menu. This is the link that is used in the "linkedin" parameters and "customer_logo" parameter. This means that if the image is updated your presentation will also update accordingly.

### embed-resources

The embed-resources setting will create self contained HTML files when marked True which can be sent to meeting attendees. If false the documents will only render correctly if opened from the project directory.

## FAQ

### Why not pptx?

If Quarto has a way to dynamically embed images (like the "The Teams" slide and Title slide rely on) in a powerpoint document I have not found it. When missing this functionality rendering from Quarto doesn't have a lot of utility, and a powerpoint template would be equally as effective.

### How can i live edit the document?

If you have two monitors you can change the slides on the fly in the quarto document and render when ready. The document will render and keep you on the same page in your browser. Unlike PowerPoint folks won't be able to see you type as you go, but once you get the hang of it it's not too different.

## Special Thanks

Tom Mock built a [great extension](https://github.com/jthomasmock/positslides) with all of the backgrounds, and a lot of the theme that i used as the foundation to build this template.
