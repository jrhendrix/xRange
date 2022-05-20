# xRange
Extract a segment of characters from a DNA sequence file. The user can define the exact positions of the range or provide a single position and specify the number of bases upstream or downstream.
Eventually there will be functionality to extract the first or last bases from a contig.

## Usage
There are three ways to specify the range of sequence to extract: defined coordinates, add from position, and subtract from position
### Defined coordinates
```
# Use defined coordinates to extract first 10 bases
python xRange.py define -f file.fasta --start 1 --stop 10

# Output sequence to file fist.fasta
python xRange.py define -f file.fasta --start 1 --stop 10 -s first

# Set read ID
python xRange.py define -f file.fasta --start 1 --stop 10 -s first --outID myID
```

### Add to position


### Subtract from position
```
# Extract positions 1 through 4
python xRange.py subtract -f tmp.fa --stop 4 --sub 2
```
