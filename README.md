# TradeAnalysis_Releases

This repository is for the purposes of distributing binaries (Windows 10 .EXE and .DLLs) for my "TradeAnalysis" report maintained in the Superalgos project. You can see the releases in the column to the right of this README.

The source code and further information can be accessed here:

https://github.com/BigGremlin/Superalgos/tree/develop/Reports/RnD/TradeAnalysis

```
Usage:
  TradeAnalysis filename.csv BTC_Ballance USDT_Ballance -s

  -s To print summary only
```

Walkthrough:
1. Get a copy of the Binance Order History Export <br> Home -> Orders -> Spot Order -> Order History -> Export
<br>Most of the time you will want to use custom dates via the "Within 6 months - Custom" option.
<br>After pressing the "Export Button" you will get an *.XLSX file 
2. Load the .XLSX file into Excel and do a "Save As" with the type "CSV (MS-DOS)" selected. (I'm sure there's a helper program for this somewhere on the internet to do this via a command line)
3. Now you can run the report program (from the command line of course).
4. It will generate the report as either a daily summary or a trade by trade detailed report. You specify which one you want by using the '-s' flag.
5. You will also need to enter your wallet ballance at the starting date for your date range for BTC and USDT.
6. The program at the moment outputs the report to standard out. You can redirect this to a .CSV file with the redirection symbol '>'
7. You can then load these report into Excel for further decorating like setting the Title cells to wrap and USDT cells to Currency ($).

Supplied test files and where they are used in the above bullet points:

1. "Export Order History-2022-12-26 12_30_35.xlsx"
2. "Export Order History-2022-12-26 12_30_35.csv"
6. "Export Order History Processed Summary-2022-12-24-01.csv" OR "Export Order History Processed-2022-12-24-02.csv"
7. "Export Order History Processed Summary-2022-12-24-01.xlsx" OR "Export Order History Processed-2022-12-24-02.xlsx"
