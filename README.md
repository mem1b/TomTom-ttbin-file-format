#_DEPRECATED_
Due to my employer's intellectual property policy I can't work on this project anymore. I recommend forking it if you would like updates.

---

My guesses so far about the .ttbin file format generated by the TomTom cardio GPS watches.


Notes:
------
0. The file format is a repetition of 1 byte tags followed by N bytes of data with N depending on the tag value.
1. The GPS coordinates are a bit different from what the TomTom software extracts as it seems to smooth the data.
2. A BPM of zero means that the was no reading, the TomTom software tends to use and old value instead.
3. The meaning of some tags and parts of the data is still unknown.

To compile:
-----------
gcc -std=c99 ttbin.c
