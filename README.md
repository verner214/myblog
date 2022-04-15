#--------- enkelt cms --------- 
Bloggen kan köras lokalt på disk. I edge funkar då inte att index.html automatiskt visas utan man får dubbelklicka.
Kommandon: build.bat  
##Så här ser build.bat ut inuti:
copy header1.html + .\blog1\blghead.html + header2.html + .\blog1\blgbody.html + footer.html .\blog1\index.html  
copy header1.html + .\blog2\blghead.html + header2.html + .\blog2\blgbody.html + footer.html .\blog2\index.html  

###Kommentar
copy src1 + src2 dest -- är legal DOS. concats src1 och src2 till dest.
* Hela bloggen byggs alltså på nytt varje gång build.bat körs.

###Filer
* header1.html -- innanför head-taggen. stylesheet och javascript, det mesta är wordpress.
* blghead.html -- titel och metataggar. hamnar innanför head.
* header2.html -- body och nedåt. Övre delen av sajtstrukturen.
* blgbody.html -- detta är bloggen.
* footer.html -- sidomeny och highlightkod.

##Ny blogpost
* gör blghead och blgbody
* lägg till menylänk i footer.html
* bygg mha build
* checka in till github (har väl inte kopplat github->AWS?)
* ladda upp till AWS manuellt(?)

#--------- filer ------------  
/blog1/body.html  
/blog1/localimage1.jpg  
/blog1/localimage2.jpg  
/blog2/etc.  
/images/  
/js/  
/css/  
header.html  
footer.html  
about.html  
404.html  
  
#--------------- output, laddas upp till molnet -------------  
/src/blog1/index.html -- .gitignore  
/src/blog2/index.html -- etc.  
  
  
  
#my useful commands  
se https://gnaget.z16.web.core.windows.net/view/index.html?id=59c9e7a1-93af-4ff0-a172-7658e695c3f9
eller sök git i wiki.
