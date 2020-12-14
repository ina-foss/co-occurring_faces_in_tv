# Co-occurring faces in TV

## Description
This archive contains the anonymized version of the data used and introduced in [1].

It is a dataset of facial descriptors with their corresponding anonymized labels. All facial descriptors are also assigned to a program. The facial descriptors assignement to each programs is based on real TV shows broadcasted on French TV as detailed in [1].

## Extraction
The archive is a a tar.gz file split in 3 parts : dataset-anonymized-part00, dataset-anonymized-part01, dataset-anonymized-part02.
You can merge them with the following command :
```
cat dataset-anonymized-part0* > dataset-anonymized.tar.gz
```

## Usage
This archives contains a training set and a test set, respectively 'anonymized_train.h5' and 'anonymized_test.h5'.
The training set size is 548,686 and the test set size is 3,823.
Each one of these archives has 3 fields : "programs", "identities" and "embeddings".
The "programs" field contains program ids as integers.
The "identities" field contains identity ids strings.
The "embeddings" field contains 128-dimensional facial descriptors.

## Credit
If you use this dataset please cite :
[1] Thomas Petit, Pierre Letessier, Stefan Duffner, Christophe Garcia. 2020. Unsupervised learning of co-occurrences for face images retrieval. In 2020 ACM Multimedia Asia.


For any additional information, please contact (in this order or priority) :
tpetit@ina.fr
pletessier@ina.fr
stefan.duffner@liris.cnrs.fr
christophe.garcia@insa-lyon.fr
 
