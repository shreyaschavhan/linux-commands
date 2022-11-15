# &#10023; Useful Linux Commands or Scripts 

> Keeping these things here so that it will be less difficult for me to search them AGAIN
---

* Remove anyline with given keyword in a file
> * Ex. ```sed -i '/keyword/d' myfile.txt``` 
> * Ex. ```sed '/google\.com/d; /google\.co.in/d; /googleusercontent\.com/d' -i file.txt``` 
> 
> ### Input file:
> ```
> https://support.google.com/websearch/answer/181196?hl=en-IN
> https://www.google.co.in/intl/en/about/products?tab=whBXoECAEQJQ
> https://www.google.com/search?q=inurl+/bug+bounty&rlz=1C1CHBD_enIN893IN893&biw=1536&bih=760&sxsrf=ALeKk01Ochq8i5aFWr340A0D7JKJKSCmQw:1620815953854&source=lnt&tbs=li:1&sa=X&ved=2ahUKEwjQs7P5-cPwAhVrzTgGHbbRAfs4UBCnBXoECAEQLA
> https://simwood.com/uk/bug-bounty
> https://webcache.googleusercontent.com/search?q=cache:g5NSs9KCD68J:https://simwood.com/uk/bug-bounty+&cd=81&hl=en&ct=clnk&gl=in
> https://firebounty.com/
> https://support.google.com/websearch/?p=ws_results_help&hl=en-IN&fg=1
> https://policies.google.com/privacy?hl=en-IN&fg=1
> https://policies.google.com/terms?hl=en-IN&fg=1
> ```
> * C: ```sed '/google\.com/d; /google\.co.in/d; /googleusercontent\.com/d' -i file.txt``` 
> ### Output File:
> ```
> https://simwood.com/uk/bug-bounty
> https://firebounty.com/
> ```

---

* Remove duplicate lines from a file
> ```awk '!seen[$0]++' filename``` 


----

- Dalfox:
```
dalfox file brute.txt --output-all dalfox.txt --only-discovery --skip-bav --skip-mining-all -w 500 --report
```
