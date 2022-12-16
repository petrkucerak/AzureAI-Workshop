# Custom Vision

V tomto DEMU si ukážeme jak pracovat s Custom Vision. K tomu pouzijeme webovy portal, ktery s modelem komunikuje pomoci REST API. Nebude tedy treba vyuzit zadneho kodu.

## Vytvoření prostředků na Azure

1. portal.azure.com
2. nova skupina prostredku
3. nova sluzba Custom Vision
   - cenová úroveň trénování ***Free F0 (2 Transactions per second, 2 Projects)***
   - cenová úroveň predikce ***Free F0 (2 Transactions per second)***

## Práce v prostředí Custom Vision - Project

1. zalozeni projektu
   - classification detection - vrati jeden nebo vice stitku, popise, jake objekty jsou na obrazku
   - object detection - popise konkretni objekty i s jejich souradnicemi
2. otagovani obrazku (min 15 obrazku na tag)
3. spusteni cviceni modelu
   - **Probability Threshold** - Minimum probability score for a prediction to be valid when calculating precision and recall
   - **Overlap Threshold** - Minimum percentage of overlap between predicted bounding boxes and ground truth boxes to be considered a correct prediction
3. vysledky cviceni
   - Precision - This number will tell you: if a tag is predicted by your model, how likely is that to be right? ***spravnost predpovedi znacky mojim modelem***
   - Recall - This number will tell you: out of the tags which should be predicted correctly, what percentage did your model correctly find? ***jaky pocet znacek, ktere byly oznaceny, model opravdu nalezl***
   - mAP - Mean average precision means the overall object detector performance across all the tags ***uspesnost ve vsech tagach***
4. test uspesnosti
   - [hrib](https://www.muzeumcb.cz/wysiwyg_thumbs/3/276/Butyriboletus-regius-1982-09-17-JN-n-560x373.jpg)
   - [mochomurka](https://upload.wikimedia.org/wikipedia/commons/a/a8/M%C5%A1eno%2C_Deb%C5%99%2C_Muchom%C5%AFrka_s_popelnic%C3%AD.jpg)

## Reference

https://studuj.digital/2020/04/18/custom-vision-uvod/