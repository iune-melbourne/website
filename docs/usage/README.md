# Running the Program

## Input File Format

Melbourne processes Excel spreadsheets that are structured in a specific format, which we will discuss below. 

The first row in the file is known as the *header row*, and contains the column labels for each column in the file. This row is required in the input file format for Melbourne. In addition, the following columns are required, and must be present in the input file for it to be properly loaded by the program:

1. **Entry Draw/Placing:** The first column can be used to show the draw or placing of the entries. This column can be thought of as a “helper” column, as the program does not actually read the values in this column — I often fill out this column in order to make it easier to see the entry rankings.
2. **Entry User/Country:** The second column is used to put information about who the entry comes from. Usually, this is the user who sent the entry, or the country who sent the entry if you are generating scoreboards for a contest with countries instead of users.
3. **Flag Details:** The third column is used to put information about the flag to use for the entry. If you don’t want to use flags in the scoreboards, you can leave this column blank. See below for more details on flags.
4. **Entry Artist:** The fourth column is used to put information about the entry's artist.
5. **Entry Song:** The fifth column is used to put information about the entry's song title.
6. **Entry Points:** The sixth column is used as another helper column which is not actually read by Melbourne. This column is used to store the total number of points the entry received, and like the first column can be left blank.
7. **Votes:** After the six required columns come the various voter columns. Put the name of the voter in the first row (the header row), and the points the voter gave to each of the entries in the appropriate row for the entry.
    - When filling out the voter columns, if you wish to disqualify an entry, simply put `DQ` in the row for that entry. The entry will then be sorted after all non-disqualified entries in scoreboard for that voter, as well as any remaining scoreboards.

**Notes:** 
* While the helper columns mentioned above do not necessarily need to be filled out, they *must* still be present in the input file for it to be properly loaded by the program.
* Make sure that there is no extraneous text in any cells in any row after the last entry's row. If there is, there is a possibility that this may be misinterpreted by the program as an additional “entry”, which may result in errors or strange output in the scoreboard.

### Flags

By default, there are three set of flags: `ISC`, `World`, and `Rect`. To use flags from each of these folders, simply use the format `<flag set>/<flag filename>` in the Excel spreadsheet (ex: `ISC/Kaledonii.png` or `World/ee.png`).

* **ISC** is the set of flags available for countries in the Internatia Song Contest on [escforum.net](http://escforum.net).
* **World** is a set of square flags available for real-world countries. Each country's flag is saved with its two letter ISO code in lowercase.
* **Rect** is a set of rectangular flags available for real-world countries. Similar to `World`, each country's flag is saved with its two letter ISO code in lowercase.
* Notes:
  - For both `World` and `Rect`, the flag for Serbia & Montenegro is available at `serbiamontenegro.png` — the country's ISO code was `yu` which would otherwise result in a naming conflict with the flag of Yugoslavia.
  - The flag of Kosovo is available at `xk.png`, following convention set by several international organizations such as the European Commission. Kosovo does not yet have an official ISO code as set by the International Organization for Standardization.

To see the list of available flags, as well as how to add custom flags for use in the scoreboards, see [Customization](https://github.com/Iune/melbourne/wiki/Customization).

### Example File
Below, you can see a screenshot of the spreadsheet I used to generate scoreboards using the Eurovision 1988 results. You can download this spreadsheet [here](https://github.com/Iune/melbourne/raw/master/resources/1988.xlsx).

![Screenshot of an example Excel spreadsheet](/sample_spreadsheet.png)

## Running the Program

![Screenshot of Melbourne](/screenshot.png)

1. Select the input file by pressing the `Input File` button or by typing `Ctrl + O` (`⌘ + O` on macOS).
    - If the contents of the input file are updated after it has been selected in *Melbourne*, you will need to refresh the program. To do this, you can either press the reload button next to the `Input File` button or type `Ctrl + R` (`⌘ + R` on macOS).
2. Select the directory to save the generated scoreboards by pressing the `Output Folder` button or by typing `Ctrl + Shift + O` (`⌘ + Shift + O` on macOS).
3. Fill out the scoreboards' title in the appropriate input file. `Results` is automatically appended to the input provided here, so it does not need to be included. (ex: `Eurovision 1988` is displayed in the scoreboards as `Eurovision 1988 Results`)
4. Set the main and accent colors using the `Main Color` and `Accent Color` buttons respectively. If you wish to go back to the default value, simply press the corresponding `Reset` button.
5. If you wish to display flags on the scoreboards, toggle `Display Flags`.
    - The program will first check to make sure that all of the flags specified in the input file are present in the `flags/` resource folder. If there are missing flags, they will be displayed in a pop-up message — these missing flags will need to be addressed if you wish to generate scoreboards with flags (scoreboards without flags can still be generated in the mean time). If the input file was updated to address the missing flags, don't forget to reload the file.
    - In addition, there is a toggle to `Display Borders Around Flags`. Disabling this can be helpful when using non-square or non-rectangular custom flags (ex: circular flags), as the program would otherwise draw borders around the rectangular images as loaded from file.
6. Once the input file, output folder and scoreboard title have been specified, the `Generate` button will become selectable. Press the button when you are ready to generate your scoreboards.
    - The program will now begin to generate scoreboards. If you wish to cancel the process while it is running, press the `Cancel` button.
    - While generation times will vary depending on your computer, I find that generating roughly 30-40 scoreboards usually takes less than 30 seconds.