## E-graph (E-neighborhood Graph Construction)

**About**

The e-neighborhood Graph or, in general, the e-graph of a data set is obtained conecting two vertices u and v if d(u, v) <= e. E-graph is vulnerable to outliers due to the fixed threshold e.

**Usage**

> kNN execution

    python main.py -f input/square.dat -e 3

> Input: any numerical dataset with any delimiter for attributes

> Output: a weighted undirected graph in the format: filename + '-knn.ncol'

**Parameters**

| Option					| Domain					| Required	| Default	| Description															|
|:------------------------- |:------------------------- | --------- | --------- |:--------------------------------------------------------------------- |
| -f, --filename			| string [FILE]				| yes		| -			| dataset as input file													|
| -o, --output				| string [FILE]				| no		| ncol		| output file															|
| -e, --e					| [1,inf] Float interval	| no		| 3			| epsilon threshold																|
| -t, --threads				| [0,n] Integer interval	| no		| 4			| number of  threads													|
| -e, --format				| ['ncol', 'pajek']			| no		| ncol		| format output file													|
| -c, --skip_last_column	| bool						| no		| true		| skip the last column													|
| -c, --skip_rows	| [1,n-1]						| no		| None		| Skip rows													|

**Dependencies**

* Python: tested with version 2.7.13.
* Packages needed: numpy, scipy and multiprocessing.

**Known Bugs**

Please contact the author for problems and bug report.

**Contact**

* Alan Valejo.
* Ph.D. candidate at University of São Paolo (USP), Brazil.
* alanvalejo@gmail.com.

**License (COPYING.md)**

* Can be used for creating unlimited applications
* Can be distributed in binary or object form only
* Non-commercial use only
* Can modify source-code and distribute modifications (derivative works)
* Giving credit to the author by citing the papers [1]
* License will expire in 2018, July, and will be renewed.

**References**

> [1] Lilian Berton and Thiago de Paulo Faleiros and Alan Valejo and Jorge Valverde-Rebaza and Alneu de Andrade Lopes: RGCLI: Robust Graph that Considers Labeled Instances for Semi-Supervised Learning. Neurocomputing. 2017

~~~~~{.bib}
@article{Berton_2016,
    author={Lilian Berton and Thiago de Paulo Faleiros and Alan Valejo and
    Jorge Valverde-Rebaza and Alneu de Andrade Lopes},
    title={RGCLI: Robust Graph that Considers Labeled Instances for Semi-Supervised Learning},
    journal={Neurocomputing},
    year={2016}
}
~~~~~

<div class="footer"> &copy; Copyright (C) 2016 Alan Valejo &lt;alanvalejo@gmail.com&gt; All rights reserved.</div>
