namespace :build do
task :pdf do
`bundle exec asciidoctor-pdf -apdf-style=themes/custom-theme.yml -a pdf-fontsdir=themes/fonts server.adoc -o output/server.pdf`
end
task :html do
`bundle exec asciidoctor server.adoc -o output/server.html`
end
end
desc 'Build all default formats'
task :build => [ 'build:html', 'build:pdf' ]
