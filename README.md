# :computer:  Appathon project for the course "Internet and Applications" 

# Περιγραφή Εργασίας
CTGOV-03: Χώρες στις οποίες έχουν λάβει χώρα Κλινικές Μελέτες γύρω από μία συγκεκριμένη Ασθένεια

# :book: Contents
Σκοπός να φτιάξουμε μία διαδικτυακή εφαρμογή που θα παρουσιάζει όλες τις χώρες στις οποίες έχουν λάβει χώρα κλινικές μελέτες για μία συγκεκριμένη Ασθένεια. Ως είσοδο θα λαμβάνει το όνομα της ασθένειας το οποίο θα το ορίζει ο χρήστης μέσω της web σελίδας ή κατάλληλου endpoint( π.χ. appathon-project.gr/countries_per_trial/{disease_name} και το output θα είναι οι χώρες ταξινομημένες ανάλογα με τον αριθμός των κλινικών μελετών που έχουν λάβει χώρα ο οποίος θα παρουσιάζεται είτε ως json είτε πάνω σε χάρτη.

Για τις ανάγκες τις εφαρμογής αυτής κατεβάσαμε όλες τις διαθέσιμες κλινικές δοκιμές (XML αρχεία) από το https://clinicaltrials.gov/ ώστε να φιλτράρουμε τις κλινικές μελέτες με βάση την ασθένεια και έπειτα να εντοπίσουμε τις χώρες. Τις μελέτες αυτές θα τις προσθέσουμε σε βάση δεδομένων μετά από κατάλληλη επεξεργασία ώστε να κρατάμε τα εξής πεδία : official_title, brief_title , acronym , nct_id , country

Εργαλεία :
  MySQL και 
  1) node-red ή
  2) html , css , javascript + χρήση google maps api καθώς και api για μετατροπή ονόματος χώρας σε συντεταγμένες ώστε να τοποθετηθούν ως markers στον χάρτη

# :pencil: Authors
The author of this project is: Roussis Dimitrios
