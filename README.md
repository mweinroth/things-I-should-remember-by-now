# things-I-should-remember-by-now


_**Bold indicates parts of command that should be amended for specific use**_

## Shell

| Command purpose | Description | Source |
| --- | --- | --- |
| count number of files with specific extension in directory | find **/path/to/directory** -mindepth 1 -type f -name "**.csv**" -printf x \| wc -c | [source](https://askubuntu.com/questions/454564/count-total-number-of-files-in-particular-directory-with-specific-extension)|
| split larger file evenly | split --number=l/4 **input** | -- |
| delete column of csv | cut -d, -f**line.number** --complement **input.csv** > **output.csv** | [source](https://unix.stackexchange.com/questions/317366/remove-columns-from-a-csv-file) |
| add prefix to all files in directory | for f in * ; do mv "$f" **word**_"$f" ; done | [source](https://unix.stackexchange.com/questions/13147/rename-all-the-files-within-a-folder-with-prefix-unix) |


## Raw files 
| Command purpose | Description | Source |
| --- | --- | --- |
| add number to fasta header | awk '/^>/{$0=$0"_"(++i)}1' **file1.fasta** > **file1.numbered.fasta** | [source](https://www.biostars.org/p/227046/)|

