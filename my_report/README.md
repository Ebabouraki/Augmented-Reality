# Lesson: Interaction Design

### First and Last Name: Eleni Vavouraki
### University Registration Number: dpsd19009
### GitHub Personal Profile: https://github.com/Ebabouraki
### Augmented Reality Personal Repository: https://ebabouraki.github.io/Augmented-Reality/

# Introduction

# Summary


# 1st Deliverable
1ο βήμα: Έβαλα τα σχήματα (κύλινδρο και σφαίρα) βάζοντας διάστασεις, χρώματα και ορίζοντας τη κατάλληλη θέση με τη βοήθεια του κώδικα απο το: A-Frame School 

2ο βήμα: Έβαλα το χιόνι στο background με τη βόηθεια απο το A-Frame Particle System 

3ο βήμα: Στη συνέχεια έψαξα για να βρω και να προσθέσω στο κώδικα μου τη φωνητική εντολή για να αρχίζει ή να σταματάει να χιονίζει 

# 2nd Deliverable


## 1ο υποερώτημα 
- Αρχικά έκανα ένα καινούργιο `a-marker` για τον marker του dpsd μου  από [εδώ](https://www.oodlestechnologies.com/blogs/how-to-create-your-own-marker-for-ar-js/) μετά έφτιαξα το marker στο **Photoshop** ώστε γράφει πάνω το σωστό DPSD και δημιούργησα την εικόνα **.png** και το αρχείο **.patt** από [εδώ](https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html) 
  - Μετά πρόσθεσα ένα `a-text` με τον **κώδικα** από [εδώ](https://levelup.gitconnected.com/simple-augmented-reality-ar-integration-with-a-frame-f625e9dc66b8) για να εμφανίζει το όνομα και το επίθετο μου [εδώ](https://aframe.io/docs/1.3.0/components/text.html)
  - Μετά πρόσθεσα ένα `a-image` με τον **κώδικα** από [εδώ](https://levelup.gitconnected.com/simple-augmented-reality-ar-integration-with-a-frame-f625e9dc66b8) για να εμφανίζει μια φωτογραφία της επιλογής μου και πείραξα το position 

## 2ο υποερώτημα 
-Αρχικά οι markers έχουν `type=pattern` οπότε για να αναγνωρίζονται τα markers έπρεπε να προσθέσω τον κώδικα μέσα στο  `a-scene` που βρήκα απο [εδώ](https://aframe.io/blog/arjs/)  
 - (hydromark-oxymark)Μετά έκανα ένα καινούργιο `a-marker` για τον marker του Hydrogen με το κώδικα από [εδώ](https://aframe.io/blog/arjs/) και άλλαξα το **value** επίσης έφτιαξα τους marker από [εδώ](https://jeromeetienne.github.io/AR.js/three.js/examples/marker-training/examples/generator.html) καθώς και τα animation τα έφτιαξα στη ζωγραφική 3d  και τα αποθήκευσα σε 3d object σε .jlb αρχείο και τα ανέβασα στα assets
   - Μετά πρόσθεσα ενα `a-image` μέσα στο marker έτσι ώστε να εμφανίζει την κάρτα του Hydrogen σαν φωτογραφία η οποία υπήρχε στο φάκελο με τα assets από πριν.
   - Μετά πρόσθεσα ενα `a-entity` μέσα στο marker έτσι ώστε να να καλέσω το `a-assets` του Hydrogen και μετά πείραξα το position και το scale ώστε να φαίνεται καλύτερα στην οθόνη και για το animation έβαλα την εντολή animation_rotate που βρήκα απο [εδώ](https://stemkoski.github.io/AR.js-examples/index.html)
   - Μετά έκανα ένα καινούργιο `a-marker` για τον marker του Oxygen με το κώδικα από [εδώ](https://aframe.io/blog/arjs/) και άλλαξα το **value**
   - Μετά πρόσθεσα ενα `a-image` μέσα στο marker έτσι ώστε να εμφανίζει την κάρτα του Oxygen σαν φωτογραφία η οποία υπήρχε στο φάκελο με τα assets από πριν.
   - Μετά πρόσθεσα ενα `a-entity` μέσα στο marker έτσι ώστε να να καλέσω το `a-assets` του Oxygen και μετά πείραξα το position και το scale ώστε να φαίνεται καλύτερα και για το animation έβαλα την εντολή animation_rotate που βρήκα απο [εδώ](https://stemkoski.github.io/AR.js-examples/index.html)
   -  Μετά πρόσθεσα ενα `a-image` μέσα στο marker έτσι ώστε να εμφανίζει την κάρτα του H2O(νερού) σαν φωτογραφία την οποία δημιούργησα στο **Photoshop**
   - Μετά μέσα στο Marker του οξυγόνου πρόσθεσα ενα `a-entity` ώστε να εμφανίζει το μοντέλο του H2O(νερού) και για το animation έβαλα την εντολή animation_rotate που βρήκα απο [εδώ](https://stemkoski.github.io/AR.js-examples/index.html)


## 3ο υποερώτημα 
- Αρχικά έβαλα τον κώδικα για το `Script` από [εδώ](https://stackoverflow.com/questions/61239107/how-to-get-marker-position-x-y-ar-js) το οποίο το βρήκα απο τα issues στο gitHub καθώς και από την αναφορά σε αυτό στη τελευταία διάλεξη και το τροποποίησα έτσι ώστε να ταιρίαζει με τους markers που είχα φτίαξει για το 2ο υποερώτημα. Μετά έβαλα μια `if-else` έτσι ώστε αν ο **Marker-Distance < 2** τότε να εμφανίζει το **animation του νερού H2O και τη κάρτα του** και να κρύβει  για το **Hydrogen**,**Oxygen** αλλιώς να εμφανίζει μεμονωμένα τα  **animation και τις κάρτες τους** για το **Hydrogen**,**Oxygen** αντίστοιχα και να κρύβει για το ** νερό H2O**
# 3rd Deliverable 


# Conclusions


# Sources
