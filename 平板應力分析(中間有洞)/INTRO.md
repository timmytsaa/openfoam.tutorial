本專案會解釋如何在線性變形,穩態的物件進行應力分析的前處理,運作及後處理。平板的尺寸為:邊長4m;半徑R＝0.5m。負載為一均勻(uniform)應力$=10 kPa$，作用在物件左側及右側牆面。兩個對稱平面可以被視為同一物件，所以只需要解此物件的1/4區域，如下圖灰色區域。
![[Geometry of the plate with a hole.png]]
此物件可以視為二維物件，在笛卡爾座標系，我們可以根據第三個座標(即座標z)提出兩個假設:在平板應力情況下，忽略第三個座標;。根據這兩個假設，在平板應力情況下物件的厚度會非常薄;。

分析解法存在於負載無限大,薄平板(中間有洞)。解法為
$$(\sigma_{xx})_{x=0} = \begin{cases}\sigma (1+\frac{R^2}{2y^2}+\frac{3R^4}{2y^4})  & \mbox{for }\mid y\mid \ge\mbox{ R} \\ 0 & \mbox{for }\mid y\mid<\mbox{ R} \end{cases}$$
可以從模擬的解法與此解法做比較。使用者可以在結束此教學後研究網格的解法和網格加權;增加平板尺寸(不增加洞的尺寸)並計算分析解法與模擬解法的誤差。