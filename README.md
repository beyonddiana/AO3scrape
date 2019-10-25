# AO3scrape

Command-line tool for scraping and exporting fandom numbers from AO3.

## Usage

Run via the console. Open *cmd.exe*, navigate to the folder you saved *AO3scrape.exe* in, and run the file with any desired flags. Example: `C:\Users\example\Desktop>AO3scrape.exe -tag "Harry Potter - J. K. Rowling" -min 5000 -max 25000 -search "&work_search[query]=- Dramione"`

**-h, -help:**
Displays the help text, overruling any other flags.

**-tag [string]**
Sets the tag to search. Required, omitting this flag will fail the process and shut down the software.

**-min [int]**
Sets the minimum word count filter. Negative values equal not setting the flag.

**-max [int]**
Sets the maximum word count filter. Negative values equal not setting the flag. Large numbers will be capped at 5,000,000.

**-search [string]**
Allows adding custom search parameters to the search results URL used internally, such as *&work_search[query]=-"High School AU"*

**-simple**
Replaces the usual "there are x works" output with a numbers-only version listing minimum and maximum word count and number of fics, separated by tabulators and fit for import into spreadsheet software.
