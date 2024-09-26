# Map<K,V> 
- [Documentação Oficial](https://docs.oracle.com/javase/10/docs/api/java/util/Map.html) <br>
- É uma coleção de pares chave/valor <br>
- Não admite repetições do objeto chave <br>
- Os elementos são indexados pelo objeto chave (não possuem posição) <br>
- Acesso, inserção e remoção de elementos são rápidos <br> 
- **Uso comum**: cookies, local storage, qualquer modelo chave-valor <br>
  
## Principais Implementações:
- **HashMap** - mais rápido (operações O(1) em tabela hash) e não ordenado <br>
- **TreeMap** - mais lento (operações O(log(n)) em árvore rubro-negra) e ordenado pelo `compareTo` do objeto (ou `Comparator`) <br>
- **LinkedHashMap** - velocidade intermediária e elementos na ordem em que são adicionados <br>

## Alguns métodos importantes:
- `put(key, value)`, `remove(key)`, `containsKey(key)`, `get(key)` <br>
  - Baseado em `equals` e `hashCode` <br>
  - Se `equals` e `hashCode` não existir, é usada comparação de ponteiros <br>
- `clear()` <br>
- `size()` <br>
- `keySet()` - retorna um `Set<K>` <br>
- `values()` - retorna uma `Collection<V>` <br>
