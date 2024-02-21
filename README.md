# investor-ranking-calculator

This tool needs is to determine if investors have enough of the financial resources to be a serious investor.  
The requirements identified include the following: Investors must have enough assets; Investors will
need to have low enough debt; Investors will need to have income to be a serious investor.  

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
    
