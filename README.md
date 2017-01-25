# SerialMerge

serialmerge.py implements the SerialMerge algorithm for merging HKL files using rank aggregation.

## Usage

    python serialmerge.py arg1 [arg2 ...]

Arguments can be a filename (i.e. data.hkl), a directory, or any combination.
In case a directory is given, SerialMerge will load all the hkl files in that directory.
hkl files should be in free format (space separated) with 5 columns: `h k l I/F esd`

Example:

    python serialmerge.py ssz45_data

## Dependencies

 - [Python2.7 or Python3.6](https://www.python.org/)
 - [Numpy](http://www.numpy.org/) (tested with 1.11.3)
 - [Pandas](http://pandas.pydata.org/) (tested with 0.19.3)

## Credits

Implementation is based on the SerialRank algorithm:

 - <http://arxiv.org/abs/1406.5370>
 - <http://www.di.ens.fr/~fogel/SerialRank/tutorial.html>

