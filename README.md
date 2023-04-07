# SA-1B-Downloader
Simple script using GPT-4 to parallelize download and extract files for [SA-1B Dataset](https://ai.facebook.com/datasets/segment-anything/). 

## Requirements
* Python >= 3.6
* requests >= 2.0

Install with:
```
pip install requests
```

## Usage

The download.py script uses the [sa1b_links.txt](https://ai.facebook.com/datasets/segment-anything-downloads/) file by default as the input file for downloading and extracting images:

```
python download.py --processes 4 --input_file sa1b.txt --raw_dir raw --data_dir images
```

The download.py script takes the following command-line arguments:

    --processes: The number of processes to use for downloading and extracting files (default: 2)
    --input_file: The path to the input file containing file names and URLs (default: 'sa1b.txt')
    --raw_dir: The directory to store downloaded files (default: 'raw')
    --data_dir: The directory to store extracted files (default: 'images')
    
