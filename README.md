# SerialMerge

serialmerge.py implements the SerialMerge algorithm for merging HKL files using rank aggregation.

## Usage

    python serialmerge.py arg1 [arg2 ...]

Arguments can be a filename (i.e. `data.hkl`), a directory, or any combination.
In case a directory is given, SerialMerge will load all the hkl files in that directory.
hkl files should be in free format (space separated) with 5 columns: `h k l I/F esd`

Example:

    python serialmerge.py ssz45_data/

## Dependencies

 - [Python 3.9 or newer](https://www.python.org/)
 - [Numpy](http://www.numpy.org/) (tested with 1.25.2)
 - [Pandas](http://pandas.pydata.org/) (tested with 2.1.0)
 
## Other

 - [CrystDiff](https://github.com/stefsmeets/serialmerge/releases/tag/crystdiff), a program for simulating electron diffraction patterns (developed by Wei Wan)
 - [Simulated data on SSZ-45, SSZ-53, SSZ-55, SSZ-56, SSZ-58, SSZ-59](https://github.com/stefsmeets/serialmerge/releases/tag/data)

## Reference

For more information, see [S. Smeets & W. Wan, J. Appl. Cryst. (2017). 50, 885-892 ](https://doi.org/10.1107/S1600576717005854)

## Credits

Implementation is based on the SerialRank algorithm:

 - <http://arxiv.org/abs/1406.5370>
 - <http://www.di.ens.fr/~fogel/SerialRank/tutorial.html>

