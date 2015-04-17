# Philips Reader Node Changelog

## 2 (c9bfb)
* Fixed bug that caused ky-chop to fail on RAW/LAB/SIN
* Fixed extension case for case sensitive file systems

## 1 (5b5e0)
* Fixed bug that caused ReadCpx to fail in some cases.
* Speed up switching between coils by bypassing file reading each time.
* Fix possible bug for lab/raw/sin reading when raw data corrections aren't applied.
