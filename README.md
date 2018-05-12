# Assesssing the Safety of a Drug

## Setup

Initial install:

    $ conda env create -f environment.yml
    $ source activate rosi_py

Update:

    $ conda env update -f environment.yml

Remove:

    $ conda remove -n rosi_py --all

## Exports

Export Jupyter notebook to LaTeX format:

    $ cd notebooks/
    $ jupyter nbconvert --to latex rosi_py.ipynb

Apply the following patch:

    --- rosi_py.tex
    +++ rosi_py.tex
    @@ -141,8 +141,9 @@
         \def\gt{>}
         \def\lt{<}
         % Document parameters
    -    \title{rosi\_py}
    -    
    +    \title{Assessing the Safety of Rosiglitazone\\
    +    for the Treatment of Type 2 Diabetes}
    +    \author{Konstantinos Vamvourellis}

Generate PDF export:

    $ pdflatex rosi_py.tex


## ToDo

* add comparison to treatment group?
* add conclusion
