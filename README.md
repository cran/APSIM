A package containing general purpose utility functions for loading and manipulating APSIM output and met files.

Release Notes
=============

### 0.9.3

-   TAV and AMP calculations have been incorrect (swapped)

### 0.9.2

-   loadApsim has new option: skipEmpty, which will skip output files with no data.
-   prepareMet now writes dates in AU format to handle Apsim 7.9 which can now read dates in addition to year/day

### 0.9.1

-   loadMet now allows met files to be streamed. Just pass it the complete url.
-   Updated loadMet documentation to point to metFile object description.

### 0.9.0

-   NEW: Added command to load APSIM Next Generation data files (GetApsimNGTable)
-   Optimised loadMet function; now loads much faster.
-   loadMet function now correctly reads constants in met files.

### 0.8.3

-   Multi-year met data that ends with an incomplete year is now processed correctly.
-   loadApsim now uses the current working directory if no directory is given.
-   Fixed bug where constants were including a leading space.
-   A vector of units is now required for prepareMet.

### 0.8.2

-   loadMet will now read existing constants.
-   metFile class has had a slot for constants added. Constants are a character vector of the format: variable=value.
-   prepareMet now correctly handles R Date formatted dates.

### 0.8.1

-   Fix for reading simulator output processed on a Condor cluster.

### 0.8.0

-   Initial Release.
