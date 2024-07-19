# odev_son
Bu problem ifadesine göre, nesne yönelimli programlama ilkelerini ve sınıflar arası ilişkileri kullanarak bir sınıf diyagramı tasarlayabiliriz. Tasarımda enkapsülasyon, kalıtım, polimorfizm ve soyutlama ilkelerini uygulamaya çalışacağız.

Sınıflar ve İlişkiler
Building (Bina) Sınıfı:

Özellikler: floors, elevators
İlişkiler: Bir binada birden fazla kat ve asansör bulunur.
Floor (Kat) Sınıfı:

Özellikler: floorNumber, elevatorDoors, arrivalBell, callButtons
İlişkiler: Her kat, bir binaya aittir ve birden fazla asansör kapısına, varış ziline ve çağrı düğmesine sahiptir.
Elevator (Asansör) Sınıfı:

Özellikler: elevatorID, currentFloor, capacity, controlPanel, door, indicatorLight
İlişkiler: Her asansör bir binaya aittir ve bir kontrol paneline, kapıya, gösterge ışığına sahiptir. Asansörler ControlPanel ve Door nesnelerini içerir.
ControlPanel (Kontrol Paneli) Sınıfı:

Özellikler: targetButtons, openDoorButton, closeDoorButton, emergencyButton
İlişkiler: Bir kontrol paneli bir asansöre aittir.
Door (Kapı) Sınıfı:

Özellikler: isOpen
İlişkiler: Bir kapı bir asansöre aittir ve open() ve close() gibi metotları içerir.
CallButton (Çağrı Düğmesi) Sınıfı:

Özellikler: direction (yukarı/aşağı), isPressed
İlişkiler: Bir çağrı düğmesi bir kata aittir.
ArrivalBell (Varış Zili) Sınıfı:

Özellikler: isRinging
İlişkiler: Bir varış zili bir kata aittir.
Passenger (Yolcu) Sınıfı:

Özellikler: currentFloor, destinationFloor
İlişkiler: Her yolcu bir binada bulunur ve bir asansöre biner.
Clock (Saat) Sınıfı:

Özellikler: currentTime
İlişkiler: Saat, simülasyonun zamanını izler ve olayları günlüğe kaydeder.
Simulator (Simülatör) Sınıfı:

Özellikler: building, clock
İlişkiler: Simülatör, bina ve saat nesnelerini içerir ve simülasyonu yönetir.

Açıklama:
Building: Bina sınıfı, katları ve asansörleri yönetir.
Floor: Kat sınıfı, asansör kapılarını, varış zilini ve çağrı düğmelerini içerir.
Elevator: Asansör sınıfı, kontrol panelini, kapıyı ve gösterge ışığını içerir.
ControlPanel: Asansörün kontrol panelini modelleyen sınıf.
Door: Asansör kapısını modelleyen sınıf.
CallButton: Katlardaki asansör çağrı düğmesini modelleyen sınıf.
ArrivalBell: Katlardaki varış zilini modelleyen sınıf.
Passenger: Yolcuları modelleyen sınıf.
Clock: Simülasyonun zamanını takip eden saat sınıfı.
Simulator: Simülasyonun tüm işleyişini yöneten sınıf.
Bu tasarım, nesne yönelimli programlamanın ilkelerini (enkapsülasyon, kalıtım, polimorfizm ve soyutlama) kullanarak asansör sistemini modellemektedir.







