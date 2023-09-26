# SVGTurkiyeIsiVeDegerHaritasi
Dashboard lar için kullanılabilecek SVG Türkiye ısı ve değer haritası. 

"github.com/dnomak/svg-turkiye-haritasi" adresindeki arkadaşın yaptığı svg yi, json değer alıp kullanılabilecek şekilde yapıldı.

Dahsboard ekranları için "Türkiye Isı Haritası" veya "İl Bazlı Sayı İstatistikleri" amacıyla kullanılabilir. 

## Kullanımı
"../index.html" sayfasında yer almaktadır.

	<link href="css/svg-harita.css" rel="stylesheet" />
	<script src="js/svg-harita.js"></script>

	$(document).ready(function () {
    	function donusClick(ilID) {
	         alert(ilID)
	    }
		var degerler = [{ ilID: 1, deger: 812.3 }, { ilID: 6, deger: 400.23 }];
		svgturkiyeharitasi('haritaDiv', degerler, donusClick, '255 179 0');
	});

------------
	svgturkiyeharitasi('Haritanın konacağı div ID', 'dizi', 'tıklandığında çalışacak fonksiyon. Boş verilebilir.', 'rgb renk kodu'
