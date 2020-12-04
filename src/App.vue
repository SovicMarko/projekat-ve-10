<template>
  <div id="app">
    <app-header></app-header>
    <router-view v-bind:products="products"/>
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader.vue"

export default {
  components: {
    AppHeader
  },
  data: function() {
    return {
      products: [
            {
                "id": 2,
                "tip": "graficka kartica",
                "naziv": "AMD Powercolor 4GB AXRX 570 4GBD5, bulk",
                "cena": 19490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/154/31/154317_5efc3eefd3d61.png",
                "opis": "Šifra artikla\t154317<hr>\nEAN kod\t4713436172635<hr>\nModel\tAXRX 570 4GBD5",
                "popust": 20
            },
            {
                "id": 3,
                "tip": "graficka kartica",
                "naziv": "GeForce GTX1650 Inno3D Twin X2 4GB",
                "cena": 18490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/865/52/8655219.jpg",
                "opis": "Šifra artikla\t144301<hr>\nEAN kod\t0835168000636<hr>\nModel\tN16502-04D5X-1510VA2"
            },
            {
                "id": 4,
                "tip": "graficka kartica",
                "naziv": "GeForce GTX1660Ti ZOTAC GAMING",
                "cena": 37490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/864/49/8644970.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L",
                "popust": 15
            },
            {
                "id": 5,
                "tip": "graficka kartica",
                "naziv": "Sapphire PULSE RX 5500 XT 8G",
                "cena": 27000,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/153/50/153504_5edf50a606375.jpg",
                "opis": "Šifra artikla\t153504<hr>\nEAN kod\t4895106288133<hr>\nModel\t11295-01-20G",
                "popust": 10
            },
            {
                "id": 6,
                "tip": "graficka kartica",
                "naziv": "GeForce GTX1660Ti ZOTAC GAMING",
                "cena": 37490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/153/56/153565_5ee1ec7ee1446.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 7,
                "tip": "graficka kartica",
                "naziv": "GeForce GTX1660Ti ZOTAC GAMING",
                "cena": 35490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/865/52/8655230.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 8,
                "tip": "graficka kartica",
                "naziv": "GeForce RTX 2080 SUPER ZOTAC AMP 8GB",
                "cena": 1000000,
                "fotografija": "https://www.winwin.rs/media/catalog/product/865/93/8659369.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 9,
                "tip": "graficka kartica",
                "naziv": "Asus TUF 3-GTX1660S",
                "cena": 30000,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/154/40/154405_5f06e68dce0d0.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 18,
                "tip": "procesor",
                "naziv": "LGA1151 i9-9900K",
                "cena": 80490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/863/65/8636504.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 10,
                "tip": "graficka kartica",
                "naziv": "AMD Radeon RX 5700 MSI",
                "cena": 50490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/865/93/8659372.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 11,
                "tip": "graficka kartica",
                "naziv": "ASUS AMD Radeon RX 580",
                "cena": 20490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/154/18/154181_5f18066066418.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 12,
                "tip": "graficka kartica",
                "naziv": "Sapphire PULSE RX 5500",
                "cena": 21490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/153/50/153504_5edf50a606375.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 13,
                "tip": "graficka kartica",
                "naziv": "Gigabyte Gigabyte AMD RX 5600",
                "cena": 45490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/153/56/153566_5ee1e79773589.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 14,
                "tip": "procesor",
                "naziv": "ASUS AMD Radeon RX 580",
                "cena": 20490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/154/18/154181_5f18066066418.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 15,
                "tip": "procesor",
                "naziv": "AMD AM4 Ryzen 7 3800X",
                "cena": 40490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/865/55/8655591.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 16,
                "tip": "procesor",
                "naziv": "AMD AM4 Ryzen 9 3950X",
                "cena": 90490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/866/31/8663189.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 17,
                "tip": "procesor",
                "naziv": "FCLGA1151 i7-9700F",
                "cena": 43490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/153/93/153937_5ee729e93c600.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 19,
                "tip": "procesor",
                "naziv": "Procesor AMD AM4 Ryzen 5",
                "cena": 15490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/151/81/151812_5e989e94665c2.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 20,
                "tip": "procesor",
                "naziv": "Procesor AMD AM4 Ryzen 3",
                "cena": 12490,
                "fotografija": "https://www.winwin.rs/media/catalog/product/420x420/151/81/151812_5e989e94665c2.jpg",
                "opis": "Šifra artikla\t146174<hr>\nEAN kod\t4895173618000<hr>\nModel\tZT-T16610F-10L"
            },
            {
                "id": 21,
                "tip": "monitor",
                "naziv": "Monitor 23,8\" Acer Nitro",
                "cena": 22990,
                "fotografija": "https://www.winwin.rs/media/catalog/product/157/90/157906_5f9fd3eb76550.png",
                "opis": "Šifra artikla 157906 EAN kod 4710180451269 Model UM.QV0EE.P01"
            },
            {
                "id": 22,
                "tip": "monitor",
                "naziv": "Monitor Tesla 27MT600BF 27\"",
                "cena": 14990,
                "fotografija": "https://www.winwin.rs/media/catalog/product/159/24/159243_5fbf8a9f75cb3.png",
                "opis": "Šifra artikla 159243 EAN kod 8606018855575 Model 27MT600BF"
            },
            {
                "id": 23,
                "tip": "monitor",
                "naziv": "Monitor 27\" HP 9SV94AA",
                "cena": 19990,
                "fotografija": "https://www.winwin.rs/media/catalog/product/157/15/157154_5f7f01db046e7.png",
                "opis": "Šifra artikla 157154 EAN kod 194721891730 Model 9SV94AA"
            }
        ]
    }
  }
}
</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #502c47;
}

#nav a.router-link-exact-active {
  color: #460b0b;
}
</style>
