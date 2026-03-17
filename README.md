# Captain Starman — PWA Assets

Generiert mit PWA Builder (privates Tool)
Datum: 17.3.2026

## Inhalt
- manifest.json    → PWA Manifest
- sw.js            → Service Worker (Offline First)
- icons/           → App Icons (72, 96, 128, 144, 152, 192, 384, 512px)

## Installation
1. Dateien in deinen PWA-Ordner kopieren
2. In index.html im <head> einfügen:
   <link rel="manifest" href="manifest.json">
   <meta name="theme-color" content="#1A1916">
3. Vor </body> einfügen:
   <script>
     if ('serviceWorker' in navigator) {
       navigator.serviceWorker.register('/sw.js');
     }
   </script>
