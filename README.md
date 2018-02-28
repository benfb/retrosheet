# retrosheet
Import Retrosheet data as a structured R object

`retrosheet` is an R package that downloads and parses the single-season event, gamelog, roster, and schedule
files from http://www.retrosheet.org into structured R objects for further analysis.

Currently, the main functions are
 - `getRetrosheet()` - This workhorse function returns the full seasonal data associated with the user-entered 
 arguments
 - `getPartialGamelog()` - An alternative to returning the full gamelog files.  This function allows the user
 to choose the columns and date. Column names are made available by the global object `gamelogFields`
 
Also included are convenience functions 
 - `getFileNames()` - for obtaining a list of all zip files currently available for use by this package
 - `getTeamIDs()` - for providing the team ID value to be used in the `team` argument of `getRetrosheet()`
 - `getParkIDs()` - for ballpark ID and name information
	
This development version can be installed with 

	install.packages("devtools")
	devtools::install_github( repo = "keberwein/retrosheet" )
	
# Note About Retrosheet

Recipients of Retrosheet data are free to make any desired use of the information, including (but not limited to) selling it, giving it away, or producing a commercial product based upon the data. Retrosheet has one requirement for any such transfer of data or product evelopment, which is that the following statement must appear prominently:

> The information used here was obtained free of charge from and is copyrighted by [Retrosheet](http://www.retrosheet.org/).  Interested parties may contact Retrosheet at 20 Sunset Rd., Newark, DE 19711.
	
*Last updated on February 28, 2018*
