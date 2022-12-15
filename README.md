# investor-ranking-calculator

This tool needs is to determine if investors have enough of the financial resources to be a serious investor.  
The requirements identified include the following: Investors must have enough assets; Investors will
need to have low enough debt; Investors will need to have income to be a serious investor.  

totalAssets() - The totalAssets() function will not be passed any parameters. It
  will prompt the user for the number of assets that the user has (i.e. bank
  accounts, investment accounts, etc.) and will then use a "for" loop to prompt
  the user for the value of each of these assets and will keep a running 
  total of these assets.  The function will return the total value of all assets.
  The loop should continue for the amount of assets the user identifies.

totalDebt() - The totalDebt() function will not be passed any parameters.  Unlike
  the totalAssets() function, totalDebt() will not use a "for" loop.
  totalDebt() will use a while loop. totalDebt() will prompt the user for the value of 
  each debt the user has and will continue asking for the value of the next debt until
  the user enters a value of "0".  totalDebt() will keep a running total of debt and when
  the user enters a debt of "0" the function will return the total debt.

calculateInvestorRanking(investmentAmount, annualIncome, assets, debts) - calculateInvestorRanking()
is passed four parameters.  These four parameters are:
  investmentAmount - Represents the amount of the proposed investment.  For smaller
    investment, the investor will not need the same type of finanacial resources
    as for larger investments.  This has been provided in the main program.
  annualIncome -  Represents the annual income of the prospective investor. This
    has been provided in the main program.  
  assets - The total assets of the prospective investor.  This is returned by the 
    totalAssets() function.  
  debts - The total debts of the prospective investor.  This is returned by the 
     totalDebt() function.

Using these four pieces of information, calculateInvestorRanking will return an "investor 
score" based on the following rules:
1) If the prospective investor's debts are greater than their assets then the investor 
    score is 0 because this investor is clearly broke.
2) If the difference between the investor's assets and the investor's debts (assets-debts)  
    is less than the investment amount then the investor score is 0 because, while this investor 
    isn't broke, they clearly don't have the financial assets to make this kind of investment.
3) After subtracting debts and the proposed investment from assets, the investor   
    needs money to live on.  If the balance of their assets 
    (total assets - total debts - proposed investment) is greater than annual income, the investor score would 
    be (total assets - total debts - proposed investment).
    
