原專案到現在雷諾數都是10，這是一個非常低的數值而且很快就會達到穩態[^1]。我們現在把雷諾數提升到100，這會大大增加達到穩定的時間。我們使用原專案cavity為範例，複製cavity專案並重新命名為cavityHighRe。除了直接複製，也可以使用`foamCloneCase`，不過它只會把時間路徑(time directory)裡的0複製過去。使用`-latestTime`複製最後的時間，即0.5[^2]。本次也使用精簡語法`run`進入`run`路徑
```
run
foamCloneCase -latestTime cavity cavityHighRe
cd cavityHighRe
```


[^1]:只有小型的漩渦(small secondary vortices)在底部的邊腳產生。
[^2]:這個數據將會成為此專案的初始狀態。