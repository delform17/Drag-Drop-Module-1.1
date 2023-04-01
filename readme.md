# Title of Project : 
**Drag and Drop witch Data Filter**

# Description :
**Niniejsze repozystorium zawiera skrypt popularnego narzędzia jakim jest przenieś i upuść wraz z opcją filtrowania plików względem rozszerzenia. Pliki wczytywać możemy poprzez przeciąganie ich w odpowiedni obszar oraz przy pomocy przycisku. 
Po wybraniu odpowiednich plików wyświetla nam się lista z plikami które zostały zaakceptowane przez skypt. Obrazy wyświetlanie sa w formie miniaturek z minimalnym opisem natomiat przy innych dokumentach wyświetla nam się wyłącznie ikonka oznaczająca rozszerzenie pliku. Skrypt posiada przystępna oraz przejrzystą grafikę w oparciu o III gen styli CSS.**

# How to run : 
**Pliki po pobraniu należy pobrać i zapisać na dowolnym serwerze www np Apache.**

## Skrypt bazuje przede wszystkim na filtrowaniu, kontroli wagi oraz typu plikow 
``` 
function checkSizeAndDisplay(fileObject)
{
    const type_of_files = file => file.type == "text/plain" || file.type == "application/msword" || file.type == "image/jpeg";
    
    if(sumOfSize < 2000000)  // 2MB 
    {
      Array.from(fileObject).filter(type_of_files).forEach(f => 
      {
        filterSettings(f);
        
      });
    }else{
      alert("To many files loaded"); 
      }
}
```

## Będziemy filtrować również dokumenty typu ,,doc"
``` 
if(f.type ===  "application/msword")
    {
          var picture = new Image(70,140);
          picture.src = "file_icons/icons8-doc-52.png";
          showIconPlace.appendChild(picture);
               
          displayFileParameter(f);
    }
```

Resztę kodu można znaleźć w folderze
 

