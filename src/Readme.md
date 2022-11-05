
To run on local sysytem, install hugo extended for linux

snap install hugo --channel=extended

then from this directory, run 
`hugo serve`

to update, enter this directory and run  `hugo -d ..`
The static website will be generated in the parent directory.. now sync it with github

To add a new publication type:, add a new catogary-id in themes/hugo-academic/data/publication_types.toml, then add corresponding id and string in the language files( themes/hugo-academic/data/i8n/en.yaml)

Place the pdf of publications in static/pdf/file.pdf and refer it in files as pdf/file.pdf

To add a new tag for the project type. add it to content/projects/projects.md

To add more sections to home page ( highlight papers, tags, experience, etc) -  edit  src/content/home corresponding section

Adding the src/themes/hugo-academic/layouts/partials/widgets/about.html has been edited to 

