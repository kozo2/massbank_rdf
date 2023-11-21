# massbank_rdf

```
docker run -it THE_IMAGE_NAME bash
git clone https://github.com/skwsm/massbank_rdf
git clone https://github.com/MassBank/MassBank-data
cd massbank_rdf
mkdir output
cd lib
for i in ../../MassBank-data/*/*.txt; do name=`basename -s txt $i`; ruby ../bin/massbank2rdf.rb $i ../output/${name}ttl; done
```
