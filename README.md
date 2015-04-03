# Philips Raw Data Reader Node
This project hosts the Philips raw data reader node for GPI in binary form for
easy access.

## Description
A module for reading in Philips MR Scanner data.
Current supported formats include: .data, .list, .lab, .raw, .sin, .par, .xml,
.rec, and .cpx.

### OUTPUTS

|Port Name|Description|
|---|---|
| data | MR data from file |
| noise | noise measurement data |
| phc | phase data for EPI correction |
| user_parms | scan information written to .txt file - requires appropriate addition to methods code |
| header | information from Philips header files (.list, .sin, .lab, .par, .xml) |

### WIDGETS

|Widget Name|Description|
|---|---|
|I/O Info| Gives info on selected file, data type, data dimensionality and dimension labels|
|File Browser| button to launch file browswer, and typein widget if the pathway is known|
|Execution Type| indicates if this is module is run as thread, process, or apploop|
|Read Param Only| set to read header only|

#### data/list Options
|Widget Name|Description|
|---|---|
|ky chop | turns on/off ky chopping (multiplying data in even-numbered Y phase encodings by -1)|
|kz chop | turns on/off kz chopping (multiplying data in even-numbered Z phase encodings by -1)|
|PROPELLER TSE | select when reading PROPELLER TSE data sets|
|PROPELLER GRASE | select when reading PROPELLER GRASE data sets|

#### par/rec Options
|Re-scale Type|Description|
|---|---|
|FP | floating point|
|DV | display value|
|SV | stored value|

#### lab/raw/sin Options
|Apply Corrections|
|---|
|Profile dependent amplification|
|Random phase|
|Measurement phase|
|DC offset correction|

## Installation
Download the latest release corresponding to your platform (Linux or OSX) to
your `~/gpi` directory (or a directory that is in your `.gpirc`: `LIB_PATH`)
unzip and restart GPI.
