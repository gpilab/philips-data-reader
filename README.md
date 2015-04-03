# Philips Raw Data Reader Node
This project hosts the Philips raw data reader node for GPI in binary form for
easy access.

## Description
A module for reading in Philips MR Scanner data.
Current supported formats include: .data, .list, .lab, .raw, .sin, .par, .xml,
.rec, and .cpx.

### OUTPUTS

| data | MR data from file |
| noise | noise measurement data |
| phc | phase data for EPI correction |
| user_parms | scan information written to .txt file - requires appropriate addition to methods code |
| header | information from Philips header files (.list, .sin, .lab, .par, .xml) |

### WIDGETS
I/O Info - Gives info on selected file, data type, data dimensionality and
    dimension labels.
File Browser - button to launch file browswer, and typein widget if the pathway
    is known.
data/list only options:
    ky chop - turns on/off ky chopping (multiplying data in even-numbered
        Y phase encodings by -1)
    kz chop - turns on/off kz chopping (multiplying data in even-numbered
        Z phase encodings by -1)
    PROPELLER TSE - select when reading PROPELLER TSE data sets
    PROPELLER GRASE - select when reading PROPELLER GRASE data sets
Re-scale Type: - used for par/rec files only
    FP = floating point
    DV = display value
    SV = stored value
Apply Corrections: - applies the following raw data corrections
    (lab/raw/sin only)
    Profile dependent amplification
    Random phase
    Measurement phase
    Not performed:
    DC offset correction
Execution Type - indicates if this is module is run as thread, process,
    or apploop
Read Param Only - set to read header only


