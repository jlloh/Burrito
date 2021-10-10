# Introduction

A very simple util that parses the XML and corresponding C struct trail files (using nom) from Taco (GW2 overlay), to produce a json compatible format for [Burrito](https://github.com/AsherGlick/Burrito), a GW2 overlay for Linux.

Note that some sample files are included in `/data/` for unit testing.

## Example used

- Uses taco marker from [here](https://fast.farming-community.eu/open-world/solo-farming) as an example.
- Attempts to parse a `.trl` file which is a C struct generated by Taco, using `nom`.
- After that, attempts to marshal it into a json that's friendly to Burrito.

## Usage

```
let json_str = gw2_taco_parser::taco_to_json_str("folder_name", "abc.xml");
```