Partei-Vergleich im Rahmen des Moduls Natural Language Processing an der FH-SWF im WS24/25.

Die Notebooks sind in folgender Reihenfolge zu durchlaufen:
1. collect_data
2. daten_verarbeiten
3. BERTopic
4. rag_ausgabe

Das Notebook collet_data sammelt Plenarsitzungen in dem Ordner "BTP20_Downloads" und Wahlprogramme in "BTW25_Downloads".

In daten_verarbeiten erstellt eine ChromaDB mit Embeddings der Protokolle und Programme welche in einem entsprechenden Ordner "chromadb".

Beim BERTopic Notebook werden die Themen mithilfe der Embeddings aus der ChromaDB modelliert und als JSON exportiert.

Im Notebook rag_ausgabe werden mit den ChromaDB Embeddings, den JSON-Topics und dem LLM "meta-llama/Llama-3.3-70B-Instruct" ein Vergleich zwischen den Parteien realisiert, wobei die LLM Ausgaben als JSON wieder exportiert werden
