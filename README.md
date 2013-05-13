# ge-data

A tool to extract Malaysia's general election data from Election Commission (EC)/Suruhanjaya Pilihan Raya (SPR)
website. It converts website data in HTML to structured JSON data that can be easily processed by machines.

## Requirements

- Gradle

## Usage

To take a snapshot of current election data from SPR's website:

    gradle takeSnapshot

This will generate a directory called `ge-13/data-yyyyMMdd-HHmmss` with the following structure:

    |____html
    | |____party-list.html
    | |____results
    | | |____*.html
    | |____seats
    | |____*.html
    |____logo
    | |____*.png
    |____party-list.json
    |____seats-result.json
    |____seats.json
    |____state-list.json

It generates a number of files:

- html/** represents the source files from SPR site that was used to extract data. Use this to cross check accuracy of
data extraction (and report bugs or better, submit a pull request).

- logo/** represents logo for each party.

- *.json represents the structured data that was extracted.

## Why?

TODO: get permission to use words from http://www.opengovdata.org/home/8principles/annotations

## Feedback

* Need help using this tool?
* Found a problem/bug with this tool?

kctang via twitter.