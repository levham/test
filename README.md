# 📂 interface
_Program şurada -> **bin\Debug\net8.0-windows\a16.exe**_ 

 Bu program ile kendi butonlu menünüzü json dosyası üzerinden yazabilirsiniz

 !Button.json içeriğini değiştirebilirsiniz

# Button.json 
| 📁 Parametre | 📌 Açıklama|
|---------------|-------------------|
| **form**       | _pencere hakkında_|
| `width: 500`       | _pencere genişliği_|
| `height: 120`      | _pencere yüksekliği_|
|`location:[0, 0]`     | _pencere konumu_|
| **button**   | _butonlar_|
| **events**    | _çalıştırılacak programlar_|
| `eventName` | _çalıştırılacak program_|


Örnek Button.json
```
{ 
    "form": 
	{
            "width": 500,
            "height": 120,
            "location": [0, 0]
    	},

     "buttons":  
	[
            { "id": 1,   "text": "Cmd"  },
            { "id": 2,   "text": "Notepad"}
    	],
    
    "events": 
	[
            {   "id": 1, "eventName": "C:\\Windows\\System32\\cmd.exe" },
            {   "id": 2, "eventName": "C:\\Windows\\System32\\notepad.exe"}
    	]

}
```

