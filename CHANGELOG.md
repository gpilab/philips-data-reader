# Philips Reader Node Changelog

## 5 (aa8d3)
* added support for spiral.txt reading with raw/lab/sin
* fixed bug in xml reading that caused issues with raw/lab/sin
* fixed integer division error
* fixed xml issue when reading certain sequence types
* fixed bugs related to reading multiple echoes of different lengths

## 4
* Fixes ky-chop and case sensitive filenames.

## 3 Python Pre-release
* Updated to Python 3

## 2 (c9bfb)
* Fixed bug that caused ky-chop to fail on RAW/LAB/SIN
* Fixed extension case for case sensitive file systems

## 1 (5b5e0)
* Fixed bug that caused ReadCpx to fail in some cases.
* Speed up switching between coils by bypassing file reading each time.
* Fix possible bug for lab/raw/sin reading when raw data corrections aren't applied.
