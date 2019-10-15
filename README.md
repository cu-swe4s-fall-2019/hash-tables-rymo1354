# Hash tables
Testing different hash functions and search methods. 
Note: random and non-random strings used for hashing. 

## Travis Status

## Installation
To use this package, you should have [Python3](https://www.python.org/download/releases/3.6/) in your environment. You should also have matplotlib installed.

## Utilized Packages
* pycodestyle
* matplotlib

## Usage
`scatter.py` is the main program used to generate plots from the hash function and search method distributions. It uses `hash_functions.py` and `hash_methods.py` to generate these plots. Examples of plots are shown in the `plots` folder.

Note: `binning` and `weighted` hash functions were plotted for EXTRA CREDIT.

### Hash Function Plots
Arguments include:
* input: name of input file, i.e. rand_words.txt, non_rand_words.txt (INPUT)
* hash_method: the method of hashing, i.e. ascii, rolling, etc. (HASH_METHOD)
* table_size: size of hash table (TABLE_SIZE)
* out_file: name of plot, i.e. output file (OUT_FILE)

Format is:
```
python hash_functions.py --input INPUT --hash_method HASH_METHOD --table_size TABLE_SIZE | python scatter.py --out_file 'OUT_FILE' --x_label "Hashed Word" --y_label "Hashed Value"
```
#### INPUT = rand_words.txt, HASH_METHOD = ascii
![](plots/ascii_random.png)

#### INPUT = rand_words.txt, HASH_METHOD = rolling
![](plots/rolling_random.png)   

#### INPUT = rand_words.txt, HASH_METHOD = binning
![](plots/binning_random.png)   

#### INPUT = rand_words.txt, HASH_METHOD = weighted
![](plots/weighted_random.png)

#### INPUT = non_rand_words.txt, HASH_METHOD = ascii
![](plots/ascii_nonrandom.png)             
 
#### INPUT = non_rand_words.txt, HASH_METHOD = rolling
![](plots/rolling_nonrandom.png) 
 
#### INPUT = non_rand_words.txt, HASH_METHOD = binning
![](plots/binning_nonrandom.png) 
 
#### INPUT = non_rand_words.txt, HASH_METHOD = weighted
![](plots/weighted_nonrandom.png)    
