編譯與執行:
	python3 hw3.py
執行成功後，輸入要input的檔名:
	Input file name: readfile.txt
輸出結果在output.txt及city result.png

此程式之演算法為SA
程式流程為:
先製作一個放入所有城市的list，前後都是原點
接著隨機交換兩個城市，除了原點
如果路徑長更短則儲存，路徑長更長則依熱力學公式:
P(dE) = exp(dE/(kT))與一隨機0~1比較大小
使其可能接受較差解
程式越執行到後期，會因為降溫而使其接受較差解的可能性越來越低
最後降溫到一定的值後 輸出結果