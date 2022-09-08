# Stack

**Topic**: #datastructures 
**Relevant topics**:  #algorithms 
**Info sources**: https://www.youtube.com/watch?v=A3ZUpyrnCbM&ab_channel=CSDojo
**Additional tags**: #flashcards
**Description**: LIFO

```cpp

template <typename T>
class Stack
{
private:

    T *data;
    int kapasitet, antall;

public:

    Stack(const int lengde = 200)
    {
        data = new T[lengde];
        kapasitet = lengde;
        antall = 0;
    }

    ~Stack() { delete[] data; }
  
    void display() const
    {
        for (int i = 0; i < antall; i++)
            cout << i << ": " << data[i] << "  ";
        cout << "\n\t'antall': " << antall << '\n';
    }

    bool empty() const { return (antall == 0); }

    T pop()
    {
        if (!empty())
            return (data[--antall]);
        else
            cout << "\nStack is empty!\n\n";
        return T();
    }

    void push(const T t)
    {
        if (antall < kapasitet)
            data[antall++] = t;
        else
            cout << "\nStack is already full!\n\n";
    }
};

```

## Questions

- Question one: Answer (Add colon)
- Question two: Answer


## Other notes

- [[Queue]]
- [[Breadth-first]]
- 