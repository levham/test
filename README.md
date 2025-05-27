# 📂 interface
 Bu program ile kendi butonlu menünüzü button.json dosyası üzerinden yazabilirsiniz.

 _! Button.json içeriğini değiştirdikten sonra a16.exe'yi çalştırabilirsiniz._

_Program şurada -> **bin\Debug\net8.0-windows\a16.exe**_ 

# button.json 
| 📁 Parametre | 📌 Açıklama|
|---------------|-------------------|
| **form**       | _pencere hakkında_|
| `width: 500`       | _pencere genişliği_|
| `height: 120`      | _pencere yüksekliği_|
|`location:[0, 0]`     | _pencere konumu_|
| **button**   | _butonlar_|
| **events**    | _çalıştırılacak programlar_|
| `eventName` | _çalıştırılacak program_|



_**Örnek Button.json**_
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
	    [   { "id": 1,   "text": "Cmd"  }, { "id": 2,   "text": "Notepad"}  ]
    	],
    
    "events": 
	[
            {   "id": 1, "eventName": "C:\\Windows\\System32\\cmd.exe" },
            {   "id": 2, "eventName": "C:\\Windows\\System32\\notepad.exe"}
    	]

}
```


_**Örnek2 Button.json**_
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
	    [   { "id": 1,   "text": "Cmd"  }, { "id": 2,   "text": "Notepad"}  ]
	    [   { "id": 3,   "text": "Paint"  }, { "id": 4,   "text": "Taskmgr"}  ]
    	],
    
    
    "events": 
	[
            {   "id": 1, "eventName": "C:\\Windows\\System32\\cmd.exe" },
            {   "id": 2, "eventName": "C:\\Windows\\System32\\notepad.exe"}
            {   "id": 3, "eventName": "C:\\Windows\\System32\\mspaint.exe"}
            {   "id": 4, "eventName": "C:\\Windows\\System32\\taskmgr.exe"}
    	]

}
```
