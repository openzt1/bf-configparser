# bf-configparser

> [!IMPORTANT]  
> Moved to [OpenZT Workspace](https://github.com/openzt1/openzt/tree/main/openzt-configparser)

This is a Rust library for parsing and writing configuration files based on `INI` like file formats used in [Zoo Tycoon (2001)](https://en.wikipedia.org/wiki/Zoo_Tycoon_(2001_video_game)). 

It is forked from [configparser-rs](https://github.com/QEDK/configparser-rs), the main differences are:
 - Duplicate keys create a list of values instead of overwriting the previous value
 - Breaks api compatibility with Python's configparser, `getbool()` and other non-snake case functions are removed
 - Adds `get_vec()` function to get a vector of values
 - Adds generic `get_parse()` and `get_vec_parse` functions, replacing all `get*()` functions
