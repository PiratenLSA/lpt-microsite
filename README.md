## Vorraussetzungen

Dieses "Projekt" benötigt **node.js** inklusive **npm**. Außerdem wird das
node.js module **wintersmith** benötigt:

    sudo npm install wintersmith -g

Man sollte es global installieren, da es ausführbare Programme enthält.

## Cloning

Dieses Repository enthält ein submodule, daher beim clonen die Option
"--recursive" angeben:

    git clone --recursive https://github.com/PiratenLSA/lpt-microsite.git

Alternativ geht das Laden des Submodules auch nach dem clonen:

    git clone https://github.com/PiratenLSA/lpt-microsite.git
    git submodule update --init --recursive

## Vorbereiten

Es müssen die node.js Module für das submodule geladen werden:

    cd wintersmith-jade
    npm install

## Ausführen

Zum testen:

    wintersmith preview

Dies erstellt einen Server und lauscht standardmäßig auf Port 8080.

Zum erstellen der HTML-Dateien:

    wintersmith build
