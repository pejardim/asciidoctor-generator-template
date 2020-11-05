namespace :build do
task :pdf do
`bundle exec asciidoctor-pdf -apdf-style=themes/custom-theme.yml -a pdf-fontsdir=themes/fonts Androiderrors.adoc -o output/Androiderrors.pdf`
end
task :html do
`bundle exec asciidoctor Androiderrors.adoc -o output/Androiderrors.html`
end
end
desc 'Build all default formats'
task :build => [ 'build:html', 'build:pdf' ]
