# TradeAnalysis_Releases

This repository is for the purposes of distributing binaries for my "TradeAnalysis" report maintained in the Superalgos project.

The source code and further instructions can be accessed here:

https://github.com/BigGremlin/Superalgos/tree/develop/Reports/RnD/TradeAnalysis

```
Usage:
  TradeAnalysis filename.csv BTC_Ballance USDT_Ballance -s

  -s To print summary only
```

Walkthrough:
1. Get a copy of the Binance Order History Export

Home -> Orders -> Spot Order -> Order History -> Export

Most of the time you will want to use custom dates via the "Within 6 months - Custom" option.

After pressing the "Export Button" you will get a *.XLSX file 

2. Load the .XLSX file into Excel and do a "Save As" with the type "CSV (MS-DOS)" selected.
3. Now you can run the report program (from the command line of course).
4. It will generate the report as either a daily summary or a trade by trade detailed report. You specify which one you want by using the '-s' flag.
5. You will also need to enter your wallet ballance for BTC and USDT.
6. The program at the moment outputs the 
