
# Rapport

**Skriv din rapport här!**


I den här dugga skulle man följa olika steg för att kunna öva sig på hur man gör/bygger en webview och lägga
till olika länkar som en extern sida respektive intern sida. För att lösa den första med webview va man tvungen att radera den
befintliga textview till en typ av Webview, detta har man gjort i filen med namnet content_main.xml. Koden för webview kan man se nedan i kod blocket där en id
tillförs för att kunna återanvända detta i de framöver processen. I MainActivity håller man med att lägga en private member och sedan återanvänder detta längre ner under
Oncreate och sedan använda detta för att kunna ladda upp de externa och interna sidorna som ligger som krav i duggan. Resultatet på den externa och interna sidorna kan man
se längre ner under figur 1 och 2. Dessa sidor har man kunnat anropa
längre ner under de olika if-satser då vi har två olika metoder och kalla på sidor, detta har man löst med hjälp
av en anrop av funktionen med namnet showExternalWebPage() och showInternalWebPage().

Programkod ska se ut som exemplet nedan. Koden måste vara korrekt indenterad då den blir lättare att läsa vilket gör det lättare att hitta syntaktiska fel.

```
<WebView
        android:id="@+id/my_webView"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_marginTop="50dp"
        />

        //noinspection SimplifiableIfStatement
                if (id == R.id.action_external_web) {
                    Log.d("==>","Will display external web page");
                    showExternalWebPage();
                    return true;
                }

                if (id == R.id.action_internal_web) {
                    Log.d("==>","Will display internal web page");
                    showInternalWebPage();
                    return true;
                }
```

Bilder läggs i samma mapp som markdown-filen.

![](Figur1.png)
![](Figur2.png)

Läs gärna:

- Boulos, M.N.K., Warren, J., Gong, J. & Yue, P. (2010) Web GIS in practice VIII: HTML5 and the canvas element for interactive online mapping. International journal of health geographics 9, 14. Shin, Y. &
- Wunsche, B.C. (2013) A smartphone-based golf simulation exercise game for supporting arthritis patients. 2013 28th International Conference of Image and Vision Computing New Zealand (IVCNZ), IEEE, pp. 459–464.
- Wohlin, C., Runeson, P., Höst, M., Ohlsson, M.C., Regnell, B., Wesslén, A. (2012) Experimentation in Software Engineering, Berlin, Heidelberg: Springer Berlin Heidelberg.
