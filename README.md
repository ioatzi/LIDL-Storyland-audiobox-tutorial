**# LIDL-Storyland-audiobox-tutorial

![alt text](https://github.com/ioatzi/LIDL-Storyland-audiobox-tutorial/blob/main/Photos/image-0001.jpg)

Το συγκεκριμένο repository αποτελεί ένα παράδειγμα που αφορά την προσθήκη καινούργιων παραμυθιών στο LIDL Storyland κουτί και την δημιουργία καινούργιων nfc tags με την χρήση του arduino και του PN532 για την επιλογή-ενεργοποίηση των συγκεκριμένων ηχητικών κομματιών.

Βήμα 1

Για αρχή, θα πρέπει πρώτα να μετονομάσουμε το αρχείο ήχου που θέλουμε να προσθέσουμε στο LIDL Storyland με την εξής ονομασία "L0016" διότι το LIDL Storyland έχει ήδη κάποια αρχεία μέσα προεγκατεστημένα τα οποία είναι (L0010-L0015) και αυξάνονται τον αριθμό και δίνοντας τις ονομασίες από L0016 έως L0090 μπορούμε να προσθέσουμε και άλλα αρχεία ήχου.

Βήμα 2

Επόμενο βήμα είναι να μετατρέψουμε την κωδικοποίηση του ονόματος του αρχείο από αυτό που έχει σε UTF16 αυτό γίνεται με τη χρήση του προγράμματος kid3  το οποίο μπορείτε να κατεβάσετε κάνοντας χρήση του παρακάτω Link [https://kid3.kde.org/]. Οπως φαίνεται και απο την παρακάτω εικόνα θα πρέπει να επιλέξουμε το πεδίο τίτλος και πατόντας εκεί που λέει επεξεργασία ανόγει ένα παράθυρο όπου εκεί βλέπουμε τον τίτλο και τον τύπο. 
![alt text](https://github.com/ioatzi/LIDL-Storyland-audiobox-tutorial/blob/main/Photos/Kid3.png)

Βήμα 3

Στην συνέχεια και αφού έχουν προηγηθεί τα προηγούμενα βήματα ήρθε η ώρα να μετατρέψουμε το αρχείο mp3 σε smp. Αυτό θα γίνει κάνοντας χρήση του python script που βρίσκεται στο παρακάτω Link [https://github.com/oyooyo/audiocube]. Οδηγίες για την χρήση του python script και πως εκτελείται βρίσκεται στο παρακάτω Link [https://oyooyo.github.io/audiocube/devices/storyland/]. Θα πρέπει το αρχείο mp3 να βρίσκεται μέσα στο φάλελο audiocube όπως επίσης να γίνει χρήση της python με versio 3.7.
![alt text](https://github.com/ioatzi/LIDL-Storyland-audiobox-tutorial/blob/main/Photos/Convert%20mp3%20to%20smp%20file.JPG)

Βήμα 4

Αφού μετατρέψουμε το αρχείο του mp3 σε smp, συνδέουμε το LIDL Storyland κουτί μέσω καλώδιο micro-usb στον υπολογιστή και μεταφέρουμε το αρχείο smp στην sd κάρτα που εμφανίζεται.

Βήμα 5

Θα πρέπει για το κάθε αρχείο που προσθέτουμε στο LIDL Storyland κουτί να δημιουργήσουμε ένα ξεχωρηστό nfc tag με το όνομα που έχουμε δώσει στο αρχείο smp. Για να γίνει αυτό υπάρχουν δύο τρόπη. Ένας είναι μέσω κινητού τηλεφώνου με διαθέτι nfc τεχνολογία και ο άλλος τρόπος είναι με την χρήση του arduino και του περιφεριακού PN532.

Πρώτος τρόπος

[ttps://zapped.to/blog/program-an-nfc-tag-with-iphone/]

Δεύτερος τρόπος

Για να γράψουμε ένα nfc tag και συγκεκριμένα ένα NTAG213 κάνουμε χρήση του κώδικα [https://github.com/ioatzi/LIDL-Storyland-audiobox-tutorial/tree/main/Code%20for%20NFC%20tag] το οποίο τροποποιήθηκε απο αυτό το Link [https://github.com/dominicklee/Arduino-PN532-NTAG213] κατάληλα ώστε να γράφουμε την σωστή ονομασία στα nfc tag.Στην παρακάτω εικόνα φαίνεται η συνδεσμολογία του arduino με το PN532
![alt text](https://github.com/ioatzi/LIDL-Storyland-audiobox-tutorial/blob/main/Photos/arduino-pn532-serial.png)
[https://www.aliexpress.com/item/32848242166.html?spm=a2g0o.productlist.main.3.464ft9ett9etNX&algo_pvid=27b1dd17-a7db-43de-90bf-29f728195abc&algo_exp_id=27b1dd17-a7db-43de-90bf-29f728195abc-1&pdp_ext_f=%7B%22sku_id%22%3A%2210000001648506311%22%7D&pdp_npi=2%40dis%21USD%212.94%212.65%21%21%21%21%21%40212244c416726063535916724d0757%2110000001648506311%21sea&curPageLogUid=PV2jt75YJgIi]
