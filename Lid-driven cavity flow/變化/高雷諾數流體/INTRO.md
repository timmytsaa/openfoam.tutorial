做完[[Lid-driven cavity flow/變化/增加雷諾數/INTRO|增加雷諾數]]並觀看速度向量場，可以看到底部的漩渦尺寸增加。使用者可以藉由減少黏滯係數來增加雷諾數，觀看漩渦會如何變化。漩渦的數量逐漸增加，為了要處理更複雜的流體，要在漩渦處增加解法數(mesh resolution)。此外，增加雷諾數會導致計算的收斂時間增加。我們可以增加或減少`endTime`確保專案已收斂。

不過當流體為紊流時，單純增加解法就便得不切實際，因為會導致穩定度下降。為了要解決這種高雷諾數的問題，Reynolds-averaged simulation(RAS)紊流模型是為計算平均流量表現及統計波動起伏。$k - \epsilon$模型[^1]將會應用在本次專案並計算雷諾數為$10^4$的lid-driven cavity專案。有==兩個變數==需要計算：$k$[^2]和$\epsilon$[^3]。其他與紊流相關的方程式及模型在[[pisoFoam]]可以參考。

[^1]:with wall functions
[^2]:紊流動能the turbulent kinetic energy
[^3]:紊流耗損率the turbulent dissipation rate