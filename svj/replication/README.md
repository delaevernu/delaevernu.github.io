Instructions
-----------

Prerequisites:
* https://git-scm.com/downloads   must be installed 
* If running on Windows, you must install the http://kdiff3.sourceforge.net/ tool on the root of C: (after installed, the path "C:/KDiff3/bin/diff3.exe" must exist)
* https://www.r-project.org/ must be installed, with the following packages (just copy and paste on R console):

	`install.packages('ggplot2', repos='http://cran.us.r-project.org');
	install.packages('reshape2', repos='http://cran.us.r-project.org');
	install.packages('beanplot', repos='http://cran.us.r-project.org');
	install.packages('xlsx', repos='http://cran.us.r-project.org');
	install.packages('coin', repos='http://cran.us.r-project.org');
	install.packages('scales', repos='http://cran.us.r-project.org'); 
	install.packages('knitr', repos='http://cran.us.r-project.org');
	install.packages('kableExtra', repos='http://cran.us.r-project.org');
	install.packages('DT', repos='http://cran.us.r-project.org');
	install.packages('tidyr', repos='http://cran.us.r-project.org');
	install.packages('effsize', repos='http://cran.us.r-project.org');
	install.packages('dplyr', repos='http://cran.us.r-project.org');`
* https://www.rstudio.com must be installed


After cloning this repository:
1. Install semistructured and structured merge with the command `java -jar mergetool-installer.jar`
2. Update the file "config.properties" accordingly with the path where the experiment will be executed
3. Update the file "projects.csv" if desired, each row contains the name of a project and its github url
4. Execute the command `java -jar experiment.jar`. Beware a single run can take several days
5. Open the script "statistics.Rmd" (you must update line 54 of this script) on RStudio installed on the prerequisites 
6. Run the script with `ctrl + shift + k`
6. Uninstall semistructured and structured merge with the uninstaller provided on the instalation folder you gave on step 1.

A HTML page "statistics.html" will be created summarizing the results. 