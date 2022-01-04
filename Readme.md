## UAS-SISTEM-REKOMENDASI-FILM-MENGGUNAKAN-MATRIX-FACTORIZATION
## NAMA : ARIE BAGAS AZZY
## NIM  : 181011400122

Untuk Menjalankan dalam terminal:    

```
python3 main.py ratings.dat -d :: -uc (0,1,2) -dt int -m cv -nf 5 -l True -li True -s 100 -lr 0.005 -lreg 0.05 -fe 10 -i 75    
```    
Within Python (in this example for no CV, where we split train/test into 80/20):   
```python
import main
main.MatrixFactorization(ratings.dat', 
                         delimiter = "::", 
                         useCols = (0,1,2), 
                         dtype = int, 
                         percTrain = 0.8, 
                         seed = 150, 
                         learningRate = 0.003, 
                         lambdaReg = 0.04, 
                         numFeatures = 15, 
                         iterations = 60)

```



