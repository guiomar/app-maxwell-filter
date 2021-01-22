# app-maxfilter

This is a draft of a future Brainlife App using [MNE MaxFilter](https://mne.tools/dev/generated/mne.preprocessing.maxwell_filter.html).

# app-maxfilter-documentation

1) Apply SSS or tSSS MaxFilter on MEG data 
2) Reduce environmental noise
3) Input files are:
    * a MEG file in `.fif` format,
    * an optional fine calibration file in `.dat`,
    * an optional crosstalk compensation file in `.fif`,
    * an optional head position file in `.pos`,
4) Ouput file is a `.fif` MEG file after Maxwell filtering 

### Authors
- [Aurore Bussalb](aurore.bussalb@icm-institute.org)
- [Maximilien Chaumon](maximilien.chaumon@icm-institute.org)

### Contributors
- [Aurore Bussalb](aurore.bussalb@icm-institute.org)
- [Maximilien Chaumon](maximilien.chaumon@icm-institute.org)

### Citations
1. Avesani, P., McPherson, B., Hayashi, S. et al. The open diffusion data derivatives, brain data upcycling via integrated publishing of derivatives and reproducible open cloud services. Sci Data 6, 69 (2019). [https://doi.org/10.1038/s41597-019-0073-y](https://doi.org/10.1038/s41597-019-0073-y)

## Running the App 

### On Brainlife.io

This App has not yet been registered in Brainlife.io.

### Running Locally (on your machine)

1. git clone this repo
2. Inside the cloned directory, create `config.json` with something like the following content with paths to your input files (see `config.json.example`)

```json
{
  "input": "rest1-raw.fif"
}
```

3. Launch the App by executing `main`

```bash
./main
```

## Output

The output file is a MEG file in `.fif` format.
