https://www.imdb.com/interfaces
https://datasets.imdbws.com

cat title.basics.tsv | awk -F"\t" '{print $1, "|" , $6, "|", $4, "|", $3}'

grep -h Halunke title.akas.tsv title.basics.tsv  | sort -u -k1,1

