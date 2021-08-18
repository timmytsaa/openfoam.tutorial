要啟用流線圖示，要在`Pipeline  Browser`找到`Stream Tracer`並按下`Apply`，即可在`Properties`調整設定。
![[Properties panel for the Stream Tracer filter.png]]

`Seed`可以調整散布圖的樣式。將`Seed`設定為`High Resolution Line Source`並且在物件中間垂直計算數值。如從(0.05, 0, 0.005)到(0.05, 0.1, 0.005)

在上圖的設定有以下：計算點(Resolution)為21;最大分階長度(Maximum Step Length)0.5;初始分階長度(Initial Step Length)0.2;還有整合方向(Integration Direction)BOTH[^1]。設定完成後按下`Apply`

若要生成圖像，在`Filter`選擇`Tube`。此設定為：邊界數量(Num. sides)為6;半徑(Radius)0.0003;半徑因素(Radius factor)10;並把色階應用為速度。設定完成後按下`Apply`

[^1]:Runge-Kutta 4/5 IntegratorType為初始設定