### Dette er et repository for tekstanalysekurs for Abakus 2017.  

#### Vedlagt ligger filer for bruk i Databricks og Tableau.

A. Start med å laste ned Ipyhon notebook fil til lokalt område for opplasting i Databricks   
B. Datafiler for tekstanalyse i Spark behøver ikke hentes ned lokalt, disse vil bli lastet inn via Ipyhon notebook  
Oppgave: 

1. Skaff deg ny bruker/Logg deg inn på Databricks Community Edition. 
  I.Lag et cluster som heter ‘analytics’
  
2. Hent URL for iPython-notebook fra github.com/mariustr/twitter-sentiment
  Text Mining Exercise - oppgavescript
  Text Mining Exercise Complete - fasit  
  II.Importer notebook fra URL i Databricks.

3. Kjør analyse (kjør cellene):
  I.Last inn pakker (ferdigskrevet)

2. Last inn twitterdata (ferdigskrevet)

3. Gjør om til småbokstaver og fjern tegnsetting (ferdigskrevet)

4. Kjør tokenizer som skiller ut enkeltord fra tekst  
I. Lag ny dataframe med ‘id’, ‘text’ og ‘words’

5. Fjern stoppord med ‘StopWordsRemover’-funksjon.

6. Les inn sentimentordbok (ferdigskrevet)

7. Gjør om twitterord til 1 rad per ord (‘explode’) og join inn ord fra sentimentordbok.

8. Lag ny dataframe med snittscore per id. (GroupBy)

9. Legg til snittscore til orginaldata (join on ‘id’)

10. Legg dataframe til S3/Redshift (ikke nødvendig å kjøre, bare til opplysning)

C. For tekstanalyse i Tableau, benytt fil 'twittersentiment.csv'  

### * Ekstraoppgave: TensorFlow er laget for maskinlæring, og kjører på Spark. Se gjennom bildegjennkjennigsanalyse ved å importere en ny notebook i Databricks. Lim inn denne url'en: https://community.cloud.databricks.com/?o=8801939843168883#notebook/3857291424109068

