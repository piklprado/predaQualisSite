---
title: Metodologia
---

## 1. Compilação de uma lista de periódicos potencialmente predatórios combinando as seguintes bases:

* [Lista de periódicos publicados pela editora OMICS](/omics.csv), uma das maiores editoras reconhecidamente predatórias [^4].

* Lista de Periódicos com práticas questionáveis criada por Jeffrey Beall. A lista foi tirada do ar[^3] mas há cópias disponíveis em vários sites, (e.g.  http://beallslist.weebly.com/) . Extraímos dessa base de dados:
	* [Standalone Journals List](/beals.csv): lista de títulos isolados potencialmente predadores, conforme está na base de Beall;
	* [Periódicos no Scopus de editoras que estão na lista de Beall](/beals_publishers_in_scopus.csv): periódicos incluídos na base Scopus de 2017 (https://www.scopus.com/home.uri) e que são de editoras incluídas nas lista de Beall.


## 2. Cruzamento com os títulos no QUALIS:

* [QUALIS](/areas.csv): classificação de todos os periódicos por cada área, para a avaliação dos programas no quadriênio 2013-2016 (https://sucupira.capes.gov.br/); 

## 3. Filtragem

São retirados da lista:

* Títulos constantes no [Directory of Open Access Journals](https://doaj.org/);
* Periódicos que não seguem estritamente o modelo de acesso aberto (p.ex, cobram taxas de assinaturas).

## 4. Códigos em R e arquivos resultantes:

* [Código em R de processamento dos dados](/verifica_predadores_qualis.R)
* [Base QUALIS com indicação dos potencialmente predatórios](/qualis_id_predadores.csv)
* [Número de periódicos e de potenciais predatórios por área e estrato](/proporcao_pred_estrato_area.csv)
* [Proporção de potenciais predatórios por área e estrato](/n_predadores_inclusivo_area.csv)

[^3]: [Why Beall’s blacklist of predatory journals died. Paul Basken, The Chronicle of Higher Education22 September 2017 Issue No:475](http://www.universityworldnews.com/article.php?story=20170920150122306)

[^4]: https://en.wikipedia.org/wiki/OMICS_Publishing_Group
