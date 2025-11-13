# Άσκηση 2 - Ανάλυση Απαιτήσεων
## Τεχνολογία Λογισμικού - ΟΠΑ 2025-2026

Αυτό το repository περιέχει τα διαγράμματα UML για την άσκηση 2.

## 📁 Δομή Αρχείων

```
ERGASIA-2/
├── SE_2026_Ex_02.pdf           # Εκφώνηση άσκησης
├── diagrams/
│   ├── A_class_diagram.puml    # Διάγραμμα κλάσεων (Ερώτημα Α)
│   └── B_activity_diagram.puml # Activity diagram (Ερώτημα Β)
└── README.md                    # Αυτό το αρχείο
```

## 📋 Περιεχόμενο Ασκήσεων

### Ερώτημα Α: Διάγραμμα Κλάσεων UML - Σύστημα Διοδίων
Μοντέλο πεδίου για σύστημα διαχείρισης διοδίων που περιλαμβάνει:
- Καταγραφή διελεύσεων οχημάτων
- Χρεώσεις ανά σταθμό και κατηγορία οχήματος
- Εντοπισμό υπερβάσεων ταχύτητας
- Ενημέρωση αστυνομίας για παραβάσεις

### Ερώτημα Β: Activity Diagram - Επίδομα Πετρελαίου Θέρμανσης
Διάγραμμα δραστηριότητας για τη διαδικασία:
- Υποβολής αίτησης επιδόματος
- Ακολουθιακών ελέγχων επικύρωσης
- Έγκρισης/απόρριψης αίτησης

## 🛠️ Δημιουργία Διαγραμμάτων

Τα διαγράμματα είναι γραμμένα σε **PlantUML** format.

### Επιλογή 1: Online PlantUML Editor
1. Ανοίξτε το [PlantUML Online Editor](http://www.plantuml.com/plantuml/uml/)
2. Αντιγράψτε τα περιεχόμενα από τα `.puml` αρχεία
3. Κατεβάστε τα διαγράμματα ως PNG ή SVG

### Επιλογή 2: Visual Studio Code με PlantUML Extension
1. Εγκαταστήστε το [PlantUML extension](https://marketplace.visualstudio.com/items?itemName=jebbs.plantuml)
2. Εγκαταστήστε το Java (απαιτείται από το PlantUML)
3. Ανοίξτε τα `.puml` αρχεία
4. Πατήστε `Alt+D` για preview
5. Εξαγωγή σε PNG/SVG: Δεξί κλικ → "Export Current Diagram"

### Επιλογή 3: Command Line (με PlantUML jar)
```bash
# Κατεβάστε το plantuml.jar
wget https://sourceforge.net/projects/plantuml/files/plantuml.jar/download -O plantuml.jar

# Δημιουργία PNG
java -jar plantuml.jar diagrams/A_class_diagram.puml
java -jar plantuml.jar diagrams/B_activity_diagram.puml

# Δημιουργία SVG
java -jar plantuml.jar -tsvg diagrams/A_class_diagram.puml
java -jar plantuml.jar -tsvg diagrams/B_activity_diagram.puml
```

## 📄 Δημιουργία Τελικού PDF

### Μέθοδος 1: Χρήση Microsoft Word/LibreOffice
1. Δημιουργήστε νέο έγγραφο
2. Προσθέστε:
   - Αριθμό μητρώου και ονοματεπώνυμο στην κορυφή
   - Τίτλο "Άσκηση 2 - Ερώτημα Α"
   - Το διάγραμμα κλάσεων
   - Τίτλο "Άσκηση 2 - Ερώτημα Β"
   - Το activity diagram
3. Εξαγωγή ως PDF με όνομα: `αριθμός_μητρώου-επώνυμο-όνομα.pdf`

### Μέθοδος 2: Χρήση LaTeX
Δημιουργήστε ένα `.tex` αρχείο με τα διαγράμματα και compile σε PDF.

### Μέθοδος 3: Online PDF Tools
1. Χρησιμοποιήστε εργαλεία όπως το [Canva](https://www.canva.com/) ή [Google Docs](https://docs.google.com/)
2. Εισάγετε τα διαγράμματα
3. Εξαγωγή ως PDF

## ⚠️ Σημαντικές Παρατηρήσεις

- **ΥΠΟΧΡΕΩΤΙΚΟ**: Αναγραφή αριθμού μητρώου και ονοματεπώνυμου
- **ΥΠΟΧΡΕΩΤΙΚΟ**: Όνομα αρχείου: `αριθμός_μητρώου-επώνυμο-όνομα.pdf`
- **ΔΕΝ ΓΙΝΟΝΤΑΙ ΔΕΚΤΕΣ** χειρόγραφες απαντήσεις
- **Ημερομηνία παράδοσης**: 20/11/2025

## 📝 Επεξηγήσεις Διαγραμμάτων

### Διάγραμμα Κλάσεων (Α)
Το διάγραμμα περιλαμβάνει:
- **SταθμόςΔιοδίων**: Διαχείριση σταθμών
- **Όχημα**: Πληροφορίες οχημάτων με πινακίδα και κατηγορία
- **Διέλευση**: Καταγραφή κάθε διέλευσης
- **Διαδρομή**: Σύνδεση σταθμών με ελάχιστο χρόνο
- **ΠαράβασηΤαχύτητας**: Εντοπισμός παραβάσεων
- **ΣύστημαΔιαχείρισης**: Κεντρική διαχείριση και ενημέρωση αστυνομίας

### Activity Diagram (Β)
Η ροή περιλαμβάνει:
1. Υποβολή αίτησης με στοιχεία δικαιούχου
2. Ακολουθιακοί έλεγχοι:
   - Εγκυρότητα ΑΦΜ
   - Έλεγχος εισοδήματος (≤ 20.000€)
   - Έλεγχος προηγούμενης αίτησης
   - Εγκυρότητα αριθμού παροχής
3. Απόρριψη (με email) ή έγκριση με καταβολή επιδόματος

## 🔗 Χρήσιμοι Σύνδεσμοι

- [PlantUML Official Site](https://plantuml.com/)
- [PlantUML Class Diagram Guide](https://plantuml.com/class-diagram)
- [PlantUML Activity Diagram Guide](https://plantuml.com/activity-diagram-beta)
- [UML Distilled - Martin Fowler](https://martinfowler.com/books/uml.html)

---

**Καλή επιτυχία στην εργασία σας!** 🎓
