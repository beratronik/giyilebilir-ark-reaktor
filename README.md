# Giyilebilir Ark Reaktör!

![Giyilebilir Ark Reaktör](img/maxresdefault.webp)

## Giyilebilir Reaktör Projesi
3D yazıcı ile yapılan bu aksesuar ile Tony Stark oluyoruz. 🌟

Proje hakkında daha fazla bilgi almak için aşağıdaki videoyu izleyebilirsiniz:
[YOUTUBE VİDEOSU: Giyilebilir Ark Reaktör Projesi](https://www.youtube.com/watch?v=k6pyL6MHIts)

### 3D Baskı Dosyaları
Projenin 3D baskı dosyalarına [buradan ulaşabilirsiniz](https://www.thingiverse.com/thing:4544459).

## Malzeme Listesi

- [Led]
- [Jumper Kablo]
- [Filament]
- [USB Kablo]

---

## Arduino Kodu

```cpp
/***************************************************************************
*                                                                          *
*       Giyilebilir Ark Reaktör                                            *
*       Youtube: https://youtu.be/k6pyL6MHIts                               *
*                                                                          *
***************************************************************************/
#include <SPI.h>
#include <Wire.h>

void setup() {
  pinMode(10, OUTPUT);  // Buton pini
}

void loop() {
  if (digitalRead(10) == HIGH) {
    // Reaktör'ü açıyoruz
    Serial.println("Reaktör Başlatıldı!");
  }
}
