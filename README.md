### README per a la Pràctica 4 - Processament del Llenguatge Humà

---

# Pràctica 4 - Processament del Llenguatge Humà

### Autores:
- Lola Monroy Mir
- Marta Nadal Par

### Data de Lliurament:
5 de juny de 2024

### Universitat:
Universitat Politècnica de Catalunya

### Facultat:
Facultat d’Informàtica de Barcelona

---

## Descripció

Aquesta pràctica té com a objectiu comparar diferents models i tècniques d'embeddings de paraules dissenyats per mesurar la similitud semàntica entre textos. S'exploren i analitzen mètodes que van des dels models bàsics com One-Hot Encoding fins a models avançats com RoBERTa. La pràctica s'implementa en un entorn de notebook que inclou tant el desenvolupament del codi com l'anàlisi dels resultats obtinguts.

## Contingut del Repositori

- **WordEmbeddings.pdf**: Document principal que conté la teoria, descripció de mètodes, anàlisi de resultats i conclusions de la pràctica.
- **practica_4.1.ipynb** i **practica_4.2.ipynb**: Notebooks de Jupyter que inclouen el codi desenvolupat per entrenar i avaluar els models d'embeddings de paraules i les seves respectives implementacions.
- **README.md**: Aquest fitxer.

## Estructura del Document

1. **Introducció**
   - Presenta els objectius de la pràctica i una visió general dels models d'embeddings de paraules que s'analitzaran.

2. **Entrenar Models de Word2Vec**
   - Descripció de l'entrenament de models Word2Vec utilitzant el corpus Catalan General Crawling.
   - Anàlisi de com la mida del dataset afecta la precisió i robustesa dels models.

3. **Entrenar Models de Similitud de Text Semàntic**
   - Comparació de diverses tècniques d'embeddings de paraules:
     - One-Hot Encoding
     - Word2Vec (mitjana simple i ponderada per TF-IDF)
     - SpaCy
     - RoBERTa (CLS, Mean i fine-tuned)
   - Anàlisi de resultats i discussió sobre l'efectivitat de cada tècnica.

4. **Models amb Embeddings Entrenables**
   - Entrenament de models utilitzant embeddings entrenables inicialitzats amb Word2Vec i embeddings aleatoris.
   - Avaluació del rendiment i capacitat de generalització d'aquests models.

5. **Conclusions**
   - Resum de descobriments clau i recomanacions per a futurs treballs en l'àrea de processament del llenguatge natural.

6. **Bibliografia**
   - Referències utilitzades en el desenvolupament de la pràctica.

## Requisits

Per executar el notebook i reproduir els resultats, es requereixen les següents llibreries i eines:

- Python 3.x
- Jupyter Notebook
- Gensim
- SpaCy
- Transformers (Huggingface)
- Scikit-learn
- Pandas
- Matplotlib

## Com Executar

1. Clona aquest repositori en la teva màquina local.
   ```bash
   git clone https://github.com/tu-usuario/PLH_4.git
   ```

2. Navega al directori del projecte.
   ```bash
   cd PLH_4
   ```

3. Instal·la les dependències necessàries.
   ```bash
   pip install -r requirements.txt
   ```

4. Obre el notebook en Jupyter.
   ```bash
   jupyter notebook notebook.ipynb
   ```

5. Executa les cel·les del notebook per entrenar els models i visualitzar els resultats.

## Notes Addicionals

- El corpus utilitzat per entrenar els models Word2Vec és el Catalan General Crawling, obtingut mitjançant tècniques de web crawling per recopilar contingut textual en català de diverses fonts web.
- S'han utilitzat tècniques de visualització com T-SNE per analitzar les relacions semàntiques capturades pels models d'embeddings de paraules.
