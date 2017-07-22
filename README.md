# belajar_bower
Membuat Template Web Server dengan Bower sebagai Dependency

*	tambahkan files project belajar_express sebagai dasar webserver
*	rubah port ke 5000 untuk membedakan dengan project belajar_express
	```js
	var port = 3000;
	```
*	instal bower
	```cmd
	>npm install -g bower
	```
* 	buat file bower.json dengan command >bower init
*	buat file .bowerrc
	```bower
	{
	  "directory" : "app/bower_components"
	}
	```
*	coba instal jquery dan bootstrap >bower install jquery bootstrap --save
* 	akan muncul script berikut di bower.json file
	```json
	"dependencies": {
	    "jquery": "^3.2.1",
	    "bootstrap": "^3.3.7"
	}
	```
*	akan ada folder bower_componets di dalam folder app sesuai dengan konfigurasi file .bowerrc
*	file-file jquery dan bootstrap ada didalam bower_components yang siap digunakan dalam file html
*	untuk menambahkan dependencies bisa dengan menambahkan didalam bower.json lalu >bower install 
	```json
	"dependencies": {
		"angular": "1.6.x", //<==== ini di tambahkan
	    "jquery": "^3.2.1",
	    "bootstrap": "^3.3.7"
	}
	```