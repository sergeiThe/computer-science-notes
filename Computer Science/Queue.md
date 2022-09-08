# Queue

**Topic**: #datastructures 
**Relevant topics**:  #algorithms 
**Info sources**: https://www.youtube.com/watch?v=A3ZUpyrnCbM&ab_channel=CSDojo
**Additional tags**: #flashcards
**Description**: FIFO


```cpp
template <typename T>                //  'T': fleksibel datatype!
class Queue {

  private:
      T*  data;                      //  PEKER til array av typen 'T'.
      int kapasitet, antall,         //  Max.lengde og nåværende antall.
          forste, siste;             //  Indeks for første/siste element.

  public:                      //  Initierer medlemmer vha. default parameter:
      Queue(const int lengde = 200) {  data = new T[lengde];
                                       kapasitet = lengde;
                                       antall = forste = siste = 0;  }


      ~Queue()  {  delete [] data;  }  // Frigir allokert memory (vha.'new').


      void display() const {         //  Skriver HELE Queuens innhold:
          int indeks = forste;
          for (int i = 0; i < antall; i++) {
              cout << indeks << ": " << data[indeks++] << "  ";
              if (indeks == kapasitet) indeks = 0;
          }
          cout << "\n\t'antall': " << antall << "\t'forste': "
               << forste << "\t'siste': " << siste << '\n';
      }


      bool empty() const  {  return (antall == 0);  }   //  Tomt eller ei.


      T get() {                //  Returnerer (om mulig) det første elementet:
          T  verdi;            //  Elementet/verdien som skal returneres.
          if (!empty()) {      //  Elementer fortsatt igjen:
              verdi = data[forste++];  //  Tar vare på første. Øker til neste.
              antall--;                //  Totalantallet telles ned.
              if (forste == kapasitet) forste = 0;  //  Wrapper til starten?!!
              return verdi;            //  Returnerer unnalagret element.
          } else
              cout << "\nQueue is empty!\n\n";      //  Egen melding ??
          return T();
      }


      void put(const T t) {  //  Legger inn (om mulig) element bakerst i køen:
          if (antall < kapasitet) {    //  Fortsatt plass:
              data[siste++] = t;       //  Legger bakerst. Øker til neste inn.
              antall++;                //  Totalantallet telles opp.
              if (siste == kapasitet) siste = 0;    //  Wrapper til starten?!!
          } else
              cout << "\nQueue is already full!\n\n";      //  Egen melding ??
      }
};
```

## Rules

We may only store N-1 elements in the array, if the length of the array is N.

Add - enqueue
Remove - dequeue

## Demo

![[Pasted image 20220906091822.png]]
![[Pasted image 20220906092112.png]]


## Questions

- What if endPointer goes out of bounds?::It is placed in the beginning of the array if it has space. (circular array)
<!--SR:!2022-09-10,4,270-->
- Question two: Answer


## Relevant notes

- [[Stack]]
- [[Deque]]