# Computer Vision

V tomto DEMU si ukážeme jak vytvořit službu Computer Vision na cloudové platformě Microsoft Azure pomocí Azure portálu.

Se službou budeme komunikovat pomocí rozhrání API a nechat ji popisovat obrázky.

## Vytvoření prostředků na Azure

1. portal.azure.com
2. nova skupina prostredku
3. nova sluzba *Pocitacove zpracovani obrazu* (Computer Vision)
   - cenova uroven ***Free F0 (20 Calls per minute, 5K Calls per month)***

## Připravení skriptu

1. nainstalujte si knihovny do pythonu
   ```sh
   pip install --upgrade azure-cognitiveservices-vision-computervision
   pip install pillow
   ```

## Reference

https://learn.microsoft.com/cs-cz/azure/cognitive-services/Computer-vision/quickstarts-sdk/client-library?pivots=programming-language-python&tabs=visual-studio