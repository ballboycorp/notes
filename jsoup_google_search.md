# Jsoup and Google Search
## Location change
If you ever want to use Jsoup for Web scrapping google for a certain information, make sure that you use certain VPN
and relocate yourself to different location.
I was searching for simple query "*footballer name* + wikipedia" to get wikipedia urls of 500 footballers, since I am located
in South Korea, simple using
```
jsoup.connect(URL).get()
```
will sometimes get you to Korean version of the Google and you will have some exception as you were expecting 
> Adam Lallana - Wikipedia

instread you get the result in Korean. 
> 아담 랄라나 - 나무위키



## Don't bruteforce couple of times

For my case I was searching google for 500 footballers and since I might have gotten some exception, I used to fix and redo.
But this approaches will get you Google detect your IP to have unusual behavior and will block you for couple of hours.
So don't re-run couple of times at the same time.
