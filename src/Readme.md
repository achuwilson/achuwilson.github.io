
To run on local sysytem, install hugo extended for linux
then from this directory, run 
`hugo serve`

To add a new publication type:, add a new catogary-id in themes/hugo-academic/data/publication_types.toml, then add corresponding id and string in the language files( themes/hugo-academic/data/i8n/en.yaml)

Place the pdf of publications in static/pdf/file.pdf and refer it in files as pdf/file.pdf

To add a new tag for the project type. add it to content/projects/projects.md
