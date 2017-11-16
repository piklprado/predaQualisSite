# predaQualisSite

Este é o repositório do site **Preda Qualis** - Periódicos potencialmente predatórios no QUALIS-CAPES

https://predaqualis.netlify.com/

## Desenvolvimento

O site é construído usando [blogdown](https://bookdown.org/) e montado com o hugo no [netlify](https://app.netlify.com/).

* Os textos são arquivos markdown (.md ou .Rmd - [instruções básicas](http://rmarkdown.rstudio.com/authoring_basics.html)) no diretório `content`.

* As partes dentro de blocos ```r ... ``` são códigos em R para gerar gráficos, tabelas, etc., que precisa verificar se funfa no R, tem que compilar o site de novo do R com ```blogdown::build_site()```.

* O resto é texto que pode ser editado, e o site é automaticamente reconstruído pelo netlify quando as modificações são enviadas para o GitHub (push ou salvo pelo site do github).

* O site tem também um blog. Para criar posts tem que criar novos arquivos com extensão .md na pasta content/post, no padrão do Hugo.

### Dependências

Algumas dependências no R (além dos suspeitos usuais: tidyr, rmarkdown etc.)

```r
   install.packages(c('blogdown', 'DT', 'VennDiagram', 'captioner'))
   blogdown::install_hugo()
```
