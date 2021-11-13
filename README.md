Időjárás naptár és óra config Conkyhoz
![ccw_screenshot](https://user-images.githubusercontent.com/58111930/141647317-b8a0063e-2f6a-4c84-877a-db45e22ca764.png)

        Beállitása :

        Csomagold ki a ccw.tar.bz2 fájlt a ~/.conky mappába ( a ccw mappát is)

        A ccw/scripts/ mappában található weather.sh-t kell szerkeszteni

        weatherLanguage="xx" 
                    (ha magyarul akarod hu)
        
        weatherUnit="metric"  
                    mértékegységek   
        
        weatherCityId="xxxxxxx" A város kódja  https://openweathermap.org/find  
        
                    Itt keresd meg a városod és az url végén levő számok pl 2761369
                    
        weatherKey="xxxxxxxxxxxxxxxxxxxxxxxx" 
        
                    https://openweathermap.org/api itt regisztrálj magadnak egy ingyenes apit
                            
        weatherlat="xx.xxxx" 
        
                    Ha megtaláltad a városod   https://openweathermap.org/find  
                    itt a Geo coords első száma pl 47.2021
                    
        weatherlon="xx.xxxx" 
                    Ha megtaláltad a városod   https://openweathermap.org/find 
                     itt a Geo coords második  száma pl 47.2021
                     
                     Ha ezzel végeztél, nyiss egy terminált: cd .conky/ccw && conky -c ccw.conf
                     
                     A jq python, és a curl kell a conky működéséhez ha nem lenne feltelepítve: sudo apt install jq curl python
