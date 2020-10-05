# Archon (Άρχων)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fbillniakas%2Farchon.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fbillniakas%2Farchon?ref=badge_shield)


```
      _____  
   __|_    |__  _____   ______  __   _  _____  ____   _  
  |    \      ||     | |   ___||  |_| |/     \|    \ | | 
  |     \     ||     \ |   |__ |   _  ||     ||     \| | 
  |__|\__\  __||__|\__\|______||__| |_|\_____/|__/\____| 
     |_____|                                            
```

## Ο πρώτος Ελληνικός Arch Linux Installer

Σκοπός αυτού του cli εγκαταστάτη είναι η εγκατάσταση του
βασικού συστήματος Arch Linux **ΧΩΡΙΣ** γραφικό περιβάλλον.
Προτείνεται η εγκατάσταση σε ξεχωριστό δίσκο για την 
αποφυγή σπασίματος του συστήματος σας. Το script αυτό 
παρέχεται χωρίς καμιάς μορφής εγγύηση σωστής λειτουργίας.

**You have been warned !!!**
## Τι κάνει;
* Ο Άρχων εγκαθιστά το βασικό σύστημα Arch Linux χωρίς την προσθήκη γραφικού περιβάλλοντος
* Αναγνωρίζει αν το PC όπου γίνεται η εγκατάσταση έχει BIOS ή UEFI και κάνει τις ανάλογες κατατμήσεις (partitions)
* Δημιουργεί ένα μόνο partition (root+home) και για swap χρησιμοποιεί το [systemD-swap](https://github.com/Nefelim4ag/systemd-swap)
* Εγκαθιστά τις multilib βιβλιοθήκες για υποστήριξη 32bit εφαρμογών
* Εγκαθιστά τις πηγές για υποστήριξη του AUR καθώς και το yaourt
## Σε ποιους απευθύνεται;
* Σε αυτούς που ήδη έχουν κάνει μερικές φορές την εγκατάσταση Arch Linux και γνωρίζουν τι κάνουν
* Σε αυτούς που θέλουν μια barebone εκδοχή του Arch Linux (πχ για server)
* Σε όσους θέλουν να πειραματιστούν σε μια εικονική μηχανή προτού αποπειραθούν να εγκαταστήσουν το Arch Linux στο PC τους

## Πως δουλεύει;
Στο root του Arch Linux LiveCD δίνουμε
```
$ wget https://raw.githubusercontent.com/billniakas/archon/master/archon.sh
$ sh archon.sh
```
Οι απαντήσεις που αφορούν το δίσκο όπου θα γίνει η εγκατάσταση θα πρέπει να είναι της μορφής
```
/dev/sdx
```
όπου x το γράμμα του δίσκου όπου θα γίνει η εγκατάσταση (πχ /dev/sda).


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fbillniakas%2Farchon.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fbillniakas%2Farchon?ref=badge_large)