# LIDL-Storyland-audiobox-tutorial
Το συγκεκριμένο repository αποτελεί ένα παράδειγμα που αφορά την προσθήκη καινούργιων παραμυθιών στο LIDL Storyland κουτί και την δημιουργία καινούργιον nfc tags με την χρήση του arduino και του PN532 για την επιλογή-ενεργοποίηση των συγκεκριμένων ηχιτικών κομματιών.

Βήμα 1
Για αρχή, θα πρέπει πρώτα να μετανομάσουμε το αρχείο ήχου που θέλουμε να προσθέσουμε στο LIDL Storyland με την εξής ονομασία "L0016" διότη το LIDL Storyland έχει ήδη κάποια αρχεία μέσα προεγκατεστημένα τα οποία είναι (L0010-L0015) και αυξάνοντα τον αριθμό και δίνοντας τις ονομασίες απο L0016 έως L0090 μπορούμε να προσθέσουμε και άλλα αρχεία ήχου.

Βήμα 2
Επόμενο βήμα είνα να μετατρέψουμε την κωδικοποίηση του ονοματος του αρχείο απο αυτό που έχει σε UTF16 αυτό γίνεται με τη χρήση του προγράμματος kid3  το οποίο μπορείτε να κατεβάσεται κάνοντας χρήση του παρακάτω Link [https://kid3.kde.org/].

Βήμα 3
Στην συνέχεια και αφού έχουν προηγηθεί τα προηγούμενα βήματα ήρθε η ώρα να μετατρέψουμε το αρχείο mp3 σε smp  
https://oyooyo.github.io/audiocube/devices/storyland/) it will convert the mp3 file in to smp file using python script.

https://github.com/oyooyo/audiocube






https://github.com/dominicklee/Arduino-PN532-NTAG213
