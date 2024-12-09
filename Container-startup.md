# Container Startup Process

1. Pobranie wybranego obrazu, pod warunkiem że nie został on już pobrany wcześniej.
2. Tworzenie kontenera.
3. Załadowanie systemu plików i utworzenie warstwy do odczytu i zapisu.
4. Inicjalizacja sieci (bridge network).
5. Konfiguracja sieci (adresu IP).
6. Uruchomienie kontenera.
7. Przechwycenie wyjścia - utworznie logów kontenera. 
