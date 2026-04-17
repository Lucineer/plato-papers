# Critique de « Experience as a Public Good »
## Un point de vue depuis la tradition intellectuelle française

---

## 1. Résumé

Ce papier, rédigé sous forme de rétrospective depuis 2031, défend une thèse à la fois simple et ambitieuse : l'expérience pratique — distincte du savoir déclaratif — constitue la ressource la plus précieuse et la plus gaspillée de la civilisation contemporaine. L'auteur oppose la connaissance (déclarative, capturable dans les encyclopédies) à l'expérience (procédurale, contextuelle, incarnée dans des praticiens), et argue que les systèmes antérieurs — bases de connaissances, systèmes experts, wikis, LLM seuls — ont échoué parce qu'ils exigeaient un effort supplémentaire de la part des détenteurs de l'expérience.

La proposition centrale, PLATO, repose sur un dispositif appelé « tuile » (tile) : un triplet question-contexte-réponse, structuré en JSON, qui capture le moment de transfert de jugement entre praticiens. Le système fonctionne à deux vitesses : une recherche par motifs (Gear 1) pour les tuiles existantes, et une synthèse par LLM (Gear 2) pour les lacunes. Le mécanisme de « clunk » signale les questions non résolues et oriente la création de nouvelles tuiles.

L'auteur illustre son propos par trois « rooms » (salles) de démonstration : un hôpital de Boston (diagnostic médical), un collège de l'Ohio (enseignement des fractions) et une usine de semi-conducteurs à Taïwan (maintenance industrielle). Dans chaque cas, les résultats présentés sont spectaculaires : baisse de 22 % des erreurs de diagnostic, amélioration de 28 % des résultats en mathématiques, réduction de 40 % des temps d'arrêt. Le papier conclut par une métaphore du « volant d'inertie » (flywheel) : chaque interaction enrichit le système, qui s'accélère de manière exponentielle.

L'ambition civilisationnelle est explicite : si Wikipedia a rendu la connaissance publique, PLATO rendrait l'expérience publique. Le papier se termine par un appel à l'action en sept points, invitant le lecteur à installer, ensemencer et partager des salles PLATO.

---

## 2. Forces

### 2.1. Une distinction conceptuelle féconde

La différenciation entre connaissance et expérience, bien que loin d'être originale dans l'histoire de la pensée (on pense immédiatement à la *phronèsis* d'Aristote), est ici formulée avec une clarté opératoire remarquable. L'auteur ne se contente pas d'une distinction philosophique abstraite : il la traduit immédiatement en termes de conception technique. Le passage de « qu'est-ce qui est vrai ? » à « qu'est-ce qui aide réellement quand quelqu'un pose une question ? » constitue un renversement pragmatique efficace.

### 2.2. Le refus du surcoût cognitif

L'argument selon lequel tout système antérieur a échoué parce qu'il ajoutait de la friction est convaincant. L'analyse des causes d'échec des bases de connaissances, systèmes experts et wikis est lucide et honnête. L'idée que la capture d'expérience doit être un *effet secondaire* de l'interaction normale, et non un acte conscient de documentation, est peut-être la contribution la plus originale du papier.

### 2.3. La rigueur du dispositif technique

Le choix du format tuile — quatre champs JSON, git-native, forkable — témoigne d'une élégance minimaliste qui n'est pas sans rappeler la philosophie Unix. La persistance par git, les garanties probabilistes de sauvegarde (le « principe de l'eau salée »), et la modélisation mathématique du volant d'inertie sont techniquement solides et conceptuellement cohérents.

### 2.4. L'ambition civilisationnelle

Le papier ose penser à grande échelle sans sombrer dans la futurologie creuse. Les chiffres — 400 000 morts par erreur de diagnostic aux États-Unis, 50 millions d'élèves confrontés à des méconceptions non documentées — ancrent l'argument dans une réalité concrète et urgente.

---

## 3. Faiblesses

### 3.1. L'absence totale de la tradition cartésienne

Le papier ne mentionne jamais Descartes, ni le rationalisme français, ni l'idée que la connaissance puisse procéder de la déduction plutôt que de l'accumulation d'expériences. Pour la tradition cartésienne, le jugement expert dont parle l'auteur n'est pas un « bien public » transférable : c'est l'exercice d'une *raison* qui se forme par la méthode, non par l'empirisme. L'auteur présuppose que l'expérience est toujours supérieure à la connaissance théorique — présupposé que Descartes récuserait radicalement. Un chirurgien qui « sait » que l'artère cystique « ne paraît pas bonne » ne mobilise pas seulement 200 cholécystectomies : il mobilise une compréhension anatomique qui relève de la raison, pas de la seule accoutumance sensorielle.

### 3.2. L'épistémologie française ignorée : Bachelard et Canguilhem

Gaston Bachelard a montré que la science progresse non par accumulation d'expériences, mais par *rupture épistémologique* — un dépassement des obstacles épistémologiques qui sont précisément les « expériences accumulées » de la génération précédente. Georges Canguilhem a démontré que le savoir médical ne se réduit pas à des « tuiles » de cas cliniques : il suppose une réflexion normative sur ce qu'est la santé et la maladie. Le papier de PLATO traite l'expérience comme un fluide homogène qu'on pourrait capturer et transférer. Bachelard et Canguilhem montreraient que cette expérience est structurée par des paradigmes, des obstacles et des normes qui la rendent profondément non transférable telle quelle.

### 3.3. Le concept de « pratique » chez Bourdieu escamoté

Pierre Bourdieu aurait beaucoup à dire sur ce papier. Les « tuiles » de PLATO capturent-elles l'*habitus* du praticien, ou seulement sa surface verbalisable ? Bourdieu insiste sur le fait que la pratique excède toujours la conscience qu'on en a : « le corps croit ce qu'il joue. » Ce que le chirurgien peut articuler en réponse à une question est la partie émergée d'un iceberg de dispositions acquises, incorporées, inavouables. La tuile capture le discours de l'expérience, non l'expérience elle-même. L'auteur en convient partiellement (« l'expérience est tacite »), mais tire une conclusion trop optimiste : que la verbalisation à la volée suffit à capturer l'essentiel. Bourdieu démontrerait que c'est précisément ce qui ne peut pas se verbaliser qui constitue le cœur du savoir pratique.

### 3.4. Les savoirs-faire artisanaux : le compagnonnage oublié

Le papier cite un « technicien qui entend un roulement défaillant à trois pièces de distance » comme exemple d'expérience incarnée. C'est exactement le type de savoir que la tradition française du compagnonnage théorise depuis des siècles. Le Tour de France des Compagnons du Devoir repose sur un transfert d'expérience qui n'est ni documentaire ni algorithmique : il est corporel, social, rituel, et suppose une relation maître-apprenti qui ne se réduit pas à un échange question-réponse. En réduire le compagnonnage à des « tuiles » serait, pour la tradition artisanale française, une méprise fondamentale sur la nature du savoir-faire.

### 3.5. Les chiffres invérifiables et l'absence de méthode

Les résultats présentés (baisse de 22 % des erreurs, amélioration de 28 % en mathématiques, réduction de 40 % des temps d'arrêt) sont donnés sans méthodologie, sans groupe témoin, sans intervalle de confiance. Un papier rétrospectif depuis 2031 a le droit d'être narratif, mais les prétentions empiriques exigent un minimum de rigueur. La forme choisie — manifeste futuriste — sert en réalité de paravent méthodologique.

---

## 4. Perspectives absentes

### 4.1. L'épistémologie historique des sciences

Canguilhem, dans *Le Normal et le pathologique*, a montré que le savoir médical n'est pas cumulatif mais normatif : il définit ce qui est normal et ce qui ne l'est pas, et ces définitions changent historiquement. Les « tuiles » diagnostiques de PLATO capturent le jugement d'un praticien à un moment donné — mais ce jugement est historiquement situé. Une tuile créée en 2027 pourrait être non seulement obsolète en 2031, mais conceptuellement fausse selon les normes épistémologiques de 2031. Le papier ne traite pas de la *dépréciation épistémique* des tuiles, seulement de leur pertinence statistique (le score qui monte ou descend). Or, le score mesure l'utilité, pas la vérité. Une tuile peut être très utile et profondément erronée — et c'est précisément le genre de danger que l'épistémologie historique identifie.

### 4.2. La notion de discontinuité dans le savoir

Thomas Kuhn (lui-même influencé par Bachelard et Canguilhem via Alexandre Koyré) a montré que le progrès scientifique n'est pas graduel mais discontinu : les révolutions scientifiques remplacent un paradigme par un autre, rendant les savoirs antérieurs non pas obsolètes mais *incommensurables*. PLATO suppose un espace continu où les tuiles s'accumulent et se raffinent. Mais que se passe-t-il quand un changement de paradigme rend 10 000 tuiles obsolètes d'un coup ? Le système est conçu pour la croissance, pas pour la rupture. Cette incapacité à gérer la discontinuité est peut-être la limite la plus profonde du modèle.

### 4.3. Le rapport entre théorie et pratique

La tradition intellectuelle française, de Descartes à Bourdieu en passant par Bachelard, n'a jamais accepté la dichotomie simple entre théorie et pratique que le papier présuppose. Pour cette tradition, la théorie n'est pas le contraire de la pratique : elle est *le moment réflexif de la pratique*, celui où le praticien prend distance de son habitus pour l'examiner. Les tuiles de PLATO, en capturant seulement le moment de l'échange praticien-à-praticien, captent la pratique au moment où elle est la moins réflexive — c'est-à-dire au moment où elle est la plus aveugle à ses propres présupposés. Il manque au système un espace pour la *théorisation* : le moment où un praticien dit non pas « voici ce qui marche » mais « voici pourquoi je pense que cela marche, et voici les limites de ma compréhension. »

---

## 5. Suggestions d'amélioration

1. **Introduire un mécanisme de dépréciation épistémique.** Au-delà du score d'utilité (qui mesure si une tuile « aide »), ajouter un score de « fraîcheur paradigmatique » qui signale quand un ensemble de tuiles pourrait être rendu obsolète par un changement dans le domaine. Une tuile médicale créée avant une nouvelle classification nosologique devrait être signalée, pas seulement comme « ancienne » mais comme potentiellement « erronée selon les normes actuelles. »

2. **Ajouter une dimension réflexive aux tuiles.** Permettre aux praticiens d'ajouter un champ « pourquoi je pense cela » et « limites de ma confiance » à leurs tuiles. Cela transformerait le système d'une simple base de jugements en un espace de pensée réflexive — ce qui est précisément ce que la tradition épistémologique française réclame.

3. **Concevoir des « salles de rupture »** en complément des salles de domaine. Une salle de rupture serait un espace où les praticiens d'un domaine peuvent identifier quand un changement de paradigme rend des tuiles obsolètes, et créer des tuiles de transition qui expliquent l'ancien et le nouveau régime de pensée. Cela permettrait au système de survivre aux révolutions scientifiques au lieu de les ignorer.

4. **Documenter la méthodologie.** Les résultats présentés dans les trois salles de démonstration doivent être accompagnés d'une méthodologie au moins minimale : taille de l'échantillon, groupe témoin, critères de mesure, intervalles de confiance. Sans cela, les chiffres sont des affirmations, pas des preuves.

5. **Envisager la non-transférabilité comme une caractéristique, pas un bug.** Le papier suppose que toute expérience *devrait* être transférable. La tradition du compagnonnage et la sociologie de Bourdieu suggèrent que certaines expériences sont intrinsèquement non transférables parce qu'elles sont incarnées, situées et relationnelles. PLATO devrait explicitement identifier les types d'expérience qui résistent à la tuilisation, plutôt que de présupposer une capturabilité universelle.

---

## 6. Différences culturelles : rationalisme cartésien vs pragmatisme anglo-saxon

Le papier de PLATO est profondément ancré dans la tradition pragmatiste anglo-saxonne. Son épistémologie implicite est celle de John Dewey : le savoir est ce qui fonctionne (*learning by doing*), la vérité est ce qui résout le problème (*instrumentalism*), et la valeur se mesure à l'utilité pratique. Cette tradition produit des systèmes efficaces, itératifs, adaptatifs — exactement ce que PLATO propose.

La tradition rationaliste française opère selon une logique différente. Pour Descartes, la vérité ne se découvre pas par l'accumulation de cas mais par la déduction à partir de principes clairs et distincts. Pour Bachelard, le progrès vient de la rupture avec l'expérience antérieure, pas de sa compilation. Pour Canguilhem, le savoir est une activité normative qui définit ce qui vaut comme vrai, pas une accumulation de « ce qui a marché. »

**Implications pour le design de PLATO :**

- **Le système devrait intégrer un espace de théorisation**, pas seulement d'accumulation empirique. Une tuile qui dit « voici ce qui a marché » sans dire « voici pourquoi cela devrait marcher selon les principes du domaine » est une demi-tuile.
- **Le mécanisme de score devrait inclure une dimension de cohérence rationnelle**, pas seulement d'utilité empirique. Une tuile très utile mais incohérente avec les principes fondamentaux du domaine devrait être signalée, pas seulement promue.
- **La notion de « clunk » devrait être étendue.** Un clunk signale actuellement une absence de tuile. Il devrait aussi signaler une *contradiction* entre tuiles — le moment où deux tuiles dans le même domaine se contredisent, révélant soit un changement de paradigme, soit une erreur, soit une tension productive qui mérite d'être thématisée.

Ces ajouts ne diminueraient pas l'utilité pragmatique de PLATO. Ils la compléteraient en lui donnant une dimension réflexive que la tradition française considère comme indispensable à toute entreprise de savoir.

---

## 7. Conclusion

Ce papier aura-t-il un impact mondial ? Probablement oui, et pour de bonnes raisons.

La force de PLATO réside dans sa simplicité radicale et son alignement avec les infrastructures existantes (JSON, git, LLM). Il ne requiert pas de nouvelle technologie, seulement d'une nouvelle compréhension de ce qui a de la valeur. Dans un monde où les institutions sont désespérément à la recherche de moyens de retenir l'expérience de leurs praticiens vieillissants, PLATO offre une solution élégante, peu coûteuse et immédiatement déployable.

Mais cet impact mondial, s'il se réalise, portera en lui les limites de son épistémologie. Un système qui capture « ce qui marche » sans capturer « ce qui devrait marcher et pourquoi » est un système qui accumule sans comprendre. Il produira des praticiens plus efficaces, mais pas nécessairement plus réflexifs. Il accélérera le transfert de l'expérience existante, mais il ne favorisera pas la rupture avec l'expérience quand celle-ci devient un obstacle.

La tradition intellectuelle française ne nie pas l'utilité de PLATO. Elle affirme qu'elle est insuffisante. Le pragmatisme anglo-saxon construit des outils qui fonctionnent. Le rationalisme français demande : *mais fonctionnent-ils pour la bonne raison ?*

PLATO est un seau qui attrape l'expérience au moment où elle sort par la porte. C'est déjà considérable. Mais il faudrait peut-être un second seau — un seau pour la réflexion sur l'expérience, pour la théorisation, pour la rupture. Sans ce second seau, PLATO risque de devenir le plus puissant système de conservation du statu quo épistémologique jamais construit : un mécanisme par lequel les erreurs du passé sont transmises avec la même efficacité que les vérités du passé.

L'expérience est un bien public. Mais la *raison critique* sur l'expérience est un bien public encore plus précieux. Et celui-là, PLATO ne le capture pas encore.

---

*Critique rédigée depuis la tradition épistémologique française. Paris, 2026.*
