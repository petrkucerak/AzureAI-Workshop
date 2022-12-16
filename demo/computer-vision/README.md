# Computer Vision

V tomto DEMU si ukážeme jak vytvořit službu Computer Vision na cloudové platformě Microsoft Azure pomocí Azure portálu.

Se službou budeme komunikovat pomocí rozhrání API a nechat ji vytahnout text z  obrazku (OCR).

## Vytvoření prostředků na Azure

1. portal.azure.com
2. nova skupina prostredku
3. nova sluzba *Pocitacove zpracovani obrazu* (Computer Vision)
   - cenova uroven ***Free F0 (20 Calls per minute, 5K Calls per month)***

## Připravení skriptu

1. nainstalujte si knihovny do pythonu
   ```sh
   # Instalace knihovny pro klienta
   pip install --upgrade azure-cognitiveservices-vision-computervision

   # PIL is the Python Imaging Library by Fredrik Lundh and Contributor. More infromation: https://pillow.readthedocs.io/en/stable/
   pip install pillow
   ```
2. nastav si klic a endpoint
3. vloz url adresu k obrazku, ktery chces analyzovat
4. spust soubor
   ```sh
   python.exe .\computer-vision.py # pouze pro moje PC
   ```
## Reference

https://studuj.digital/2020/05/17/podobne-obrazky/
https://learn.microsoft.com/cs-cz/azure/cognitive-services/Computer-vision/quickstarts-sdk/client-library?pivots=programming-language-python&tabs=visual-studio