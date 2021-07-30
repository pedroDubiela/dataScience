# Objetivo:
Desenvolvimento de um sistema especializado para diagnóstico de doenças na plantação de soja.

# Como ele faz?
Aplicando métodos de Machine Learning (classificação - aprendizado supervisionado) em uma base de dados histórica que correlaciona diversas características apresentada pela soja com sua respectiva doença, os modelos serão treinados para diagnóstico dessas doenças.

# Descrição do Banco de Dados:
O banco de dados possui 35 atributos previsores, ou seja, ele traz 35 características avaliadas que estão correlacionadas a uma doença específica, tais como: Data da plantação; Características das folhas; se houve granizo ou não; Manchas nas olhas; tamanho das manchas etc. A base histórica traz 683 registros analisados, que estão classificados dentre 19 tipos de doenças (as classes).
Apresento abaixo as classes e os atributos previsores, os quais não traduzi, pois dentro da própria análise também utilizei os nomes em inglês:

  1)Classes: Diaporthe-stem-canker, charcoal-rot, rhizoctonia-root-rot, phytophthora-rot, brown-stem-rot,
  powdery-mildew, downy-mildew, brown-spot, bacterial-blight, bacterial-pustule, purple-seed-stain, anthracnose,
  phyllosticta-leaf-spot, alternarialeaf-spot, frog-eye-leaf-spot, diaporthe-pod-&-stem-blight, cyst-nematode, 2-4-d-injury,
  herbicide-injury.
  
 2)Atributos Previsores: Onde consta dna, significa que não se aplica (dna = Does not  apply)
 1) date: april , may, june, july, august, september, October
 2) plant-stand: normal, lt-normal;
 3) precip: t-norm, norm, gt-norm;
 4) temp: lt-norm, norm, gt-norm;
 5) hail: yes,no;
 6) crop-hist: diff-lst-year, same-lst-yr, same-lst-two-yrs, same-lst-sev-yrs;
 7) area-damaged: scattered, low-areas, upper-areas, whole-field;
 8) severity: minor, pot-severe, severe;
 9) seed-tmt: none, fungicide, other;
 10) germination: 90-100%, 80-89%, lt-80%;
 11) plant-growth: norm, abnorm;
 12) leaves: norm,abnorm;
 13) leafspots-halo: absent, yellow-halos, no-yellow-halos;
 14) leafspots-marg: w-s-marg, no-w-s-marg, dna;
 15) leafspot-size: t-1/8, gt-1/8, dna;
 16) leaf-shread: absent, present;
 17) leaf-malf: absent, present;
 18) leaf-mild: absent, upper-surf, lower-surf;
 19) stem: norm, abnorm;
 20) lodging: yes, no;
 21) stem-cankers: absent, below-soil, above-soil, above-sec-nde;
 22) canker-lesion: dna, brown, dk-brown-blk, tan;
 23) fruiting-bodies: absent, present;
 24) external decay: absent, firm-and-dry, watery;
 25) mycelium: absent, present;
 26) int-discolor: none, brown, black;
 27) sclerotia: absent, present;
 28) fruit-pods: norm, diseased, few-present, dna;
 29) fruit spots: absent, colored, brown-w/blk-specks, distort, dna;
 30) seed: norm, abnorm;
 31) mold-growth: absent, present;
 32) seed-discolor: absent, present;
 33) seed-size: norm, lt-norm;
 34) shriveling: absent, present;
 35) roots: norm, rotted, galls-cysts.
    
# Resultados:
Os modelos de Machine Learning utilizados e suas respectivas taxas de acerto foram:
  1) Rede Neural (98.4%).
  2) RandomForest (92,6%). 
  3) Árvores de Decisão (90,0%). 
  4) NaiveBayes (87,4%).
  5) SVC – (80,0%). 
  6) KNN (77,4%).

# Referências dos Dados: Explicações técnicas sobre a base de dados podem ser encontradas na fonte:
  1) Autor: R.S. Michalski e R.L. Chilausky (Doadores: Ming Tan e Jeff Schlimmer)
  2) Fonte: [UCI] (https://archive.ics.uci.edu/ml/datasets/Soybean+ (Grande)) – 1988
