# OOD
# Designmönster: Strategy Pattern
Då mitt parkeringssystem har olike priser beroende på tid på dygn och eventuella zoner. 

Strategy Pattern passar då eftersom det tillåter att välja olika "strategier" för priessättning vid runtime.

Det förbättrar systemets flexibilitet och underhållbarhet då gör det lätt att lägga till nya strategier utan att ändra existerande logik.
# Use Case: Beräkning av parkeringsavgift
Aktör: Parkeringsanvändare
Preconditions: Användaren har valt områdeskod och fyllt i starttid
Flöde:

1. Systemet identifierar tidpunkt (t.ex. 22:00)
2. Rätt strategi (NightTimeRateStrategy) används för att beräkna pris
3. Pris presenteras för användaren innan köp

Postcondition: Användaren ser korrekt avgift.

# User Story:
Som bilförare vill jag att systemet automatiskt väljer rätt prissättning beroende på tid på dygnet så att jag slipper tänka om det är dag eller nattaxa.
