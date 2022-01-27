# SVR
SVR - Modelka oświetlenie
Projekt oparty o rozwiązanie ThreeDPoseUnityBarracuda - https://github.com/digital-standard/ThreeDPoseUnityBarracuda****
# Przygotowanie środowiska
Projekt należy uruchamiać w Unity 2019.3.13f1. Po pobraniu projektu, należy pobrać model sieci neuronowej z adresu: 
https://digital-standard.com/threedpose/models/Resnet34_3inputs_448x448_20200609.onnx.
Następnie w uruchomionym projekcie należy uruchomić scenę "Sample Scene", jeśli prosi o zapisanie klikamy "nie".
W tej scenie umieszczamy sieć neuronową pod ścieżką: Assets/Scripts/Model. 
W inspektorze znajdujemy obiekt "BarracudaRunner" i wrzucamy NN Model z poprzedniego kroku do pola o nazwie "NN Model".
![obraz](https://user-images.githubusercontent.com/58195641/151460331-5ce3f56b-f97e-466a-9b1b-92b7efb74824.png)

Następnie uruchamiamy całe rozwiązanie. 

Aby użyć trybu z kamerą w obiekcie MainTexture ustawiamy "Use Web Cam" na true.
![obraz](https://user-images.githubusercontent.com/58195641/151460453-a5a88488-0349-4974-968b-560a0f12d274.png)


# Sposób użycia
Przy użyciu sieci neuronowych mapowana jest sylwetka osoby stojącej przed kamerą a model umieszczany jest na scenie. 

Scena wyposażona jest w trzy lampy, których parametrami sterujemy w trybie edycji. Aby wejść w tryb edycji należy lewym przyciskiem myszy kliknąć w jedną z lamp. Wyjście jest poprzez przycisk Exit Edit Mode.

Poza trybem edycji użytkownik może kierować kamerą używająć "WSAD" oraz myszki wraz z jej przyciskami
