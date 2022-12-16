# Text to Speech

V tomto DEMU si ukážeme jak vytvořit Speech Services na Azure pomocí Azure portálu, jak prevest clanek na podcast a jak pracovat se studiem.

## Vytvoření prostředků na Azure

1. portal.azure.com
2. nova skupina prostredku
3. nova sluzba *Řeč* (Speech services)
   - cenova uroven ***Free F0***

## Připravení skriptu

1. nainstalujte si knihovny do pythonu
   ```sh
   yarn # nainstaluje potrebne balicky
   ```
2. spust skript s pozadovanymi paramtery
   ```sh
   yarn node -e 'require(\"./text2speech\").text2speech()' <API-KEY> <location> <filename>
   ```

## Online prostredi

*Prace pomoci weboveho portalu komunikujicim s modelem pres API.*

https://speech.microsoft.com/

## Reference

https://blog.petrkucerak.cz/post/Jak-z-blogu-vytvorit-podcast-pomoci-AI