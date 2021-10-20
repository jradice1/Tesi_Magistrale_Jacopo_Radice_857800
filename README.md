# Tesi_Magistrale_Jacopo_Radice_857800
## Enriching Word Embeddings with Multiword Expressions

Files relativi alla tesi di laurea dal titolo Enriching Word Embeddings with Multiword Expressions.

Nella cartella data sono presenti i dati utilizzati per gli esperimenti.

In preprocessing vi è il codice relativo alle fasi di preprocessing per Wiki50, Wikipedia titles dump e CCOHA2.

In direct_testing è presente il codice relativo a tutti i test fatti su corpus annotato, in particolare in Wiki50 sono utilizzati e confrontati 5 approcci (Gensim Phrases, W2P, TopicRank, YAKE, RAKE). PoS-Entities è presente singolarmente per via della sua maggiore complessità rispetto ai metodi precedenti.

In ccoha_methods, tutti i metodi più promettenti utilizzati sul testo oggetto di esperimenti: in output viene restituito tale testo modificato con le MWEs.

Nella cartella benchmarks sono presenti: 
delete_missing_words, codice relativo alla cancellazione delle coppie o gruppi di parole non presenti nel corpus; 
new_datasets, contentente il codice con il conteggio delle coppie o gruppi nel corpus e successiva creazione di 3 classi di dataset suddivisi per frequenza;  vector_analysis, nel quale viene controllato l'intorno di alcune coppie di parole e i risultati di alcune analogie prese a campione;  
word_embeddings_benchmarks, contentente il codice relativo ai benchmarks su analogie e similarità. N.B. è stato riportato per completezza, preferibilmente utilizzare localmente clonando la repository al link: https://github.com/kudkudak/word-embeddings-benchmarks ; 
benchmarks_results, codice per verificare i risultati e i delta dei benchmark effettuati in precedenza.

Infine è presente il codice relativo al training di modelli Word2vec.

N.B. il codice presente è in formato Jupyter Notebook, avendo effettuato gran parte dei test utilizzando Google Colab per motivi di performance.
